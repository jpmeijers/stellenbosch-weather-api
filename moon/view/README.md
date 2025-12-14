# Moon view

This endpoint returns a jpeg image of the moon as it looks like from the earth at the moment.

## Requirements

This script depends on xplanet.
This directory needs to contain the `xplanet` executable.
THe repo at https://github.com/jpmeijers/xplanet can be used to compile a statically linked binary of xplanet using the following command:

```
git clone https://github.com/jpmeijers/xplanet.git
cd xplanet
mkdir -p build
cd build
../configure LDFLAGS="-static -static-libgcc -static-libstdc++"
make
cd src
cp xplanet <this api>/moon/view
```
