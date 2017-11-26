# vfs
Abstract file mechanism for R

## Classes
* FSDriver
* FileSystem

## Proposed API
```R
library(vfs)
fs <- fsOpen(vfs-local::local-driver())
# or an S3 bucket
# fs <- fsOpen(vfs-s3::s3-driver(), credentials_file="/path/to/aws/credentials", bucket="https://bucket.s3.amazonaws.com")
fsSave(fs, path="/path/to/file", data=foo)
bar <- fsLoad(fs=, path="/path/to/file")
fsClose(fs)
```
