---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.12
    jupytext_version: 1.8.0
kernelspec:
  display_name: OCaml 4.11
  language: OCaml
  name: ocaml-jupyter
---

# Vaje

```{code-cell}
:tags: [remove-cell, remove-stdout]

(* Ko se v Jupytru prvič požene OCaml, program Findlib izpiše neko sporočilo.
   Da se to sporočilo ne bi videlo v zapiskih, je tu ta celica, ki sproži izpis,
   vendar ima nastavljeno, da je v zapiskih v celoti skrita. *)
```

## Naloga 1

Dopolnite lambda račun s celimi števili <u>`n`</u> in seštevanjem `e1 + e2`.  

- Dopolnite pravila za leno in neučakano izvajanje velikih in malih korakov. Komentirajte, kje se pojavijo ključne razlike.

## Naloga 2

Izračunajte spodnje izraze v lambda računu. Jasno označite korake izvajanja pri vsakem.

- `(\y -> (\x -> x + y)) 2 3`
- `(\y -> (\x -> x + x)) 2 3`
- `(\x -> x x) (\x -> x x)`

## Naloga 3

Razložite kaj naredijo naslednje funkcije za Churchova števila

- `\n f z -> f (n f z)`
- `\n f z -> n f (f z)`
- `\m n f z -> m f (n f x)`
- `\m n f z -> m (n f) z`
- `\m n -> n m`

## Naloga 4

Uporabite Churchovo kodiranje za predstavitev seznamov kot aplikacije `fold` na tem seznamu.
