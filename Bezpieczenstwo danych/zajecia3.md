Skrocenie z 128 do 64 bylo strzalem w kolano.
Nastepca AES

# Ataki

1. **Brute force** - polega na generowaniu 2^56^ kluczy i sprawdzaniu ktory pasuje. Przy szyfrach 128bit juz gorzej, bo pamiec w kompie jest za mala zeby sobie z tym poradzic. Teraz minimum 256bit.
2. **Lamanie szyfrogramami** - odtwarzamy klucz na podstawie szyfrogramow ktore juz mamy. Ma zbior, porownuje zbior, na podstawie algorytmow wyciaga poszczegolne znaki. Najczestsza metoda, bo statystyczna. Ilosc materialow do analizy jest na tyle duza, ze mozna to spokojnie robic. Instalowane jest u nas malware i nasz komp jest uzywany do obliczen.
3. **Lamanie z wybranym tekstem jawnym** - analityk sam wybiera jaki tekst zostanie zaszyfrowany i na tej podstawie potem powoli lamie szyfr. Komunikacja z klientem wymaga jednorazowego klucza.
4. **Lamanie z wybranych szyfrogramem** - dosc rzadko stosowane bo trzeba miec dostep do szyfrogramu i do tekstow jawnych. Polega na porownywaniu i dekrypcji jawnego z niejawnym. Tez metoda statystyczna.
5. **Lamanie adaptacyjne z wybranym tekstem jawnym** - jako osoba seszyfrujaca moge wielokrotnie zmieniac tekst. Wpuszczam go, zmieniam, wpuszczam itd i patrze co sie zmienia zeby skumac jaki szyfr.
6. **Kryptoanaliza roznicowa** - miala zlamac DES szybko. Zaproponowalo ze z danym tekstem jawnym mozna na podstawie ksorowania (podwojny NOT) cos tam. Ale jest do dupy ogolnie.
7. **Atak urodzinowy** - paradoks dnia urodzin (23 osoby w grupie zeby dwie statystycznie byly urodzone tego samego dnia) wykorzystano do ataku na znalezienie costam kluczy szyfrujacych (SHA1).

# Czym jest kryptografia w praktyce?

Nigdy nie implementujemy algorytmow samodzielnie!
Implementracja algorytmow jest na tyle zlozona, ze ...

Oparte o matematyke binarna
Nie dotykamy algorytmow, ktore nie zostaly zweryfikowane wczesniej.

Wybierajac system do szyfrowania informacji: czy ktos juz korzystal, jaki by efekt i czy pasuje do tego co potrzebujemy.

## Co to jest bezpieczny system informatyczny?

Kevin Mitnick - poslugiwal sie phishing i metody socjotechnika - okreslil jako system zamkniety do ktorego nie ma dostepu zaden czlowiek.

Glowny problem bezpieczenstwa to ludzie.

Generowanie liczb pseudolosowych - np oparte o system operacyjny.

Przesylanie informacji - VPN. Bezposrednie wirtualne polaczenie wyciagniecie z niego danych jest niemal niemozliwe.

Najwieksze zagrozenie to ==socjotechnika==.

Byli pracownicy i niezabieranie dostepow.
