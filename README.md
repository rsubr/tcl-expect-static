# TCL Expect Static Binary

Static build of [TCL Expect](https://wiki.tcl-lang.org/page/Expect) for Linux x64.

Download the [latest release](https://github.com/rsubr/tcl-expect-static/releases/download/v5.45.5/tcl-expect-static-5.45.5-linux64.tar.gz).

# Installation

Extract the binaries and files in `/opt/expect`.

```
cd /tmp
wget https://github.com/rsubr/tcl-expect-static/releases/download/v5.45.5/tcl-expect-static-5.45.5-linux64.tar.gz
cd /opt
tar xf /tmp/tcl-expect-static-5.45.5-linux64.tar.gz

/opt/expect/expect -v
```

## Notes
 - This binary is built using TCL 8.6.12 and Expect 5.45.5.
 - Build environment is alpine linux with `apk install alpine-sdk`.
 - TCL cannot work without an `init.tcl` file, the `/opt/expect/expect` shell script sets up the required environment and then calls the real expect binary.
