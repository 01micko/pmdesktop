pmdesktop
=========

A simple library interface to Xlib to work out the "desktop" window ID.

It is design as a shared (or static) library for [pmck](https://github.com/01micko/pmck)
and similar programs (yet to be developed).

Build
-----
run:

```
./configure
```

then:

```
make
```

and as root:

```
make install
```

Some basic options to `configure` are provided. Run `configure --help`

Description
-----------
`libpmdesktop` is a simple library using the Xlib function `XQueryTree()`
which iterates through the window tree looking for an approriate entry
which matches the desktop then finds and returns that window ID.

There is one function

```Window find_root(Display *Display, int Screen, int DisplayWidth, int DisplayHeight)```

which returns an X Window.

Bugs
----
- may not work correctly with all window managers

Please report all bugs here.
