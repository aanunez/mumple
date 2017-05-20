# Mumple

This is just going to be a collection of playful programs written in mumps and notes on how to do various things in GT.M

## Getting Started

[Installing GT.M](https://github.com/OSEHRA/VistA/blob/master/Documentation/InstallGTM.rst) - Vista has a great run dowing on intsalling gtm. I had zero issues when setting it up on Mint 18.1

[Fidelity Manual](http://tinco.pair.com/bhaskar/gtm/doc/books/pg/UNIX_manual/) - The lenghty Fidelity Manual on the workings of gtm, mostly useful to ctl+f for the $ variables.

[Mumps programm manual](http://mumps.sourceforge.net/docs.html) - Useful if you forget something trivial about mumps.

[An actual Mumps blog](https://youngmumpster.wordpress.com/) - Just thought this was cool

## Useful FYIs

```gtm``` will get you into an interactive mumps shell.

Inside of gtm, you'll want to set the current directory (or a dir named 'src' inside of it) as a [valid place to load routines from](http://tinco.pair.com/bhaskar/gtm/doc/books/pg/UNIX_manual/ch08s50.html#establishing_the_value_from_gtm_routine).
```s $zroutines=".(src) $gtm_dist"```

You'll want to link mumps to your usr/bin so you can compile from command line. Not sure why this isn't done by default.
```sudo ln -s /opt/gtm/mumps /usr/bin/mumps```

When working outside of gtm (i.e. using mumps) you'll need to manually set $gtm_dist
```
gtm_dist=/opt/gtm
export gtm_dist
```
