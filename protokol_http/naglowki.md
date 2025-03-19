odpowiedzi:

1) access-control-allow-credentials: true{

    Nagłówek Access-Control-Allow-Credentials: true informuje, że serwer zezwala na przesyłanie danych uwierzytelniających (takich jak ciasteczka) w ramach żądań między różnymi domenami. Oznacza to, że jeśli aplikacja frontendowa na jednej domenie wysyła żądanie do serwera na innej domenie, może towarzyszyć temu ciasteczko, które zawiera dane użytkownika, np. token sesji. Jednak, aby to działało, serwer musi też odpowiedzieć nagłówkiem Access-Control-Allow-Origin z określoną domeną, a nie * (czyli wszystkimi domenami). Ten nagłówek jest ważny w przypadku aplikacji, które muszą przechodzić między różnymi serwerami (np. frontend na jednej domenie, a backend na innej). W skrócie, umożliwia to autoryzację i przesyłanie danych między różnymi serwisami, zachowując bezpieczeństwo.

    }

2) access-control-allow-origin: null{
    Nagłówek Access-Control-Allow-Origin: null oznacza, że serwer zezwala na żądania pochodzące z określonych źródeł, ale tylko z "pustych" (null) źródeł. Często spotyka się go w sytuacjach, gdy aplikacja jest uruchomiona lokalnie (np. z plików bezpośrednio na dysku) lub gdy żądanie pochodzi z nieautoryzowanego źródła. Zwykle w przypadku CORS (Cross-Origin Resource Sharing) nagłówek Access-Control-Allow-Origin określa konkretną domenę, z której serwer akceptuje żądania. Jeśli jest ustawiony na null, oznacza to, że serwer może akceptować żądania tylko z takich źródeł, które nie są pełnoprawnymi domenami, np. w przypadku aplikacji uruchamianych lokalnie lub z protokołem file://. Może to ograniczyć możliwość wykonywania żądań między różnymi serwisami.
}
3) content-length: 791{
    Nagłówek "Content-Length: 791" informuje, że rozmiar treści (danych) w odpowiedzi HTTP wynosi 791 bajtów. Oznacza to, że cała zawartość, którą serwer zwróci w odpowiedzi na żądanie, ma dokładnie 791 bajtów. Ten nagłówek jest używany do informowania klienta (np. przeglądarki), ile danych ma otrzymać, co pozwala na odpowiednie przygotowanie odbioru tych danych. Jest to szczególnie ważne przy przesyłaniu danych, takich jak pliki czy duże odpowiedzi, aby klient mógł wiedzieć, kiedy otrzymał całą treść odpowiedzi.
}


zapytanie

1) :authority: httpbin.org{
    Nagłówek :authority: httpbin.org jest częścią protokołu HTTP/2 i wskazuje na nazwę hosta (domenę) serwera, do którego skierowane jest żądanie. W tym przypadku oznacza, że żądanie jest wysyłane do serwera o adresie httpbin.org. W HTTP/2 nagłówek :authority pełni rolę tradycyjnego nagłówka Host z HTTP/1.1, który również wskazuje na nazwę hosta, ale w HTTP/2 jest on używany w inny sposób, z bardziej zoptymalizowaną strukturą. Nagłówek ten pomaga serwerowi zrozumieć, który dokładnie serwis lub zasób jest żądany, zwłaszcza w przypadku, gdy na jednym serwerze hostowane są różne usługi.
}
2) :method: GET{
    Nagłówek ":method: GET" w żądaniu HTTP wskazuje, że jest to żądanie typu GET. Oznacza to, że klient (np. przeglądarka) prosi serwer o pobranie danych lub zasobów, bez wprowadzania jakichkolwiek zmian w danych na serwerze. Metoda GET jest jedną z podstawowych metod HTTP, która służy głównie do uzyskiwania zasobów (np. stron, plików) z serwera. W kontekście protokołu HTTP/2, nagłówek ":method" określa rodzaj operacji wykonywanej przez żądanie, a w tym przypadku jest to operacja pobierania danych (GET).
}
3) :path: /get{
    Nagłówek ':path: /get' wskazuje na ścieżkę w URL-u, do której wysyłane jest żądanie. W tym przypadku "/get" oznacza, że klient (np. przeglądarka) żąda zasobu dostępnego pod tym konkretnym adresem na serwerze. Ścieżka jest częścią URL-a, która określa, który zasób lub strona ma być pobrana z serwera. Na przykład, w przypadku pełnego adresu URL "https://httpbin.org/get", część "/get" jest ścieżką, która wskazuje, że klient żąda zasobu lub odpowiedzi związanego z tą ścieżką na serwerze "httpbin.org".
}
