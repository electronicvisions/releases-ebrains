# Releases of BrainScaleS-2 software for EBRAINS


## Full clone of all BSS-2 top-levels for EBRAINS

```
git clone --depth=2 https://github.com/electronicvisions/releases-ebrains .
git submodule update --init --depth=2
```


## Single top-level checkout

```
git clone --no-checkout --depth=2 https://github.com/electronicvisions/releases-ebrains .
# now select one top-level: pynn-brainscales, hxtorch, jaxsnn, oppulance
git sparse-checkout set "pynn-brainscales"
git checkout
git submodule update --init --depth=2 -- pynn-brainscales
```
