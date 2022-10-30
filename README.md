# argparse Definitions

Definitions for [luarocks/argparse](https://github.com/luarocks/argparse) 0.7.1 to use with [sumneko/lua-language-server](https://github.com/sumneko/lua-language-server). The annotations have been manually re-written directly from the [docs](https://argparse.readthedocs.io/en/stable/parsers.html) and [source code](https://github.com/luarocks/argparse) to be parsable by the LSP.

## Usage

```jsonc
// settings.json
{
	"Lua.workspace.library": [
		// path to wherever this repo was cloned to
		"path/to/this/repo",
		// e.g. on Windows, "$USERPROFILE/Documents/LuaEnvironments/penlight"
	]
}
```

For a more detailed description of how to install a library of definition files, see the LSP's [wiki](https://github.com/sumneko/lua-language-server/wiki/Libraries).

## Types

The types provided by this library are:

* Classes, given as `argparse.[CLASS NAME]`. Every class is listed below:
  * `argparse`
  * `argparse.Parser`
	* `argparse.Argument`
	* `argparse.Option`
	* `argparse.Command`
* Aliases, given as `argparse.[ALIAS NAME]`. Every alias is listed blow:
  * `argparse.Converter`
	* `argparse.BuiltInActions`