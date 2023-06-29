# neoruby-debugger

`neoruby-debugger` is a Vim plugin that allows you to debug Ruby code using the Neovim interface. It integrates with the Neovim DAP (Debug Adapter Protocol) to provide a seamless debugging experience for Ruby developers.

## Installation

You can install `neoruby-debugger` using your favorite Vim plugin manager. Here's an example using [vim-plug](https://github.com/junegunn/vim-plug):

1. Add the following line to your Vim/Neovim configuration file:

   ```vim
   Plug 'neoruby/neoruby-debugger'
   ```

2. Save the configuration file and run the following command in Vim/Neovim:

   ```vim
   :PlugInstall
   ```

3. Restart Vim/Neovim to activate the plugin.

## Usage

### Configuration

The `neoruby-debugger` plugin provides several configuration options that can be customized using the `M.setup` function. You can modify the behavior of the debugger by passing an options table to `M.setup`.

Example usage of `M.setup`:

```lua
require('neoruby-debugger').setup({
  rdbg = {
    initialize_timeout_sec = 30,
    port = "${port}",
  },
})
```

The available configuration options include:

- `rdbg.initialize_timeout_sec` (number): The timeout value (in seconds) for initializing the debugger. Default is 20 seconds.
- `rdbg.port` (string): The port number used for the debugger. You can use the `${port}` placeholder to specify a dynamic port number.

You can modify these options according to your requirements.

### Debugging Ruby Files

To debug a Ruby file, you can use the following command:

```vim
:lua require('neoruby-debugger').debug_test()
```

This command will start a debug session for the current Ruby file. It will search for the closest test case above the cursor position and launch the debugger for that test.

### Debugging Last Run Test

To debug the last run test, you can use the following command:

```vim
:lua require('neoruby-debugger').debug_last_test()
```

This command will start a debug session for the last run test. It uses the previously recorded test name and test path to launch the debugger.

## Contributing

If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on the [neoruby-debugger GitHub repository](https://github.com/neoruby/neoruby-debugger). Your contributions are greatly appreciated!

## License

The `neoruby-debugger` plugin is open-source and licensed under the [MIT License](https://github.com/neoruby/neoruby-debugger/blob/main/LICENSE). You are free to use, modify, and distribute this software.
```
