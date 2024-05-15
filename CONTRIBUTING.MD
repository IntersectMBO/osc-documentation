Contributions from those that Sit on the Open Source Committee are welcome. data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7

The following is a set of guidelines for contributing to the Consensus component
of Cardano. If you have suggestions on how to improve this document, please feel
free to [propose changes](#contributing-to-the-code) to it in a pull request.
Bear in mind that the document should remain simple.
See [the quick reference section](#quick-reference) if you are in a hurry.

# Documentation

Documentation should be a first-class citizen of the Consensus code base. We are
in the process of improving the Consensus documentation, and your improvement
proposals are welcome.

We have two types of documentation:

# Contributing to the code

The following sections contain some guidelines that should be followed when
contributing to the Consensus code base. Please take some time to go through
them. We do not expect newcomers to adhere to these guidelines perfectly, and we
will guide you through the process when reviewing your pull request.

## Quick reference

This section contain guidelines on what to check when making a pull request.

- When bumping version bounds on the dependencies *it is not necessary* to
  increase the package version number. See [this
  section](#updating-the-dependencies-bounds).
- When you want to create a changelog entry, follow [this and the following
  section](docs/website/contents/for-developers/ReleaseProcess.md#installing-scriv).

## Following our git process

Our [git process](docs/website/contents/for-developers/GitProcess.md) describes
the `git` practices we encourage when working with the code in this repository.

## Updating the documentation

When submitting a pull request, please look update the relevant parts of the
documentation (see [this section](#documentation)).

## Following the style guide

We have a [Haskell style
guide](docs/website/contents/for-developers/StyleGuide.md) that should be
followed when writing code in Consensus. Our style guide is not set in stone,
and improvements are always welcome.

## Formatting the code

We use `stylish-haskell` 0.14.6.0 for Haskell code formatting.

Either enable editor integration or call the script used by CI itself:

```bash
./scripts/ci/run-stylish.sh
```

When using Nix, you can use the following command, which will build and use
the right version of `stylish-haskell`.

```bash
nix develop -c ./scripts/ci/run-stylish.sh
```

# Generating documentation and setting up hoogle

To generate the documentation, use the documentation script:

```bash
./scripts/docs/haddocks.sh
```

Often times, it is useful to have a
[`hoogle`](https://github.com/ndmitchell/hoogle) server at hand, with the
packages and its dependencies. Our suggestion is to use
[`cabal-hoogle`](https://github.com/kokobd/cabal-hoogle) which is included in
the `nix` shell:

```bash
nix develop
$ cabal-hoogle generate
$ cabal-hoogle run -- server --local
```

This will fire a `hoogle` server at https://localhost:8080/ with the local
packages and their dependencies.

## Making and reviewing changes

If you are working on changing a **substantial** part of Consensus, it is
**important** that you contact the core developers first to discuss design
considerations (See section [Contacting the
developers](#contacting-the-developers)). This will help detecting any potential
problems with the change in the design phase, preventing misunderstandings and
frustrations later on in the process.

We maintain a changelog. If your pull request requires a changelog entry, please
follow [these
instructions](docs/website/contents/for-developers/ReleaseProcess.md#adding-a-changelog-fragment).
Even if your change doesn't require a changelog fragment, create an empty one as
CI will reject your change otherwise. We made this choice to ensure authors of
PRs would always take a moment to consider whether a changelog fragment should
be added for their PR. For more information see [our release
process](docs/website/contents/for-developers/ReleaseProcess.md).

When creating a pull-request (PR), it is **crucial** that the PR:

- has a clear description,

- targets the `main` branch (unless there is a good reason not to),

- is as small as possible, and

- is organized in a cohesive sequence of commits, each representing a
  meaningful, logical and reviewable step.

# Reporting a bug or requesting a feature

If you happen to encounter what you think is a bug or you wish there was some
feature that was added to Consensus, please
[open](https://github.com/IntersectMBO/ouroboros-consensus/issues/new/choose) an
issue in our [issue
tracker](https://github.com/IntersectMBO/ouroboros-consensus/issues/).

# Submitting pull requests

We monitorize the repository constantly so we should be aware if you open a
pull-request, however if some reasonable time passes and we miss your PR, feel
free to ping someone from the team.

# Contacting the developers

The core contributors to consensus codebase are:

-   [Christian Taylor](https://github.com/ThatGuyLLC)

-   [Terence McCutcheon](https://github.com/ranchhand87)

-   [Nicholas Clarke](https://github.com/nc6)

# Code of conduct

See [Cardano engineering
handbook](https://github.com/input-output-hk/cardano-engineering-handbook/blob/main/CODE-OF-CONDUCT.md)'s
code of conduct.
