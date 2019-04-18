# SISL Registry

This is a registry to host SISL's Julia packages.

To add the SISL registry run this command from the Julia REPL: 
```julia 
] registry add https://github.com/sisl/Registry
```

## Adding packages to the registry

For now, adding packages is only supported locally. To add `CoolPackage.jl` to the registry proceed as follow:
- clone the `CoolPackage.jl` repository 
- Use the script `registratura.jl` from https://github.com/sisl/registratura.
  ```
  julia registratura.jl add SISL path/to/CoolPackage
  ```
- push the changes to the registry to github
