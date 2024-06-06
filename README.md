# SNiDL_Projekt

[Wprowadzenie](#Wprowadzenie)

[Zarys projektu](#Zarys)

[Zbiory Danych](#Dane)

[Ocena modelu](#Ocena)

[Instrukcja obsługi](#Instrukcja)






## Wprowadzenie

Jest to repozytorium na rzecz projektu na przedmiot Sieci Neuronowe i Deep Learning (SNiDL). Projekt dotyczny rozpoznawania i odczytywania tablic rejestracyjnych ze zdjęć.


## Zarys

Projekt składa się z trzech kroków:

+ Znalezienie tablicy na zdjęciu z samochodem
+ Podzielenie tablicy na pojedyńcze znaki
+ Klasyfikacja pojedyńczych znaków oraz złączenie otrzymanych klas w numer tablicy

Do kroku pierwszego użyto architektury Yolov8. Drugi krok został zrobiony poprzez manipulowanie obrazem i szukanie odpowiednich boxów zawierających znaki. Ostatni krok to prosta sieć konwolucyjna stosowana do klasyfikacji. Kod z implementacją modelu Yolov8 można znaleźć w pliku (tu wstaw). Implementacja dzielenia tablicy znajduje się w pliku [Dzielenie](Dzielenie.ipynb).



## Dane
W trakcie tworzenia projektu użyto niejednego zbioru danych. Wśród zbiorów zawierających zdjecia samochodów i pozycje tablic rejestracyjnych (format PASCAL VOC) znajdują się [Car License Plate Detection](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection) oraz [Automatic Number Plate Recognition](https://www.kaggle.com/datasets/aslanahmedov/number-plate-detection). Zbiór użyty do nauki klasyfikatora cyfr i liter to [License Plate Digits Classification Dataset](https://www.kaggle.com/datasets/aladdinss/license-plate-digits-classification-dataset). Wszystkie zbiory danych można znaleźć w tym repozytorium.

## Ocena

Ocena zbudowanych modeli jest nietrywialna. Nie dysponujemy zbiorem który zawirałby trójkę (obraz,współrzędne,numer) składającej się z obrazu, pozycją tablicy rejestracyjne na nim oraz numer tablicy rejestracyjnej na obrazie. Nawet gdybyśmy dysponowali to wybór funkcji błędu jest nietrywialny. Jednak ze względu na specyfikę problemu, kryterium oceny finalnego modelu zostało odpowiednio potraktowane. Szczegóły znajdują się w raporcie

## Instrukcja

W celu umozliwienia zreplikowania naszych wyników ustaliliśmy seed, jego zmiana może istotnie wpłynać na otrzymane wyniki. Należy pobrać foldery $\textit{CNN\_Letter}$ oraz $\textit{CNN\_Cars}$
