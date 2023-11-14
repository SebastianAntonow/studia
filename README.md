# Projekt XYZ - Repozytorium

To repozytorium zawiera kod źródłowy i dokumentację projektu XYZ.

## Zmiany

### Konfiguracja GIT

```bash
git config --global user.name "Twoje Imię Nazwisko"
git config --global user.email "adres@mailowy.edu"
```

### Inicjalizacja Repozytorium

```bash
git init
```

### Dodanie Plików i Pierwszy Komit

```bash
touch plik1.txt plik2.txt
git add plik1.txt plik2.txt
git commit -m "Dodanie plik1.txt i plik2.txt"
```

### Wprowadzenie Zmian i Drugi Komit

```bash
echo "Treść pliku 1" > plik1.txt
git add plik1.txt
git rm plik2.txt
git mv plik1.txt nowy_plik.txt
git commit -m "Zmiany w plikach"
```

### Dodanie .gitignore i Trzeci Komit

```bash
echo ".DS_Store" > .gitignore
git add .gitignore
git commit -m "Dodanie .gitignore"
```

### Historia rewizji
```bash
# Skrócony zapis historii
git log --oneline

# Wyświetlanie historii na gałęzi
git log --graph --oneline --all

```

### Tworzenie i łączenie gałęzi
```bash
# Utworzenie nowej gałęzi
git branch nowa_galaz
git checkout nowa_galaz

# Wprowadzenie zmian na nowej gałęzi
git add plik3.txt
git commit -m "Dodanie pliku3.txt"

# Powrót do głównej gałęzi
git checkout master

# Połączenie gałęzi
git merge nowa_galaz

```

### Sposoby na wyswietlanie log'u

```bash
# 1. Standardowy Log
git log

# 2. Skrócony Log
git log --oneline

# 3. Graficzny Log
git log --graph --oneline --all

# 4. Log Z Początkiem i Końcem
git log --since=2022-01-01 --until=2022-12-31

# 5. Log Z Plikiem
git log -- plik.txt

# 6. Log Z Pominięciem Mergów
git log --no-merges

# 7. Log z Numerycznymi Referencjami
git log --decorate

# 8. Log Zmian W Plikach
git log -p

```