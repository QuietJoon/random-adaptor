random-wrapper
====

Wrapper to switch among random packages simply.

## Supported random packages

* splitmix

## Planned random packages

* pcg-random
* mwc-random
* sfmt
* tf-random
* random

## Why do I need wrapper series?

Not only for unified function interface, but for benchmarking and comparing the performance of each libraries.

When you write a comparing benchmark, you may not need this.
However, when you write a real application, you may want to wrapper which helps easy switching among the packages.

