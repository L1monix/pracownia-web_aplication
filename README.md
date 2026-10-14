# Elektro-Bud – analiza wymagań
## 1. Wymagania funkcjonalne

| ID | Nazwa |
|----|-------|
| FR-01 | Logowanie użytkownika |
| FR-02 | Wylogowanie użytkownika |
| FR-03 | Wyszukiwanie produktu |
| FR-04 | Sprawdzanie lokalizacji produktu |
| FR-05 | Przyjęcie towaru |
| FR-06 | Wydanie towaru |
| FR-07 | Kontrola stanu przy wydaniu |
| FR-08 | Przechowywanie stanu magazynowego |
| FR-09 | Rejestrowanie historii operacji |
| FR-10 | Przeglądanie stanów magazynowych |
| FR-11 | Zarządzanie produktami |
| FR-12 | Przeglądanie historii operacji |
| FR-13 | Raporty magazynowe |
| FR-14 | Zarządzanie kontami użytkowników |
| FR-15 | Nadawanie uprawnień |
| FR-16 | Obsługa zapomnianego hasła |
| FR-17 | Ograniczenie funkcji według roli |

## 2. Wymagania niefunkcjonalne

| ID | Kategoria | Nazwa |
|----|-----------|-------|
| NFR-01 | Wydajność | Czas wyszukiwania |
| NFR-02 | Wydajność | Czas operacji magazynowych |
| NFR-03 | Bezpieczeństwo | Przechowywanie haseł |
| NFR-04 | Bezpieczeństwo | Uwierzytelnianie |
| NFR-05 | Bezpieczeństwo | Szyfrowanie transmisji |
| NFR-06 | Kontrola dostępu | Role (RBAC) |
| NFR-07 | Spójność danych | Operacje współbieżne |
| NFR-08 | Audytowalność | Niezmienność historii |
| NFR-09 | Dostępność | Dostęp zdalny kierownika |
| NFR-10 | Dostępność | Dostępność systemu |
| NFR-11 | Niezawodność | Kopie zapasowe |
| NFR-12 | Użyteczność | Interfejs magazyniera |
| NFR-13 | Użyteczność | Komunikaty |
| NFR-14 | Skalowalność | Liczba użytkowników |
| NFR-15 | Przenośność | Kompatybilność |

## 3. Aktorzy

| Aktor | Rola | Podstawowe działania |
|-------|------|----------------------|
| **Użytkownik systemu** (abstrakcyjny) | Uogólnienie wspólne dla wszystkich ról; sam nie występuje w praktyce. | Logowanie, wylogowanie. |
| **Magazynier** | Bieżąca obsługa magazynu (3 osoby). | Wyszukiwanie produktów, sprawdzanie lokalizacji, przyjmowanie i wydawanie towaru. |
| **Kierownik magazynu** | Nadzór nad magazynem, potrzebuje szerszej informacji; może pracować poza magazynem. | Przeglądanie stanów, zarządzanie produktami, przeglądanie historii, raporty, wyszukiwanie produktów. |
| **Administrator** | Odpowiada za użytkowników i dostęp do systemu. | Zarządzanie kontami, nadawanie ról, reset haseł. |

## 4. Diagram przypadków użycia

Źródło PlantUML: [`use_case_diagram.puml`](use_case_diagram.puml) (renderowanie: plantuml.com lub rozszerzenie PlantUML w VS Code; wyeksportuj do `use_case_diagram.png` i dodaj do repozytorium).
