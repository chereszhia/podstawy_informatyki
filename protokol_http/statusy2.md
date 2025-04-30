Grupa statusów HTTP składa się z kodów odpowiedzi, które są podzielone na kilka kategorii (grup) w zależności od typu odpowiedzi, jaką serwer zwraca do klienta. Każda grupa ma swoje znaczenie, które pozwala zrozumieć, jaki jest wynik przetwarzania zapytania. Oto opis poszczególnych grup statusów:

1XX – Informacyjne
Statusy w tej grupie oznaczają, że zapytanie zostało przyjęte i serwer jeszcze nie zakończył przetwarzania zapytania. Klient powinien oczekiwać dalszych informacji.

100 Continue – Serwer otrzymał część zapytania i czeka na resztę. Klient może kontynuować wysyłanie zapytania.

101 Switching Protocols – Serwer zgadza się na zmianę protokołu, który został zadeklarowany przez klienta (np. z HTTP na WebSocket).

102 Processing (WebDAV) – Serwer przetwarza zapytanie, ale nie ma jeszcze odpowiedzi (używane w przypadku długotrwałych operacji).

2XX – Sukces
Statusy w tej grupie oznaczają, że zapytanie zostało pomyślnie przyjęte, zrozumiane i przetworzone przez serwer.

200 OK – Zapytanie zostało przetworzone pomyślnie, a odpowiedź zawiera żądane dane.

201 Created – Zasób został utworzony w odpowiedzi na zapytanie (np. w przypadku tworzenia nowego obiektu).

202 Accepted – Zapytanie zostało przyjęte, ale przetwarzanie może jeszcze nie być zakończone.

204 No Content – Serwer przetworzył zapytanie, ale nie ma zawartości do zwrócenia.

205 Reset Content – Prosi klienta o zresetowanie dokumentu wyświetlanego w przeglądarce (np. po przesłaniu formularza).

206 Partial Content – Serwer zwraca tylko część danych w odpowiedzi na zapytanie o część zasobu (np. pobieranie pliku w kawałkach).

3XX – Przekierowania
Statusy w tej grupie informują, że klient musi wykonać dodatkowe działania (np. wysłać nowe zapytanie), aby zakończyć operację.

301 Moved Permanently – Zasób został trwale przeniesiony do innego miejsca. Klient powinien używać nowego adresu w przyszłości.

302 Found – Zasób został tymczasowo przeniesiony. Klient powinien kontynuować używanie starego adresu w przyszłości.

303 See Other – Zasób powinien zostać pobrany z innego URI. Klient powinien wykonać zapytanie GET na wskazany adres.

304 Not Modified – Zasób nie został zmieniony od ostatniego pobrania, więc klient może używać zapisanej kopii.

307 Temporary Redirect – Zasób został tymczasowo przeniesiony. W przeciwieństwie do 302, metoda HTTP powinna pozostać niezmieniona.

308 Permanent Redirect – Zasób został trwale przeniesiony. Klient powinien używać nowego adresu w przyszłości, ale metoda zapytania pozostaje niezmieniona.

4XX – Błędy klienta
Statusy w tej grupie oznaczają, że zapytanie wysłane przez klienta jest błędne lub nieprawidłowe w kontekście serwera.

400 Bad Request – Zapytanie jest źle sformułowane, np. ma błędną składnię lub brakujące parametry.

401 Unauthorized – Klient nie jest autoryzowany do wykonania zapytania (np. brak lub niepoprawne dane logowania).

403 Forbidden – Klient nie ma uprawnień do wykonania zapytania, nawet jeśli jest autoryzowany.

404 Not Found – Zasób nie został znaleziony na serwerze.

405 Method Not Allowed – Użyta metoda HTTP (np. GET, POST) nie jest dozwolona dla wskazanego zasobu.

406 Not Acceptable – Serwer nie może dostarczyć żądanej treści w żądanym formacie.

408 Request Timeout – Serwer czekał zbyt długo na zapytanie od klienta i zakończył połączenie.

409 Conflict – Wystąpił konflikt podczas przetwarzania zapytania (np. podczas próby utworzenia zasobu, który już istnieje).

410 Gone – Zasób był kiedyś dostępny, ale teraz został trwale usunięty.

413 Payload Too Large – Zapytanie jest za duże, aby mogło zostać przetworzone przez serwer.

414 URI Too Long – URI zapytania jest za długie.

429 Too Many Requests – Klient wysłał zbyt wiele zapytań w krótkim czasie.

5XX – Błędy serwera
Statusy w tej grupie oznaczają, że wystąpił błąd po stronie serwera i zapytanie nie mogło zostać przetworzone.

500 Internal Server Error – Ogólny błąd serwera, który wskazuje na problem z przetwarzaniem zapytania.

501 Not Implemented – Serwer nie obsługuje danej metody HTTP.

502 Bad Gateway – Serwer działający jako brama lub proxy otrzymał błędną odpowiedź od serwera nadrzędnego.

503 Service Unavailable – Serwer jest chwilowo niedostępny (np. z powodu przeciążenia lub prac konserwacyjnych).

504 Gateway Timeout – Serwer bramy lub proxy nie otrzymał odpowiedzi od serwera nadrzędnego w wyznaczonym czasie.

505 HTTP Version Not Supported – Serwer nie obsługuje wersji protokołu HTTP użytej w zapytaniu.

Podsumowanie:
1XX: Informacje – zapytanie jest przyjmowane, ale proces nie jest zakończony.

2XX: Sukces – zapytanie zostało przetworzone pomyślnie.

3XX: Przekierowanie – konieczne są dodatkowe działania (np. zmiana adresu).

4XX: Błędy klienta – zapytanie jest błędne lub niepoprawne.

5XX: Błędy serwera – wystąpił problem z przetwarzaniem zapytania po stronie serwera.

Każdy z tych kodów pozwala precyzyjnie określić, co się stało z zapytaniem i jak klient (np. przeglądarka internetowa) powinien na nie zareagować.