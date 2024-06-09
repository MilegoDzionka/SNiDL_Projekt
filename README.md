# SNiDL_Projekt


Jest to repozytorium na rzecz projektu na przedmiot Sieci Neuronowe i Deep Learning (SNiDL). Projekt dotyczny rozpoznawania i odczytywania tablic rejestracyjnych ze zdjęć.


# Instrukcja obsługi 

W Celu replikacji należy pobrać całą zawartość tego repozytorium. W plikach .ipnyb znajdują się ścieżki do plików/folderów. Należy ustawić główną sciężkę na lokalizacje folderu z pobranymi danymi. Powinno to wyglądać tak:

- Główny folder
  - :file_folder: CNN_Letters
  - :file_folder: Dane
  - README.md
  - Test_image.jpg
  - Raport.pdf 
  - best.pt
  - model.pt
  - [Python]Całość
  - [Python]Dzielenie
  - [Python]Szukanie
  - [Python]Klasyfikacja

 W razie problemów z pobraniem folderów, mamy również bezpośrednie linki do zbiorów [Dane](https://drive.google.com/file/d/1_FLU1zXT9rKYJLGNkzCDd0W6O1SSendz/view). Folder [CNN_Letter](https://www.kaggle.com/datasets/aladdinss/license-plate-digits-classification-dataset) po pobraniu należy nazwać własnie "CNN_Letter". Oba foldery można również pobrać używając takich [narzędzi](https://download-directory.github.io/?url=https%3A%2F%2Fgithub.com%2FMilegoDzionka%2FSNiDL_Projekt%2Ftree%2Fmain%2FDANE)
    

### Raport 
Raport znajduje się w pliku :notebook_with_decorative_cover: [Raport](Raport.pdf)

## Kod
Kod z szukaniem tablic na zdjęciu znajduje się w pliku [Wyszukiwanie]([Python]Wyszukiwanie.ipynb). <br />
Kod z dzieleniem tablicy na znaki znajduje się w pliku [Dzielenie]([Python]Dzielenie.ipynb). <br />
Kod z klasyfikacją znaków znajduje się w pliku.

## Prezentacja

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/dQw4w9WgXcQ/0.jpg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
### Zarys projektu

Projekt składa się z trzech kroków:

+ Znalezienie tablicy na zdjęciu z samochodem
+ Podzielenie tablicy na pojedyńcze znaki
+ Klasyfikacja pojedyńczych znaków oraz złączenie otrzymanych klas w numer tablicy W 

Do kroku pierwszego użyto architektury Yolov8. Drugi krok został zrobiony poprzez manipulowanie obrazem i szukanie odpowiednich boxów zawierających znaki. Ostatni krok to prosta sieć konwolucyjna stosowana do klasyfikacji. Kod z implementacją modelu Yolov8 można znaleźć w pliku (tu wstaw). Implementacja dzielenia tablicy znajduje się w pliku [Dzielenie](Dzielenie.ipynb).



## Zbiory danych
W trakcie tworzenia projektu użyto niejednego zbioru danych. Wśród zbiorów zawierających zdjecia samochodów i pozycje tablic rejestracyjnych (format PASCAL VOC) znajdują się [Car License Plate Detection](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection) oraz [Automatic Number Plate Recognition](https://www.kaggle.com/datasets/aslanahmedov/number-plate-detection). Zbiór użyty do nauki klasyfikatora cyfr i liter to [License Plate Digits Classification Dataset](https://www.kaggle.com/datasets/aladdinss/license-plate-digits-classification-dataset). Wszystkie zbiory danych można znaleźć w tym repozytorium.

## Ocena dokładności modelu

Ocena zbudowanych modeli jest nietrywialna. Nie dysponujemy zbiorem który zawierałby trójkę (obraz,współrzędne,numer) składającej się z obrazu, pozycją tablicy rejestracyjne na nim oraz numer tablicy rejestracyjnej na obrazie. Nawet gdybyśmy dysponowali to wybór funkcji błędu jest nietrywialny. Jednak ze względu na specyfikę problemu, kryterium oceny finalnego modelu zostało odpowiednio potraktowane. Szczegóły znajdują się w raporcie

