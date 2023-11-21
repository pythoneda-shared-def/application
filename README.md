# Application

Definition for [pythoneda-shared-pythoneda](https://github.com/pythoneda-shared-pythoneda "pythoneda-shared-pythoneda")/[application](https://github.com/pythoneda-shared-pythoneda/application "application").

## How to declare it in your flake

Check the latest tag of this repository, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-shared-pythoneda-application = {
      [optional follows]
      url =
        "github:pythoneda-shared-pythoneda-def/application/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-shared-pythoneda-application-python38` 
- `#packages.[system].pythoneda-shared-pythoneda-application-python39` 
- `#packages.[system].pythoneda-shared-pythoneda-application-python310` 
- `#packages.[system].pythoneda-shared-pythoneda-application-python311`
