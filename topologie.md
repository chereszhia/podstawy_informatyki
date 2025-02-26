# Topologie sieci komputerowych

## 1. Topologie fizyczne
Topologia fizyczna określa, w jaki sposób urządzenia są fizycznie połączone w sieci komputerowej.

### 🔹 Topologia magistrali (Bus)
Wszystkie urządzenia są podłączone do jednej wspólnej magistrali (kabla). Dane przesyłane są w obu kierunkach i odbierane przez wszystkie urządzenia.

**✅ Zalety:**
- Prosta implementacja i niski koszt
- Łatwa rozbudowa

**❌ Wady:**
- Awaria głównej magistrali powoduje zatrzymanie całej sieci
- Ograniczona wydajność, im więcej urządzeń, tym większe przeciążenie

**📌 Zastosowanie:**
- Starsze sieci LAN, sieci edukacyjne

---

### 🔹 Topologia pierścienia (Ring)
Urządzenia są połączone w zamkniętą pętlę, dane przesyłane są w jednym kierunku (lub w obu w przypadku pierścieni dwukierunkowych).

**✅ Zalety:**
- Brak kolizji danych
- Stabilna wydajność przy dużej liczbie urządzeń

**❌ Wady:**
- Awaria jednego urządzenia powoduje przerwanie działania całej sieci
- Trudniejsza diagnostyka i naprawa

**📌 Zastosowanie:**
- Sieci korporacyjne, starsze systemy telekomunikacyjne

---

### 🔹 Topologia gwiazdy (Star)
Każde urządzenie jest podłączone do centralnego punktu (np. switcha lub routera), przez który odbywa się komunikacja.

**✅ Zalety:**
- Awaria jednego urządzenia nie wpływa na całą sieć
- Prosta rozbudowa

**❌ Wady:**
- Awaria centralnego węzła zatrzymuje działanie całej sieci
- Wysokie koszty wdrożenia (potrzebne więcej kabli)

**📌 Zastosowanie:**
- Nowoczesne sieci LAN w biurach i szkołach, sieci domowe

---

## 2. Topologie logiczne
Topologia logiczna określa sposób przesyłania danych między urządzeniami w sieci.

### 🔹 Punkt-punkt (Point-to-Point)
Każde połączenie składa się tylko z dwóch urządzeń, które komunikują się bezpośrednio.

**📌 Zastosowanie:**
- Połączenia między serwerami, komunikacja w technologii Bluetooth

---

### 🔹 Przekazywanie żetonu (Token Passing)
Dane są przekazywane sekwencyjnie w sieci, gdzie specjalny pakiet (żeton) kontroluje prawo do nadawania.

**📌 Zastosowanie:**
- Starsze sieci oparte na technologii Token Ring

---

### 🔹 Wielodostępowa (Multiple Access)
Wiele urządzeń może przesyłać dane w tym samym czasie, stosując mechanizmy kontroli dostępu do medium transmisyjnego.

**📌 Zastosowanie:**
- Sieci Ethernet (CSMA/CD), sieci Wi-Fi (CSMA/CA)
