In order to flash our panda board with our custom version

of code

We needed to do:

First get a dfu-tool compiled to flash the board.

```bash
sudo apt-get install autoconf
git clone https://github.com/dsigma/dfu-util
cd dfu-util
./autogen.sh
./configure
make
sudo make install
```

Then in `panda/board`:

```bash
make recover
```

With the panda plugged.




