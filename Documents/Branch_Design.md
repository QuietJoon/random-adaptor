Branch Design
====

## Summary

Because Stack does not support Backpack yet, I have difficulties for developing.

* Need to develop `random-adaptor` with Non-Backpack version and Backpack version
* However, there are sharing code like package adopter like `Util.Adaptor.Random.SplitMix`.

## Resolver

### Use package-adapter branch and merge to Non-Backpack and Backpack branch

* master - Currently, Non-Backpack version
* design - Design of `random-adaptor`, may not needed
* bk - Backpack version branch
* non-bk - Non-Backpack version branch
* bare-adopter - Provide adopter template
  * SplitMix
  * ...

#### Issues

##### Where bare-adopter would depends on?

Considerable conditions:
* Before branching `bk` and `non-bk`
* But, enough template functions/structure are prepared in bare-adopter
