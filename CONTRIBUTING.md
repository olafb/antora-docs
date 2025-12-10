# Porady dotyczące tworzenia treści dokumentacji

Ten plik zawiera szczegóły dotyczące składni AsciiDoc (.adoc).

---

## 1. Nagłówki

AsciiDoc używa znaku `=` do oznaczania nagłówków:

```
= H1 - Tytuł dokumentu
== H2 - Sekcja
=== H3 - Podsekcja
==== H4 - Pod-podsekcja
```

---

## 2. Tekst i formatowanie

* **Pogrubienie:** `*tekst*`
* **Kursywa:** `_tekst_`
* **Podkreślenie:** `[underline]#tekst#`
* **Przekreślenie:** `[line-through]#tekst#`
* **Kod inline:** `` `kod` ``

---

## 3. Listy

### Lista punktowana

```
* Punkt 1
* Punkt 2
** Podpunkt 2.1
** Podpunkt 2.2
```

### Lista numerowana

```
. Punkt 1
. Punkt 2
.. Podpunkt 2.1
.. Podpunkt 2.2
```

---

## 4. Linki i obrazy

* **Link:** `link:https://example.com[Opis linku]`
* **Obraz:** `image::sciezka/do/obrazka.png[Alternatywny tekst]`

---

## 5. Bloki kodu

```
[source, javascript]
----
console.log('Hello, world!');
----
```

* Możesz zmienić język w nagłówku `[source, język]` (np. `python`, `bash`, `html`).

---

## 6. Cytaty i uwagi

* Cytat:

```
____
To jest cytat.
____
```

* Uwagi i ostrzeżenia:

```
[NOTE]
====
To jest notatka.
====

[WARNING]
====
To jest ostrzeżenie.
====
```

---

## 7. Tabele

```
[cols="1,2,3", options="header"]
|===
| Kolumna 1 | Kolumna 2 | Kolumna 3
| Wiersz 1  | Wiersz 1  | Wiersz 1
| Wiersz 2  | Wiersz 2  | Wiersz 2
|===
```

* `cols` definiuje szerokość i liczbę kolumn.
* `options="header"` oznacza pierwszą linię jako nagłówek tabeli.

---

## 8. Linki do sekcji i kotwice

* Tworzenie kotwicy: `[[unikatowa_kotwica]]`
* Odwołanie do sekcji: `<<unikatowa_kotwica, Tekst linku>>`

---

## 9. Linie poziome

```
'''
```

lub

```
'''[separator]
```

---

Więcej informacji o AsciiDoc: [https://docs.asciidoc.org/](https://docs.asciidoc.org/)
