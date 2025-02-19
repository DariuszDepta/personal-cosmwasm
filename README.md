[CosmWasm]: https://github.com/CosmWasm
[Task]: https://taskfile.dev/

# Personal customizations for [CosmWasm] projects

It is not uncommon for my personal preferences regarding the tools used in a project
to differ from the standards in projects I would like to work on, and [CosmWasm] is no exception.

This repository contains my personal configuration of tools, such as [Task],
for use in [CosmWasm] projects without needing to store them in their repositories.

The [global-gitignore](./global-gitignore) file contains global Git configuration
that should be stored in the user's home directory.

Do not forget to configure Git:

```shell
$ git config --global core.excludesFile '~/.gitignore'
```

In every [CosmWasm] repository, a symbolic link should be created that points
to the configuration files in this repository, all in lowercase,
exactly as specified in the global `.gitignore` file.

This ensures that my customized configuration files are globally ignored by Git,
preventing accidental commits to any [CosmWasm] repository. At the same time,
I can continue using my preferred tools seamlessly in my daily workflow.
