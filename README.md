# Spagghetto

Good ass perl scripts for making a Spacchetti project work locally. See [spag-test](https://github.com/justinwoo/spag-test) for an example.

After you've read through some stuff in this repo, check out [Psc-Package2Nix](https://github.com/justinwoo/psc-package2nix) for a nicer way to work with your Psc-Package dependencies.

Blog post about this repo here: <https://qiita.com/kimagure/items/625070775da70b37b67e>

```
[bash:~/Code/spaghetto/testbed] master ギ ls -a
.  ..

[bash:~/Code/spaghetto/testbed] master ギ ../spacchetti-init
initialized Spacchetti project.

[bash:~/Code/spaghetto/testbed] master ギ ../spacchetti-install
wrote .spacchetti/spacchetti.json
Installing 3 packages
remote: Enumerating objects: 966, done.
remote: Total 966 (delta 0), reused 0 (delta 0), pack-reused 966
Receiving objects: 100% (966/966), 239.56 KiB | 679.00 KiB/s, done.
Resolving deltas: 100% (491/491), done.
From https://github.com/purescript/purescript-prelude
 * tag               v4.1.0     -> FETCH_HEAD
HEAD is now at 7a691ce Merge pull request #180 from LiamGoodacre/feature/ord-record
Initialized empty Git repository in /home/justin/Code/spaghetto/testbed/.spacchetti/prelude/v4.1.0/.git/
Installed .spacchetti/prelude/v4.1.0
remote: Enumerating objects: 188, done.
remote: Total 188 (delta 0), reused 0 (delta 0), pack-reused 188
Receiving objects: 100% (188/188), 24.22 KiB | 206.00 KiB/s, done.
Resolving deltas: 100% (66/66), done.
From https://github.com/purescript/purescript-console
 * tag               v4.1.0     -> FETCH_HEAD
HEAD is now at eee71b1 Merge pull request #18 from justinwoo/compiler/0.12
Initialized empty Git repository in /home/justin/Code/spaghetto/testbed/.spacchetti/console/v4.1.0/.git/
Installed .spacchetti/console/v4.1.0
remote: Enumerating objects: 318, done.
remote: Total 318 (delta 0), reused 0 (delta 0), pack-reused 318
Receiving objects: 100% (318/318), 44.53 KiB | 373.00 KiB/s, done.
Resolving deltas: 100% (135/135), done.
From https://github.com/purescript/purescript-effect
 * tag               v2.0.0     -> FETCH_HEAD
HEAD is now at a0abb5a Merge pull request #4 from purescript/compiler/0.12
Initialized empty Git repository in /home/justin/Code/spaghetto/testbed/.spacchetti/effect/v2.0.0/.git/
Installed .spacchetti/effect/v2.0.0

[bash:~/Code/spaghetto/testbed] master ギ ../spacchetti-sources
".spacchetti/console/v4.1.0/src/**/*.purs"
".spacchetti/prelude/v4.1.0/src/**/*.purs"
".spacchetti/effect/v2.0.0/src/**/*.purs"

[bash:~/Code/spaghetto/testbed] master ギ ../spacchetti-build && node -e "require('./output/Main').main()"
Compiling Type.Data.Row
Compiling Type.Data.RowList
Compiling Data.Symbol
Compiling Data.NaturalTransformation
Compiling Record.Unsafe
Compiling Data.Boolean
Compiling Control.Semigroupoid
Compiling Control.Category
Compiling Data.Show
Compiling Data.Unit
Compiling Data.Void
Compiling Data.Semiring
Compiling Data.HeytingAlgebra
Compiling Data.Semigroup
Compiling Data.Ring
Compiling Data.Eq
Compiling Data.BooleanAlgebra
Compiling Data.CommutativeRing
Compiling Data.Ordering
Compiling Data.EuclideanRing
Compiling Data.Ord.Unsafe
Compiling Data.Ord
Compiling Data.DivisionRing
Compiling Data.Field
Compiling Data.Monoid
Compiling Data.Bounded
Compiling Data.Function
Compiling Data.Functor
Compiling Control.Apply
Compiling Control.Applicative
Compiling Control.Bind
Compiling Control.Monad
Compiling Prelude
Compiling Data.Monoid.Multiplicative
Compiling Data.Monoid.Additive
Compiling Data.Semigroup.Last
Compiling Effect
Compiling Data.Semigroup.First
Compiling Data.Monoid.Endo
Compiling Data.Monoid.Disj
Compiling Data.Monoid.Conj
Compiling Data.Monoid.Dual
Compiling Effect.Unsafe
Compiling Effect.Uncurried
Compiling Effect.Console
Compiling Effect.Class
Compiling Test.Main
Compiling Main
Compiling Effect.Class.Console
Build succeeded.
Hello Spacchetti!
```
