# Documentation

Imagine dictionary but worse.

# Modules

This section contain informations about functions that are available on this module.
~~Information about the bot's OOTB commands will be covered in the next segment, but I am lazy.~~

## dscord

Provide minimal setup for Discord bot hosting.
~~(but again, why you need a wrapper for a wrapper)~~

    import dscord
    dscord.load('system') # Pre-load extension
    dscord.run(TOKEN)

### `dscord.load(name: str, package='dscord.ext': str) -> None`

[`importlib.import_module(name, package)`](https://docs.python.org/3/library/importlib.html#importlib.import_module) equivalent. Loads `discord.py` extention from local library (`dscord.ext` by default).

`name`, `package` - Name of module and package

### `dscord.run(token: str) -> None`

Obviously [`discord.Client.run()`](https://discordpy.readthedocs.io/en/stable/api.html#discord.Client.run) equivalent.

`token` - Discord bot's access token