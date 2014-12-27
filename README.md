python-dtrace-tracker
=====================

tracking the implementation of DTrace probes in Python

Patches
-------

Several known patches, sourced from patches shipped in distribution packages and from the Python issue tracker, are collected here. Patches are named

    FRAMEWORK-SOURCE-OS.patch

where `FRAMEWORK` is `dtrace` or `systemtap`,  `SOURCE` is the distribution or Python issue ID the patch was extracted from, and `OS` is a `+`-separated list of the operating systems it purports to enable DTrace for.

Python bugs
-----------

1. [**Issue 4111: Add Systemtap/DTrace probes**][4111]

    Original issue.

1. [**Issue 13405: Add DTrace probes**][13405]

    Current DTrace tracking issue. Appears blocked on combined
    SystemTap and DTrace patch.

1. [**Issue 14776: Add SystemTap static markers**][14776]

    Current SystemTap tracking issues. Appears blocked on combined
    SystemTap and DTrace patch.

1. [**Issue 21590: Systemtap and Dtrace support**][21590]

    Combined tracking of 13405 and 14776. Appears inactive.

[4111]: http://bugs.python.org/issue4111
[13405]: http://bugs.python.org/issue13405
[14776]: http://bugs.python.org/issue14776
[21590]: http://bugs.python.org/issue21590

Useful references
-----------------
* [**Official DTrace guide**](http://dtrace.org/guide/preface.html)

* [**DTrace patch for Python 2.7.x and 3.x**](https://www.jcea.es/artic/python_dtrace.htm)

    jcea's lovingly-maintained DTrace patches for recent versions of Python.

* Python's [**`sys.settrace`**](https://docs.python.org/3.5/library/sys.html#sys.settrace)

    DTrace probes should eventually cover everything a system trace function gets called for.

* [**Understanding DTrace ustack helpers**](http://dtrace.org/blogs/dap/2013/11/20/understanding-dtrace-ustack-helpers/)

    Awesome breakdown of how the Node.js ustack helper was built.

* [**Python and DTrace in build 65**](https://blogs.oracle.com/levon/entry/python_and_dtrace_in_build)

    Notes on original Python ustack helper patch from the folks at Sun.

* [**Ruby DTrace probes and arguments**](https://web.archive.org/web/20070727033528/http://dev.joyent.com/projects/ruby-dtrace/wiki/Ruby+DTrace+probes+and+arguments)

    Probes added to Ruby by Joyent. May be lost to the sands of time?

* [**Official Python benchmark suite**](https://hg.python.org/benchmarks/file/100eee4adc4c/README.txt)

    For profiling performance impact of this patch. See dmalcom's thoughts on this: <http://bugs.python.org/issue4111#msg100173>
