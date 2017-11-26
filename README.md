# vfs
Abstract file mechanism for R

## Classes
* FSDriver
* FileSystem

## Proposed API
```R
library(vfs)
fs <- fsOpen(vfs-local::local-driver())
fsSave(fs, path="/path/to/file", data=foo)
bar <- fsLoad(fs=, path="/path/to/file")
fsClose(fs=fs)
```
