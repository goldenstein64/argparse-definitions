# Argparse Definitions

Definitions for [luarocks/argparse](https://github.com/luarocks/argparse) 0.7.1 to use with [LuaLS/lua-language-server](https://github.com/LuaLS/lua-language-server). The annotations have been manually re-written directly from the [docs](https://argparse.readthedocs.io/en/stable/parsers.html) and [source code](https://github.com/luarocks/argparse) to be parsable by the LSP.

Some features are missing from the library simply because the LSP doesn't support them. The most pressing feature is currently autocomplete for arguments to the `call` operator on classes. Supporting this would mean autocomplete is available for keys in property tables when creating instances and assigning their properties with a table, like `argparse() { [keys here] }`.

## Usage

```jsonc
// settings.json
{
	"Lua.workspace.library": [
		// path to wherever this repo was cloned to
		"path/to/this/repo",
		// e.g. on Windows, "$USERPROFILE/Documents/LuaEnvironments/argparse"
	]
}
```

For a more detailed description of how to install a library of definition files, see the LSP's [wiki](https://github.com/sumneko/lua-language-server/wiki/Libraries).

## Types

The types provided by this library are:

* Classes, given as `argparse.[CLASS NAME]`. Every class is listed below:
  * `argparse`
  * `argparse.Parser`
	* `argparse.Parser.PropertiesTable`
	* `argparse.Argument`
	* `argparse.Argument.PropertiesTable`
	* `argparse.Option`
	* `argparse.Option.PropertiesTable`
	* `argparse.Command`
	* `argparse.Command.PropertiesTable`
* Aliases, given as `argparse.[ALIAS NAME]`. Every alias is listed blow:
  * `argparse.Converter`
	* `argparse.Argument.Action`
	* `argparse.Parser.Action`
	* `argparse.BuiltInActions`
