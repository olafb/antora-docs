# Dokumentacja inEwi

To repozytorium zawiera projekt dokumentacji zbudowany w oparciu o Antora. Poniżej znajdziesz instrukcję, jak uruchomić dokumentację lokalnie — nawet jeśli nie masz jeszcze zainstalowanego Node.js ani npm.

---

## 1. Wymagania

Do generowania dokumentacji potrzebne są:

* Node.js (LTS)
* npm (instalowany automatycznie wraz z Node.js)

Sprawdź, czy masz już Node i npm:

```
node -v
npm -v
```

Jeśli obie komendy zwracają wersje, przejdź dalej.

---

## 2. Instalacja Node.js i npm (jeśli wymagane)

Jeśli nie masz Node.js, pobierz wersję LTS ze strony:
[https://nodejs.org/](https://nodejs.org/)

Zainstaluj z domyślnymi ustawieniami. Po instalacji sprawdź:

```
node -v
npm -v
```

---

## 3. Instalacja zależności projektu

W katalogu repozytorium uruchom:

```
npm install
```

Polecenie zainstaluje wszystkie wymagane paczki, w tym Antorę i narzędzia pomocnicze.

---

## 4. Uruchomienie dokumentacji w przeglądarce

Aby zbudować dokumentację i automatycznie otworzyć ją w przeglądarce, użyj:

```
npm start
```

Skrypt wykona:

1. zbudowanie dokumentacji komendą `npx antora antora-playbook.yml`
2. otwarcie wygenerowanego pliku HTML w domyślnej przeglądarce

Nie jest wymagany lokalny serwer — dokumentacja otwierana jest bezpośrednio ze statycznego pliku.

---

## 5. Lokalizacja wygenerowanych plików

Po zbudowaniu dokumentacji Antora generuje statyczny serwis w folderze:

```
build/
```

Główna strona znajduje się pod:

```
build/index.html
```

---

## 6. O Antora

Więcej informacji o Antora: [https://docs.antora.org/](https://docs.antora.org/)

---

