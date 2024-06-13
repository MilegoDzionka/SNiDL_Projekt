# SNiDL_Projekt


Jest to repozytorium na rzecz projektu na przedmiot Sieci Neuronowe i Deep Learning (SNiDL). Projekt dotyczny rozpoznawania i odczytywania tablic rejestracyjnych ze zdjęć.


# Instrukcja obsługi 

W Celu replikacji należy pobrać całą zawartość tego repozytorium. W plikach .ipnyb znajdują się ścieżki do plików/folderów. Należy ustawić główną sciężkę na lokalizacje folderu z pobranymi danymi. Powinno to wyglądać tak:

- Główny folder
  - :file_folder: CNN_Letter
  - :file_folder: Dane
    - :file_folder: data_images
        - :file_folder: test
        - :file_folder: train
        - :file_folder: val
    - data.yaml

  - README.md
  - Test_image.jpg
  - Raport.pdf 
  - best.pt
  - model.pt
  - [Python]Całość
  - [Python]Dzielenie
  - [Python]Szukanie
  - [Python]Klasyfikacja

 W razie problemów z pobraniem folderów, mamy również bezpośrednie linki do zbiorów [Dane](https://drive.google.com/file/d/1_FLU1zXT9rKYJLGNkzCDd0W6O1SSendz/view). Folder [CNN_Letter](https://www.kaggle.com/datasets/aladdinss/license-plate-digits-classification-dataset) po pobraniu należy nazwać własnie "CNN_Letter". Folder DANE musi być takiej samej postaci jak w repozytorium
 

    

### Raport 
Raport znajduje się w pliku :notebook_with_decorative_cover: [Raport](Raport.pdf)

## Kod
Kod z szukaniem tablic na zdjęciu znajduje się w pliku [Wyszukiwanie]([Python]Szukanie.ipynb). <br />
Kod z dzieleniem tablicy na znaki znajduje się w pliku [Dzielenie]([Python]Dzielenie.ipynb). <br />
Kod z klasyfikacją znaków znajduje się w pliku [Klasyfikacja]([Python]Klasyfikacja.ipynb). <br />
Kod z działającą predykcją znajduje się w pliki [Całość]([Python]Całość.ipynb)

## Prezentacja

[![IMAGE ALT TEXT HERE]([https://img.youtube.com/vi/dQw4w9WgXcQ/0.jpg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ](https://youtu.be/SbNnrgLuI0w))


## Zbiory danych
W trakcie tworzenia projektu użyto niejednego zbioru danych. Wśród zbiorów zawierających zdjecia samochodów i pozycje tablic rejestracyjnych (format PASCAL VOC) znajdują się [Car License Plate Detection](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection) oraz [Automatic Number Plate Recognition](https://www.kaggle.com/datasets/aslanahmedov/number-plate-detection). Zbiór użyty do nauki klasyfikatora cyfr i liter to [License Plate Digits Classification Dataset](https://www.kaggle.com/datasets/aladdinss/license-plate-digits-classification-dataset). Wszystkie zbiory danych można znaleźć w tym repozytorium.
