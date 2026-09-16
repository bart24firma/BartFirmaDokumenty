# BartFirmaDokumenty

Prywatna aplikacja desktopowa przeznaczona do zarządzania załącznikami dokumentów w ofertach Allegro.

## Zastosowanie

Aplikacja umożliwia właścicielowi konta Allegro:

- odczyt aktywnych ofert,
- wybór ofert,
- dodawanie dokumentów PDF jako załączników do wskazanych ofert,
- dodawanie m.in. instrukcji obsługi, instrukcji montażu oraz kart informacyjnych produktu.

Aplikacja jest przeznaczona wyłącznie do własnego użytku właściciela konta Allegro.

Nie świadczy usług dla innych sprzedawców.

## Uprawnienia Allegro REST API

Aplikacja korzysta wyłącznie z zakresów:

- `allegro:api:sale:offers:read`
- `allegro:api:sale:offers:write`

## Bezpieczeństwo

Aplikacja nie służy do zarządzania zamówieniami, płatnościami, wiadomościami ani danymi osobowymi.

Operacje edycji ofert są ograniczone do zarządzania załącznikami dokumentów.

## Nazwa aplikacji

BartFirmaDokumenty
## Wersje

### v1.2.0
Stabilna, zamrożona wersja produkcyjna.
Obsługa masowego dodawania dokumentów do ofert Allegro.

### v1.3.0
Wersja rozszerzona o bezpieczne usuwanie wybranych załączników z ofert.

Funkcja usuwania:
- działa tylko na zaznaczonych ofertach,
- najpierw może być uruchomiona w trybie testowym,
- zachowuje pozostałe załączniki,
- nie usuwa informacji GPSR,
- zapisuje stan przed i po zmianie,
- kontroluje, czy nie zmieniły się inne chronione pola oferty.
