# Scoop Bucket Template

<!-- Uncomment the following line after replacing placeholders -->
[![Tests](https://github.com/js0ny/bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/js0ny/bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/js0ny/bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/js0ny/bucket/actions/workflows/excavator.yml)

Personal bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

This bucket contains manifests for software that

- I use but not included in the official bucket
- I maintain.

## Usage

After manifests have been committed and pushed, run the following:

```powershell
scoop bucket add js0ny https://github.com/js0ny/bucket
scoop install js0ny/<manifest>
```

## Naming

- The bucket name is `js0ny`.
- The manifest name is the same as the software name.
- The manifest ended with `-git` for software that is installed from the source code.
- The manifest ended with `-np` for software that is non-portable.
- The manifest ended with `-dotnet*` for software that requires .NET *.
    - These are softwares that I manually compiled with .NET *.
    - Native AOT published executables are not included in this category.

## Notes

- Symbolic Link this directory to `~\scoop\buckets\js0ny-local` for local testing before pushing to the repository.


## Manifests

### I maintain

- commandlinemedia-dotnet9
- renamedit
- renamedit-git

### I use

- ltspice
- ltspice17-np
