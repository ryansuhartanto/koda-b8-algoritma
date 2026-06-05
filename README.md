# Algortima

Konversi Suhu Celsius

## Deskripsi

1. Mulai
2. Masukan Suhu Sebagai Celsius
3. Masukan Type Sebagai tipe
4. Jika tipe sama dengan 'f' maka akan mengkonversi Farenheit, Celsius dikali 9 / 5 di tambah 32 dan akan di simpan di hasil
5. Jika tipe sama dengan 'k' maka suhu mengkonversi Kelvin,Celsius ditambah 273,15 dan disimpan sebagai hasil
6. Outputkan hasil
7. Selesai

## Flowchart

```mermaid
flowchart TD
  start@{shape: circle, label: "start"}
  stop@{shape: dbl-circ, label: "end"}
  unit@{shape: lean-r, label: "celsius"}
  type@{shape: lean-r, label: "tipe"}
  f@{shape: diamond, label: "tipe == 'f'"}
  k@{shape: diamond, label: "tipe == 'k'"}
  f_calc@{shape: rect, label: "hasil = celsius * 9 / 5 + 32"}
  k_calc@{shape: rect, label: "hasil = celsius + 273,15"}
  out@{shape: lean-r, label: "Hasil Konversi = {hasil}"}


  start-->unit-->type-->f

  f--true-->f_calc
  f--false-->k
  
  k--true-->k_calc
  k--false-->stop

  f_calc-->out
  k_calc-->out
  out-->stop
```

## Pseudocode

```pseudo
DECLARE celsius: INTEGER
DECLARE hasil: DOUBLE
DECLARE tipe: CHAR
INPUT celsius
INPUT tipe

IF tipe == 'f' THEN
  hasil <- celsius * 9 / 5 + 32
ELSEIF tipe == 'k' THEN
  hasil <- celsius + 273,15
ENDIF

OUTPUT "Hasil Konversi = ", hasil
```
