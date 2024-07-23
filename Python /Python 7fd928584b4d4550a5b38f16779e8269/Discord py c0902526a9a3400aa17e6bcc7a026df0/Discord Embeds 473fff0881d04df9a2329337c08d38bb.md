# Discord Embeds

Discord embeds in `discord.py` allow you to create rich messages with various formatting options. Here's a comprehensive guide to using embeds, including all parameters.

### Creating an Embed

To create an embed, you use the `discord.Embed` class. Here's the basic structure:

```python
import discord

embed = discord.Embed(
    title="Title of Embed",
    description="Description of Embed",
    color=discord.Color.blue()  # You can use predefined colors or pass an integer for a custom color
)

```

### Parameters

Here are all the parameters you can use with `discord.Embed`:

1. **title** (str): The title of the embed.
2. **type** (str): The type of embed. Defaults to `"rich"`.
3. **description** (str): The main body text of the embed.
4. **url** (str): A URL that will make the title a hyperlink.
5. **timestamp** (datetime): A timestamp to display in the footer.
6. **color** (discord.Color or int): The color strip of the embed. You can use predefined colors or an integer for a custom color.

### Adding Fields

You can add fields to an embed using the `add_field` method:

```python
embed.add_field(name="Field Name", value="Field Value", inline=True)

```

Parameters for `add_field`:

- **name** (str): The name of the field.
- **value** (str): The value of the field.
- **inline** (bool): Whether the field should display inline with other fields.

### Setting Author

You can set an author for the embed:

```python
embed.set_author(name="Author Name", url="https://author.url", icon_url="https://author.icon.url")

```

Parameters for `set_author`:

- **name** (str): The name of the author.
- **url** (str): A URL that will make the author's name a hyperlink.
- **icon_url** (str): A URL to an image that will be displayed as the author's icon.

### Setting Footer

You can set a footer for the embed:

```python
embed.set_footer(text="Footer text", icon_url="https://footer.icon.url")

```

Parameters for `set_footer`:

- **text** (str): The footer text.
- **icon_url** (str): A URL to an image that will be displayed as the footer's icon.

### Setting Thumbnail

You can set a thumbnail image for the embed:

```python
embed.set_thumbnail(url="https://thumbnail.url")

```

Parameters for `set_thumbnail`:

- **url** (str): A URL to the image to be used as the thumbnail.

### Setting Image

You can set an image for the embed:

```python
embed.set_image(url="https://image.url")

```

### Complete Example

Here's a complete example of an embed with all parameters:

```python
import discord
from datetime import datetime

embed = discord.Embed(
    title="Embed Title",
    description="This is the description of the embed",
    color=discord.Color.blue(),
    url="https://example.com",
    timestamp=datetime.utcnow()
)

embed.set_author(
    name="Author Name",
    url="https://author.url",
    icon_url="https://author.icon.url"
)

embed.set_footer(
    text="Footer text",
    icon_url="https://footer.icon.url"
)

embed.set_thumbnail(url="https://thumbnail.url")
embed.set_image(url="https://image.url")

embed.add_field(name="Field 1", value="This is the value of field 1", inline=True)
embed.add_field(name="Field 2", value="This is the value of field 2", inline=True)
embed.add_field(name="Field 3", value="This is the value of field 3", inline=False)

# To send the embed
await channel.send(embed=embed)

```

### Sending an Embed

To send an embed, you use the `send` method of a `discord.TextChannel` or `discord.User`:

```python
await channel.send(embed=embed)

```

By using these parameters and methods, you can create rich and informative embeds to enhance your Discord bot's messages.