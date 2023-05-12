# MyAwesomePackage
A dummy package for the [Julia Concise Tutorial](https://syl1.gitbook.io/julia-language-a-concise-tutorial/language-core/11-developing-julia-packages)

To create a new package (let's say `MyPackage`):
- fork this package in your own or your organisation account (let's say `MyUser`)
- from the github interface:
  - edit the `README.md` file to update the badges
  - edit the `Project.toml` file to change package name, author, dependences and UUID (you can get a new UUID from a Julia prompt with `using UUIDs; uuid1()`) 
  - edit the file `.github/workflows/ci.yml` to update the package name
  - rename the file `src/MyAwesomePackage.jl` and edit its content (docstring and module name) to reflect the new name
  - in `docs/make.jl` rename all the occurrences of `MyAwesomePackage` to `MyPackage` (including the account/organisation name where to deploy the documentation)
  - update `docs/src/index.md` and `docs/src/anotherPage.md`
- get it in julia. From a Julia prompt type `] [ENTER]` to enter the `pkg` prompt and then `add git@github.com:MyUser/MyPackage.jl.git`
- declare you want to develop it. Still from the `pkg` prompt, type; `dev MyPackage`. Your new package will be in `[JULIA_ROOT]/dev/MyPackage`. 


[![](https://img.shields.io/badge/docs-stable-blue.svg)](https://sylvaticus.github.io/MyAwesomePackage.jl/stable)
[![](https://img.shields.io/badge/docs-dev-blue.svg)](https://sylvaticus.github.io/MyAwesomePackage.jl/dev)
[![Build status (Github Actions)](https://github.com/sylvaticus/MyAwesomePackage.jl/workflows/CI/badge.svg)](https://github.com/sylvaticus/MyAwesomePackage.jl/actions)
[![codecov.io](http://codecov.io/github/sylvaticus/MyAwesomePackage.jl/coverage.svg?branch=main)](http://codecov.io/github/sylvaticus/MyAwesomePackage.jl?branch=main)
