# elm-compiler
Learning to compile elm

## :o: ghcup

```
✔✔ ghc   8.10.7   recommended,base-4.14.3.0 hls-powered
✔✔ cabal 3.6.2.0  latest,recommended                   
✔✔ hls   1.4.0    latest,recommended                   
✔✔ ghcup 0.1.17.3 latest,recommended  
```

## :a: Compile

* clone and compile

```
git clone https://github.com/elm/compiler.git && cd compiler && cabal run
```

* Linking (x86_64) on Mac M1 :heavy_check_mark:

```
...
Linking ~/compiler/dist-newstyle/build/x86_64-osx/ghc-8.10.7/elm-0.19.1/x/elm/build/elm/elm ...
Hi, thank you for trying out Elm 0.19.1. I hope you like it!
...
```

* execute

```
dist-newstyle/build/x86_64-osx/ghc-8.10.7/elm-0.19.1/x/elm/build/elm/elm 
```

## :b: compile aarch64

- [ ] Needs LLVM@9

```
<no location info>: error:
    Warning: Couldn't figure out LLVM version!
             Make sure you have installed LLVM between [9 and 13)
```

- [ ] Install LLVM

```
brew install llvm 
```

- [ ] Check architecture `arm64`

```
% file dist-newstyle/build/aarch64-osx/ghc-8.10.7/elm-0.19.1/x/elm/build/elm/elm
dist-newstyle/build/aarch64-osx/ghc-8.10.7/elm-0.19.1/x/elm/build/elm/elm: Mach-O 64-bit executable arm64
```
