# **Porównanie modelu OSI i TCP/IP**

## **Różnice między modelami OSI i TCP/IP**
- **Liczba warstw**: Model OSI ma 7 warstw, a TCP/IP tylko 4.
- **Podział funkcji**: W modelu TCP/IP nie ma oddzielnych warstw sesji i prezentacji.
- **Praktyczność**: Model TCP/IP jest szeroko stosowany w Internecie, a OSI ma głównie charakter teoretyczny.
- **Protokół bazowy**: OSI nie przypisuje konkretnych protokołów do warstw, natomiast TCP/IP opiera się na standardowych protokołach, takich jak IP i TCP.

## **Tabela porównawcza warstw modeli OSI i TCP/IP**

| **Warstwa OSI**         | **Opis**                                | **Warstwa TCP/IP**       | **Opis**                          |
|-------------------------|-----------------------------------------|--------------------------|-----------------------------------|
| Warstwa aplikacji       | Interakcja użytkownika z siecią         | Warstwa aplikacji        | Zawiera protokoły HTTP, FTP, SMTP itp. |
| Warstwa prezentacji     | Formatowanie, szyfrowanie danych        | **Brak**                 | Funkcje zawarte w aplikacji      |
| Warstwa sesji           | Zarządzanie sesjami i połączeniami      | **Brak**                 | Funkcje zawarte w aplikacji      |
| Warstwa transportowa    | Zapewnia niezawodność transmisji        | Warstwa transportowa     | Obsługuje TCP, UDP               |
| Warstwa sieciowa        | Adresowanie i routowanie                | Warstwa internetowa      | Obsługuje IP, ICMP               |
| Warstwa łącza danych    | Kontrola dostępu do medium              | Warstwa dostępu do sieci | Obsługuje Ethernet, Wi-Fi        |
| Warstwa fizyczna        | Transmisja sygnałów przez medium        | **Brak**                 | Funkcje zawarte w dostępie do sieci |

---

# **Najpopularniejsze protokoły TCP/IP**

## **Przykłady popularnych protokołów**
- **HTTP/HTTPS** – Protokół przesyłania stron internetowych.
- **FTP** – Protokół przesyłania plików.
- **SMTP/POP3/IMAP** – Protokoły poczty elektronicznej.
- **DNS** – Zamienia nazwy domenowe na adresy IP.
- **DHCP** – Automatycznie przydziela adresy IP w sieci.
- **ICMP** – Służy do przesyłania komunikatów kontrolnych, np. w poleceniu `ping`.

