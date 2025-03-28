# Topologie sieci

## Topologie fizyczne

### 1. Magistrala (Bus)

**Opis:** Wszystkie urządzenia są podłączone do jednej głównej magistrali (kabla), przez który przesyłane są dane.

**Zalety:**

- Niska cena implementacji
- Prosta struktura

**Wady:**

- Awaria głównego kabla powoduje unieruchomienie całej sieci
- Niska skalowalność

**Zastosowanie:**

- Małe sieci lokalne (LAN) o ograniczonej liczbie urządzeń

### 2. Pierścień (Ring)

**Opis:** Urządzenia są połączone w zamknięty pierścień, gdzie dane przesyłane są w jednym kierunku.

**Zalety:**

- Brak kolizji danych
- Przewidywalna wydajność sieci

**Wady:**

- Awaria jednego węzła może zakłócić działanie całej sieci
- Trudna rozbudowa

**Zastosowanie:**

- Sieci przemysłowe i rozproszone systemy sterowania

### 3. Gwiazda (Star)

**Opis:** Wszystkie urządzenia są połączone z centralnym punktem (np. przełącznikiem lub hubem).

**Zalety:**

- Łatwa diagnostyka i konserwacja
- Awaria pojedynczego urządzenia nie wpływa na działanie całej sieci

**Wady:**

- Awaria centralnego punktu powoduje unieruchomienie całej sieci
- Większe zużycie kabli

**Zastosowanie:**

- Sieci domowe i biurowe
- Większość nowoczesnych sieci LAN

---

## Topologie logiczne

### 1. Punkt-punkt (Point-to-Point)

**Opis:** Połączenie bezpośrednie między dwoma urządzeniami, bez pośredników.

**Zastosowanie:**

- Połączenia modemowe, łącza światłowodowe między dwoma serwerami

### 2. Przekazywanie żetonu (Token Passing)

**Opis:** Urządzenia przekazują sobie specjalny „żeton”, który umożliwia transmisję danych.

**Zastosowanie:**

- Sieci Token Ring, FDDI

### 3. Wielodostępowa (Broadcast)

**Opis:** Węzły sieci wysyłają dane do wszystkich innych urządzeń w sieci, a odbiorca decyduje, czy dana informacja jest dla niego.

**Zastosowanie:**

- Sieci Ethernet, Wi-Fi



