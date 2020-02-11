# jormungandr-block0

block0 as a service

## how to extract block0 from a running instance:

replacing HASH by the expected block0 hash value:

```sh
sqlite3 stn/blocks.sqlite "select hex(block) from blocks where hash = x'<HASH>'" | xxd -r -p > block0.blk
```
