# Discord Bot

```python
import discord
from discord.ext import commands

intents = discord.Intents.all()
bot = commands.Bot(command_prefix='!', intents=intents)

@bot.event
async def on_ready():
    print("We have logged in as {0.user}".format(bot.user))

@bot.command()
async def hi(ctx):
    await ctx.send("Now you can make Chemixol bot -_-")

@bot.command()
async def table_base_unit(ctx):
    # Use forward slashes or double backslashes in the file path
    file = discord.File("C:/Users/Uttam/Desktop/Chemixol/c1/Base Physical Quantities.png")
    await ctx.send(file=file)

bot.run("YOUR_BOT_TOKEN")
```