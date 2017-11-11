# AIS

Liczniki jednokierunkowe
Stały dostęp do energii elektrycznej
Jedna stacja odbiorcza zbiera dane z liczników - niezależnie czy w bloku czy z zabudowy jednorodzinnej


Interesariusze:
Klienci indywidualni /firmy
Główny dostawca medium, sponsor systemu
Inkasent - zbierający odczyty z obszaru
Jednostka przetwarzająca odczyty - agregacja do faktury
Operatorzy / użytkownicy systemu / technicy i serwisanci, twórcy systemu (studenci, MY i ja i ty)



MAD 2.0
Dywersyfikacja rodzajów liczników - jedna stacja odbiorcza, wiele liczników nadających
Protokół przesyłowy - własny/IP/ ZigBee
Częstość rozsyłu danych - 15 min
Stałe łącze z centralą / człowiek zbierający dane
Skala zbierania odczytów do koncentratora - blok, osiedle, ...
Podział klientów - bloki, domki, firmy - ile koncentratorów na jakim obszarze
Zbierane dane - klient, odczyt, czas odczytu
Wykrywanie i reakcja na defekty
Bezpieczeństwo danych - szyfrowanie




Wzorce architektoniczne
Warstwowe rozmieszczenie komponentów (hierarchiczne)
Wspólne repozytorium zebranych odczytów
Klient serwer między licznikami a koncentratorem - komunikacja między komponentami
Przetwarzanie wsadowe - od inkasenta do centrali



Kluczowy scenariusz:
Licznik co 15 minut wysyła info do koncentratora, przychodzi inkasent zbiera dane z okolicy, wprowadza dane do systemu, system (+ administrator) co miesiąc wystawia fakturę
