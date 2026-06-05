# Algortima

Cek bilangan ganjil/genap

## Deskripsi

1. Mulai
2. Masukan angka bilangan
3. Jika bilangan di modulus dengan 2 dan hasilnya adalah 0 maka angka tersebut adalah genap
4. Dan jika tidak maka angka tersebut adalah ganjil
5. Selesai

## Flowchart

```mermaid
flowchart TD
  start@{shape: circle, label: "start"}
  end@{shape: dbl-circ, label: "end"}
  input@{shape: lean-r, label: bilangan}
  calc@{shape: diamond, label: bilangan % 2 == 0}
  even@{shape: lean-r, label:  '"genap"'}
  odd@{shape: lean-r, label:  '"ganjil"'}

  start-->input-->calc
  calc--true-->even-->end
  calc--false-->odd-->end
```

## Pseudocode

```pseudo
DECLARE bilangan: INTEGER
INPUT bilangan

IF bilangan % 2 == 0 THEN
  OUTPUT "genap"
ELSE
  OUTPUT "ganjil"
ENDIF
```
