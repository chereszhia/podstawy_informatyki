Statusy HTTP są podzielone na pięć grup, które odpowiadają różnym rodzajom odpowiedzi serwera. Każda grupa ma swój zakres kodów, który wskazuje na specyficzny rodzaj odpowiedzi. Oto opis każdej grupy:

1. **1XX (Informacyjne)**:
   - **Zakres**: 100-199
   - **Opis**: Kody w tej grupie wskazują, że żądanie zostało odebrane, ale serwer wymaga dalszych działań. Są to odpowiedzi tymczasowe, informujące klienta, że przetwarzanie żądania trwa.
   - **Przykład**: `100 Continue` – klient może kontynuować wysyłanie danych, jeśli serwer nie odrzucił żądania.

2. **2XX (Sukces)**:
   - **Zakres**: 200-299
   - **Opis**: Kody statusu w tej grupie oznaczają, że żądanie zostało pomyślnie przetworzone przez serwer. Odpowiedzi te oznaczają, że wszystko przebiegło zgodnie z oczekiwaniami.
   - **Przykład**: `200 OK` – żądanie zostało pomyślnie przetworzone, a odpowiedź zawiera oczekiwane dane.
   
3. **3XX (Przekierowanie)**:
   - **Zakres**: 300-399
   - **Opis**: Kody statusu w tej grupie informują, że żądanie wymaga dalszych działań (np. przekierowanie użytkownika na inną stronę). Zwykle oznacza to, że zasób został przeniesiony na inny URL lub wymaga interakcji ze strony klienta.
   - **Przykład**: `301 Moved Permanently` – zasób został trwale przeniesiony na inny adres URL.

4. **4XX (Błąd klienta)**:
   - **Zakres**: 400-499
   - **Opis**: Kody w tej grupie oznaczają, że żądanie jest błędne lub zawiera niepoprawne dane. Zwykle oznacza to, że klient musi coś poprawić, aby żądanie mogło zostać poprawnie przetworzone przez serwer.
   - **Przykład**: `404 Not Found` – żądany zasób nie został znaleziony na serwerze.

5. **5XX (Błąd serwera)**:
   - **Zakres**: 500-599
   - **Opis**: Kody statusu w tej grupie wskazują, że wystąpił problem po stronie serwera. Żądanie zostało poprawnie odebrane, ale serwer napotkał problem podczas przetwarzania lub nie jest w stanie obsłużyć żądania.
   - **Przykład**: `500 Internal Server Error` – wystąpił nieoczekiwany błąd po stronie serwera.

