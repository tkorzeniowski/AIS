## AIS
Architektura i integracja systemów 17Z.

### Temat
System zbierania danych z bezprzewodowych mierników gazu/ciepła/energii elektrycznej. Zadaniem systemu jest zbieranie danych i naliczanie należnośc za zużyte medium.

### Etap 1
Architektura systemu zgodna z metodą '4+1 views' oraz podjęte (kluczowe) decyzje architektoniczne z wykorzystaniem modelu MAD 2.0.

**Interesariusze systemu:**
* dostawcy i operatorzy medium
* odbiorcy medium
* inkasenci
* operatorzy, administratorzy i serwisanci systemu
* twórcy systemu

**Widoki systemu:**
1. Logiczny - diagram klas
2. Deweloperski - diagram pakietów
3. Procesów - diagramy sekwencji
4. Fizyczny - diagram rozmieszczenia
5. Scenariusze - główe przypadki użycia systemu

**Kluczowe decyzje architektoniczne (MAD 2.0):**
* Hierarchia komponentów - centrala, koncentratory, liczniki
* Jednokierunkowa, przewodowa komunikacja licznika z koncentratorem
* Kominikacja koncentratora z centralą - inkasent
* Komunikacja koncentratora z inkasentem - Zigbee, UDP
* Częstość rozsyłu danych - 15 min
* Języki programowania urządzeń (liczników/koncentratorów) i aplikacji, bazy danych, ...

**Wykorzystane wzorce architektoniczne:**
* Widok poziomów abstrakcji: warstwy
* Widok przechowywania danych: współdzielone repozytorium
* Widok przepływu danych: przetwarzanie wsadowe
* Widok interakcji między komponentami: klient – serwer

### Etap 2
Architektura systemu przedstawiona w jezyku ArchiMate.
