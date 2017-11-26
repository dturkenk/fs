# vfs
Abstract file mechanism for R

## Classes
* FSDriver
* FileSystem

## Proposed API
```R
fs <- vfs::FileSystem(vfs-local::local-driver)
vfs::save(fs=fs, path="/path/to/file", data=foo)
vfs::close(fs=fs)
```
