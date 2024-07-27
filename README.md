# mini.jump2

A tweak to awesome [echasnovski/mini.jump](https://github.com/echasnovski/mini.nvim/blob/main/readmes/mini-jump.md) plugin, which allow jumping up to 2 length of characters.

## Default config

```lua
-- No need to copy this inside `setup()`. Will be used automatically.
{
  -- Module mappings. Use `''` (empty string) to disable one.
  mappings = {
    forward = 'f',
    backward = 'f',
    forward_till = 't',
    backward_till = 'T',
    repeat_jump = ';',
    -- 2 characters jump target
    forward2 = 's',
    backward2 = 'S',
  },

  -- Delay values (in ms) for different functionalities. Set any of them to
  -- a very big number (like 10^7) to virtually disable.
  delay = {
    -- Delay between jump and highlighting all possible jumps
    highlight = 250,

    -- Delay between jump and automatic stop if idle (no jump is done)
    idle_stop = 10000000,
  },
}
```
