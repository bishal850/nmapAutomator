# Contributing Guidelines

## Coding Standards

`nmapAutomator` is 100% POSIX compatible, and should run with `/bin/sh`. To keep it compatible, please try to follow these Coding Standards:
- Keep the current indentation and code structure. *You can use VSCode to automatically format it.*
- For any variables/functions added, please use Camel Casing 'e.g. `newVariable`'.
- For any output files, please use underscores `_` instead of spaces, and include the `${HOST}` in the name.
- Enclose all variables in `${}` 'e.g. `${myVar}`'
- Always quote the variables 'e.g. `echo "${my_var}"`', *unless you're doing shell-splitting.*
- Use POSIX commands where possible 'i.e. `awk`/`sed`', as some commands may not work with `sh` or older shells. *You may open an issue if you don't know how to write the command you need.*

Furthermore, you can always utilize code re-use, by looking for adding new recon options, by basing your pull request on existing options in the `reconRecommend()` function.