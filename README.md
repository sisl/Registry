# SISL Registry

This is a registry to host SISL's Julia packages.

To add the SISL registry run this command from the Julia REPL: 
```julia 
] registry add https://github.com/sisl/Registry
```

## Adding packages to the registry

For now, adding packages is only supported locally. To add `CoolPackage.jl` to the registry proceed as follow:
- clone the `CoolPackage.jl` repository 
- Use the script [`private_register.jl`](https://gist.github.com/MaximeBouton/8ddc2cff0bc9b664a34b3c165f35360d)
- uncomment the line `const private_reg_url = "https://github.com/sisl/Registry"` 
- run `julia private_register.jl path/to/CoolPackage`
- the script is going to open a PR in the Registry repository, check that it is correct, merge the PR and delete the branch.
