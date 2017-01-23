# Kyberia nginx build
This repository contains sources of kyberia nginx build for el5 with static libressl

## How to build
### Build srpm 
```bash
spectool -g -R SPECS/nginx-libre.spec
mock -r epel-5-x86_64 --buildsrpm  --sources SOURCES --spec SPECS/nginx-libre.spec
```

### Build rpm
```bash
mock -r epel-5-x86_64 nginx-1.11.6-1.kyberia.src.rpm
```