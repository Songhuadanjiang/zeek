

Getting Started
---------------

The best place to find information about getting started with Zeek is
our web site [www.zeek.org](https://www.zeek.org), specifically the
[documentation](https://docs.zeek.org/en/stable/index.html) section
there. On the web site you can also find downloads for stable
releases, tutorials on getting Zeek set up, and many other useful
resources.

You can find release notes in [NEWS](https://github.com/zeek/zeek/blob/master/NEWS),
and a complete record of all changes in [CHANGES](https://github.com/zeek/zeek/blob/master/CHANGES).

To work with the most recent code from the development branch of Zeek,
clone the master git repository:

`git clone --recursive https://github.com/zeek/zeek`

With all [dependencies](https://docs.zeek.org/en/stable/install/install.html#prerequisites)
in place, build and install:

`./configure && make && sudo make install`

Write your first Zeek script:

```zeek
# File "hello.zeek"

event zeek_init()
    {
    print "Hello World!";
    }
```

And run it:

`zeek hello.zeek`

For learning more about the Zeek scripting
language, [try.zeek.org](http://try.zeek.org) is a great resource.

Development
-----------

Zeek is developed on GitHub by its community. We welcome
contributions. Working on an open source project like Zeek can be an
incredibly rewarding experience and, packet by packet, makes the
Internet a little safer. Today, as a result of countless
contributions, Zeek is used operationally around the world by major
companies and educational and scientific institutions alike for
securing their cyber infrastructure.

If you're interested in getting involved, we collect feature requests
and issues on GitHub [here](https://github.com/zeek/zeek/issues) and
you might find
[these](https://github.com/zeek/zeek/labels/good%20first%20issue)
to be a good place to get started. More information on Zeek's
development can be found
[here](https://docs.zeek.org/en/current/devel/index.html), and information
about its community and mailing lists (which are fairly active) can be
found [here](https://www.zeek.org/community/).

License
-------

Zeek comes with a BSD license, allowing for free use with virtually no
restrictions. You can find it [here](https://github.com/zeek/zeek/blob/master/COPYING).


Tooling
-------

We use the following tooling to help discover issues to fix, amongst a number of
others.

- [Clang-Tidy](https://clang.llvm.org/extra/clang-tidy/)
- [Coverity](https://scan.coverity.com/projects/bro)
- [PVS-Studio](https://pvs-studio.com/en/pvs-studio/?utm_source=github&utm_medium=organic&utm_campaign=open_source) - static analyzer for C, C++, C#, and Java code.
