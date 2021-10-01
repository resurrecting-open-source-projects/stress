# stress

#### stress - tool to impose load on and stress test a computer system

## What is stress?

stress is a tool that imposes a configurable amount of CPU, memory, I/O,
or disk stress on a POSIX-compliant operating system and reports any errors
it detects.

stress is not a benchmark. It is a tool used by system administrators to
evaluate how well their systems will scale, by kernel programmers to evaluate
perceived performance characteristics, and by systems programmers to expose
the classes of bugs which only or more frequently manifest themselves when
the system is under heavy load.

## Help this project ##

stress needs your help. **If you are a programmer** and want to help a nice
project, this is your opportunity.

The original stress went unmaintained; the source of the last version, 1.0.4,
was [imported from Debian](https://snapshot.debian.org/package/stress/).
After, patches from Debian and other changes were applied to create the 1.0.5
release. The details of each release are registered in the [ChangeLog](ChangeLog)
file. Now, stress is maintained by volunteers under [Resurrecting Open Source
Projects](https://github.com/resurrecting-open-source-projects).

If you are interested in helping stress, read the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## Building

From a Unix command line, building is simple:

```
./autogen.sh
./configure
make
make install
```

## Author ##

stress was originally developed by Amos Waterland <apw@rossby.metr.ou.edu>,
under the GPL-2+ license.

The original download sites were http://people.seas.harvard.edu/~apw/stress
and http://weather.ou.edu/~apw/projects/stress/

Currently, source code is maintained by volunteers. Newer versions are
available at https://github.com/resurrecting-open-source-projects/stress
