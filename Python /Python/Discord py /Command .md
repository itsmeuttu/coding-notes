# / Command

Discord bot using Python with `discord.app_commands.CommandTree`:

### Setting Up the Bot

1. **Install the required libraries**:
    
    ```bash
    pip install discord.py
    
    ```
    
2. **Create the bot**:
    
    ```python
    import discord
    from discord.ext import commands
    from discord import app_commands
    
    intents = discord.Intents.all()
    bot = commands.Bot(command_prefix='!', intents=intents, status=discord.Status.do_not_disturb, activity=discord.Game(name='Playing with Integration'))
    
    @bot.event
    async def on_ready():
        await bot.tree.sync()
        print(f'Logged in as {bot.user}!')
    
    bot.run('YOUR_BOT_TOKEN')
    
    ```
    

### Adding Slash Commands

1. **Create a simple slash command**:
    
    ```python
    @bot.event
    async def on_ready():
        await bot.tree.sync()
        print(f'Logged in as {bot.user}!')
    
    @bot.tree.command(name="hello")
    async def hello(interaction: discord.Interaction):
        await interaction.response.send_message("Hello! How can I assist you today?")
    
    ```
    
2. **Command with options**:
    
    ```python
    @bot.tree.command(name="greet")
    @app_commands.describe(name="The name of the person to greet")
    async def greet(interaction: discord.Interaction, name: str):
        await interaction.response.send_message(f"Hello, {name}!")
    
    ```
    
3. **Command with choices**:
    
    ```python
    @bot.tree.command(name="choose")
    @app_commands.choices(color=[
        app_commands.Choice(name="Red", value=1),
        app_commands.Choice(name="Green", value=2),
        app_commands.Choice(name="Blue", value=3),
    ])
    async def choose(interaction: discord.Interaction, color: app_commands.Choice[int]):
        await interaction.response.send_message(f"You chose {color.name}!")
    
    ```
    
4. **Command with subcommands**:
    
    ```python
    class MyGroup(app_commands.Group):
        @app_commands.command(name="subcommand1")
        async def subcommand1(self, interaction: discord.Interaction):
            await interaction.response.send_message("This is subcommand 1")
    
        @app_commands.command(name="subcommand2")
        async def subcommand2(self, interaction: discord.Interaction):
            await interaction.response.send_message("This is subcommand 2")
    
    bot.tree.add_command(MyGroup(name="group", description="A group of commands"))
    
    ```
    
5. **Handling errors**:
    
    ```python
    @bot.tree.error
    async def on_app_command_error(interaction: discord.Interaction, error: app_commands.AppCommandError):
        await interaction.response.send_message(f"An error occurred: {error}", ephemeral=True)
    
    ```
    

### Syncing Commands

To ensure that the commands are registered and updated properly:

```python
@bot.event
async def on_ready():
    await bot.tree.sync()
    print(f'Logged in as {bot.user}!')

```

### Running the Bot

Make sure you have your bot token and run your script:

```python
bot.run('YOUR_BOT_TOKEN')

```

### Defining the Command

1. **Decorator for Command Registration**:
    
    ```python
    @bot.tree.command(name="greet")
    
    ```
    
    - `@bot.tree.command`: This decorator registers a new slash command.
    - `name="greet"`: Specifies the name of the slash command. This is the command users will type in the chat (e.g., `/greet`).
2. **Decorator to Describe the Command's Options**:
    
    ```python
    @app_commands.describe(name="The name of the person to greet")
    
    ```
    
    - `@app_commands.describe`: This decorator provides a description for the command's parameters.
    - `name="The name of the person to greet"`: Describes the `name` parameter, making it clear to users what they should provide.

### Command Function

1. **Async Function Definition**:
    
    ```python
    async def greet(interaction: discord.Interaction, name: str):
    
    ```
    
    - `async def greet`: Defines an asynchronous function named `greet`. The function will be executed when the slash command is invoked.
    - `interaction: discord.Interaction`: Represents the interaction with the Discord API when a user invokes the command. This object provides context and methods to respond to the command.
    - `name: str`: A string parameter that will be provided by the user when invoking the command. This is the name of the person to greet.
2. **Sending a Response**:
    
    ```python
    await interaction.response.send_message(f"Hello, {name}!")
    
    ```
    
    - `await interaction.response.send_message`: Sends a message in response to the interaction.
    - `f"Hello, {name}!"`: A formatted string that includes the `name` provided by the user, resulting in a personalized greeting message.

### Full Code for Reference

Here’s the complete code snippet with all components explained:

```python
@bot.tree.command(name="greet")
@app_commands.describe(name="The name of the person to greet")
async def greet(interaction: discord.Interaction, name: str):
    await interaction.response.send_message(f"Hello, {name}!")

```

### Explanation Recap

- **@bot.tree.command(name="greet")**: Registers the command `/greet`.
- **@app_commands.describe(name="The name of the person to greet")**: Describes the `name` parameter for user clarity.
- **async def greet(interaction: discord.Interaction, name: str)**: Defines the function to handle the command.
- **await interaction.response.send_message(f"Hello, {name}!")**: Sends a personalized greeting as a response to the command.