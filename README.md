# xdg-open-wsl

This implements a simple binary that implements `xdg-open` for WSL.


## Install

Via `cargo`:
```
cargo install --git https://github.com/LucioFranco/xdg-open-wsl
```

Via `nix`:

```nix
# flake.nix
xdg-open-wsl = {
    url = "github:LucioFranco/xdg-open-wsl";
};

# imported to your home-manager packages like so
home.packages = [
    inputs.xdg-open-wsl.packages."x86_64-linux".xdg-open
];
```

