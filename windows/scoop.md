# Scoop
A command-line installer for Windows
Scoop homepage: [Scoop](https://scoop.sh/)

## Install Scoop
```powershell
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser # Optional: Needed to run a remote script the first time
> irm get.scoop.sh | iex
```


## Buckets management

#### List
```powershell
scoop bucket list #list added buckets
scoop bucket known #list remote buckets
```

#### Add
``` powershell
scoop bucket add extras
```

#### Install, Uninstall, Update, Cleanup
```powershell
scoop install nano
scoop uninstall nano
scoop update *
scoop cleanup *
```

#### Example tools
1. sudo
2. gsudo
3. nano


