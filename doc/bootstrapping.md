Bootstrapping Mafia
===================

Mafia is required to build Mafia. Fortunately there is a script that will
bootstrap build it from a git checkout as follows:

```shell
git clone https://github.com/ambiata/mafia/
cd mafia
script/mafia build
```

This will build a `mafia` binary which will be at `dist/build/mafia/mafia`
which you can then copy to a directory on your `PATH` like for instance
`$HOME/bin`.

Once you have a `mafia` binary and you want to build a newer version of `mafia`
is simply a process of going to your mafia git checkout, pulling the latest
version from Github and then:

```shell
mafia build
cp dist/build/mafia/mafia $(which mafia)
```

which builds it and copies it over the old binary.
