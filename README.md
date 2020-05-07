random-adaptor
====

Adaptor to switch among random packages easily.

## Random package support status

### Supported

* splitmix

### Planned

* tf-random
* random

### Postponed

Because they do not provide pure interfaces, Need to write IO monad wrapper and generalization for pure packages.

* pcg-random
* mwc-random
* sfmt

## Limitation

* Only for pure interface (`IO` or `ST` monad interfaces are not supported yet)
* The dependency footprint is too big because of the character of the package
  * This can be resolved by providing an adaptor package for each random package, but this means that there would be very many packages.

## Why do I need adaptor series?

Not only for a unified function interface, but for benchmarking and comparing the performance of each library.

When you write a comparing benchmark, you may not need this.
However, when you write a real application, you may want an adaptor which helps easy switching among the packages.

## How about Backpack instead of Adaptor series?

Yes, Backpack is a beautiful feature.
However, even with Backpack, when the interfaces among the target packages are not the same, we still needs an Adaptor package.
