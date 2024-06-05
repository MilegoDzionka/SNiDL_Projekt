# SNiDL_Projekt

[Wprowadzenie](#Wprowadzenie)

[Zarys projektu](#Zarys)

[Instrukcja obsługi](#Instrukcja)



## Wprowadzenie

Jest to repozytorium na rzecz projektu na przedmiot Sieci Neuronowe i Deep Learning (SNiDL). Projekt dotyczny rozpoznawania i odczytywania tablic rejestracyjnych ze zdjęć.


## Zarys

Projekt składa się z trzech kroków:

+ Znalezienie tablicy na zdjęciu z samochodem
+ Podzielenie tablicy na pojedyńcze znaki
+ Klasyfikacja pojedyńczych znaków oraz złączenie otrzymanych klas w numer tablicy

Do kroku pierwszego użyto architektury Yolov8. Drugi krok został zrobiony poprzez manipulowanie obrazem i szukanie odpowiednich boxów zawierających znaki. Ostatni krok to prosta sieć konwolucyjna stosowana do klasyfikacji.
