<div align="center">

  <h1>🌌 QiuX AppCenter</h1>
  <p><b>Oficjalny hub, launcher i centrum zarządzania aplikacjami z ekosystemu QiuX.</b></p>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" width="100%" height="100%">
  <defs>
    <!-- Gradient Liniowy Tła -->
    <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0518"/>
      <stop offset="50%" stop-color="#150a2a"/>
      <stop offset="100%" stop-color="#05020c"/>
    </linearGradient>

    <!-- Główny Gradient Liniowy dla Logo (Sygnatury Q) -->
    <linearGradient id="qiuxPrimaryGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00f2fe"/>
      <stop offset="35%" stop-color="#7000ff"/>
      <stop offset="70%" stop-color="#e010ff"/>
      <stop offset="100%" stop-color="#ff007f"/>
    </linearGradient>

    <!-- Gradient Akcentu / Ogona Litery Q -->
    <linearGradient id="qiuxAccentGradient" x1="0%" y1="100%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00f2fe"/>
      <stop offset="100%" stop-color="#e010ff"/>
    </linearGradient>

    <!-- Efekt Świetlistej Poświaty (Glow) -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="12" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
  </defs>

  <!-- Tło Logo z Zaokrąglonymi Rogami (Sformatowane jak ikona aplikacji) -->
  <rect width="512" height="512" rx="110" fill="url(#bgGradient)"/>
  <rect width="504" height="504" x="4" y="4" rx="106" fill="none" stroke="url(#qiuxPrimaryGradient)" stroke-width="3" stroke-opacity="0.4"/>

  <!-- Tło Świetliste w Centrum -->
  <circle cx="256" cy="236" r="130" fill="url(#qiuxPrimaryGradient)" opacity="0.15" filter="url(#glow)"/>

  <g transform="translate(0, -10)">
    <!-- Główny Pierścień Litery Q -->
    <path d="M 256,106 
             C 170,106 106,170 106,256 
             C 106,342 170,406 256,406 
             C 342,406 406,342 406,256 
             C 406,170 342,106 256,106 Z 
             M 256,166 
             C 308,166 346,204 346,256 
             C 346,308 308,346 256,346 
             C 204,346 166,308 166,256 
             C 166,204 204,166 256,166 Z" 
          fill="url(#qiuxPrimaryGradient)" 
          filter="url(#glow)"/>

    <!-- Ogon Litery Q (Stylizowany na dynamiczne wycięcie / promień) -->
    <path d="M 310,310 
             L 410,410 
             C 425,425 400,440 380,420 
             L 290,330 
             Z" 
          fill="url(#qiuxAccentGradient)" 
          filter="url(#glow)"/>

    <!-- Dodatkowy Akcent Ostrego Rdzenia Wewnątrz -->
    <circle cx="256" cy="256" r="18" fill="url(#qiuxAccentGradient)" opacity="0.9"/>
  </g>
</svg>

  [![Status](https://img.shields.io/badge/Status-Beta_v0.5-orange.svg)](#)
  [![Platforma](https://img.shields.io/badge/Platforma-Windows-blue.svg)](#)
  [![UI Theme](https://img.shields.io/badge/UI-Aesthetic_Dark_Purple-8a2be2.svg)](#)
  [![Licencja](https://img.shields.io/badge/Licencja-Proprietary_QiuX-red.svg)](#)

  <p><i>"One place. Every QiuX app."</i></p>

</div>

---

> [!WARNING]
> **Aplikacja w fazie testów (Wersja v0.5 Beta)**
> Program **QiuX AppCenter** jest obecnie w intensywnej fazie rozwoju (jesteśmy w połowie fazy v0.5)[cite: 1]. Zaraz będziemy wychodzić ze wczesnej wersji[cite: 1]. Niektóre funkcje mogą ulegać zmianom lub działać nieprawidłowo[cite: 1].

---

## 📖 Spis Treści

- [📖 Spis Treści](#-spis-treści)
- [✨ O Projekcie](#-o-projekcie)
- [🚨 Status Deweloperski (v0.5 Beta)](#-status-deweloperski-v05-beta)
- [🖼️ Proces Uruchomienia i Galeria](#️-proces-uruchomienia-i-galeria)
  - [1. Wybór Trybu Użytkownika / Sesji](#1-wybór-trybu-użytkownika--sesji)
  - [2. Wybór Posiadania Licencji](#2-wybór-posiadania-licencji)
  - [3. Wpisywanie i Aktywacja Licencji](#3-wpisywanie-i-aktywacja-licencji)
  - [4. Akceptacja Regulaminu i Warunków (EULA)](#4-akceptacja-regulaminu-i-warunków-eula)
  - [5. Ekran Ładowania (Splash Screen)](#5-ekran-ładowania-splash-screen)
  - [6. Pulpit Główny – Wszystko od QiuX](#6-pulpit-główny--wszystko-od-qiux)
- [🛡️ Dostępne Tryby Korzystania](#️-dostępne-tryby-korzystania)
- [🔑 Licencjonowanie i Aktywacja](#-licencjonowanie-i-aktywacja)
- [📐 Architektura Techniczna](#-architektura-techniczna)
- [⚙️ Wymagania i Instalacja](#️-wymagania-i-instalacja)
- [📜 Licencja i Prawa Autorskie](#-licencja-i-prawa-autorskie)

---

## ✨ O Projekcie

**QiuX AppCenter** to nowatorska aplikacja desktopowa stanowiąca centralny punkt dostępowy do wszystkich programów, gier i narzędzi z ekosystemu QiuX[cite: 2, 6, 9]. 

Zamiast ręcznie szukać instalatorów, **QiuX AppCenter** pozwala przeglądać, pobierać oraz aktualizować aplikacje QiuX z poziomu jednego, spójnego i bezpiecznego interfejsu[cite: 2, 6, 9].

---

## 🚨 Status Deweloperski (v0.5 Beta)

Aplikacja znajduje się obecnie w trakcie przełomowej aktualizacji **v0.5**[cite: 1]:
* Jesteśmy w połowie fazy v0.5 i przygotowujemy się do wyjścia z wczesnej wersji testowej[cite: 1].
* Niektóre moduły sieciowe oraz integracje mogą być poddawane testom obciążeniowym[cite: 1].
* Wszelkie uwagi oraz błędy można zgłaszać bezpośrednio przez sekcję *Issues* na GitHubie.

---

## 🖼️ Proces Uruchomienia i Galeria

### 1. Wybór Trybu Użytkownika / Sesji

Na samym początku użytkownik decyduje, w jakim trybie chce uruchomić aplikację – do wyboru jest Tryb Użytkownika, Tryb Gościa oraz prywatny Tryb Incognito.

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 1: WYBÓR TRYBU UŻYTKOWNIKA -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164414.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/01_wybor_uzytkownika.png" alt="Wybór trybu użytkownika" width="750"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIE 1: Zrzut ekranu 'Jak chcesz korzystać?' - plik 'assets/01_wybor_uzytkownika.png']</b>[cite: 2]
</p>

---

### 2. Wybór Posiadania Licencji

Aplikacja pyta użytkownika, czy posiada już licencję na pełny dostęp do ekosystemu QiuX.

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 2: PYTANIE O LICENCJĘ -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164433.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/02_pytanie_o_licencje.png" alt="Czy chcesz licencję?" width="750"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIE 2: Zrzut ekranu 'Czy chcesz licencję?' - plik 'assets/02_pytanie_o_licencje.png']</b>[cite: 3]
</p>

---

### 3. Wpisywanie i Aktywacja Licencji

Ekran weryfikacji i wpisywania indywidualnego identyfikatora licencji (ID License), np. kodów aktywacyjnych takich jak `QXGIFT2026`[cite: 4, 5].

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 3: WPISYWANIE LICENCJI -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164445.jpg lub 164504.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/03_potwierdzenie_licencji.png" width="48%" alt="Potwierdzenie zakupu licencji"/>
  <img src="assets/03_wpisywanie_licencji.png" width="48%" alt="Podaj ID License"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIA 3: Zrzuty z potwierdzeniem zakupu oraz wpisywaniem kodu 'Podaj ID License' - pliki w 'assets/']</b>[cite: 4, 5]
</p>

---

### 4. Akceptacja Regulaminu i Warunków (EULA)

Przed pierwszym pełnym uruchomieniem wymagane jest zapoznanie się i zaakceptowanie warunków licencji użytkownika końcowego.

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 4: AKCEPTOWANIE REGULAMINU -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164528.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/04_akceptacja_regulaminu.png" alt="Zanim zaczniemy - Licencja użytkownika" width="750"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIE 4: Zrzut ekranu 'Zanim zaczniemy - Licencja użytkownika końcowego' - plik 'assets/04_akceptacja_regulaminu.png']</b>
</p>

---

### 5. Ekran Ładowania (Splash Screen)

Pojawia się podczas inicjalizacji modułów systemowych oraz łączenia z centrum aplikacji QiuX.

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 5: EKRAN ŁADOWANIA -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164554.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/05_ekran_ładowania.png" alt="Ładowanie centrum aplikacji QiuX" width="750"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIE 5: Zrzut ekranu z logo QiuX i paseczkiem ładowania - plik 'assets/05_ekran_ładowania.png']</b>[cite: 8]
</p>

---

### 6. Pulpit Główny – Wszystko od QiuX

Docelowy ekran aplikacji, w którym użytkownik ma dostęp do pełnej biblioteki programów i gier ekosystemu QiuX w jednym miejscu.

<!-- ================================================================= -->
<!-- 📸 ZDJĘCIE 6: PULPIT GŁÓWNY -->
<!-- Wstaw tutaj Zrzut ekranu 2026-10-04 164604.jpg -->
<!-- ================================================================= -->
<p align="center">
  <img src="assets/06_pulpit_glowny.png" alt="Wszystko od QiuX. W jednym miejscu." width="800"/>
  <br>
  <b>📸 [TUTAJ WSTAW ZDJĘCIE 6: Zrzut ekranu 'Wszystko od QiuX. W jednym miejscu.' - plik 'assets/06_pulpit_glowny.png']</b>[cite: 9]
</p>

---

## 🛡️️ Dostępne Tryby Korzystania

1. **Tryb Użytkownika:**
   - Logowanie przez konto Google[cite: 2, 7].
   - Zapisywanie ustawień, zakładek i historii pobierania w chmurze[cite: 2].
2. **Tryb Gościa:**
   - Przeglądanie zasobów bez potrzeby zakładania konta[cite: 2].
   - Pobieranie może być zablokowane do momentu zalogowania[cite: 2].
3. **Tryb Incognito:**
   - Całkowicie prywatna sesja[cite: 2, 9].
   - Wybory i dane tymczasowe są usuwane natychmiast po zamknięciu aplikacji[cite: 2, 9].

---

## 🔑 Licencjonowanie i Aktywacja

Aplikacja zawiera moduł obsługi licencji komercyjnych oraz promocyjnych[cite: 3, 5]:
- Możliwość wpisania indywidualnego identyfikatora **ID License**.
- Obsługa specjalnych kodów aktywacyjnych (np. `QXGIFT2026` aktywujący dożywotni dostęp)[cite: 5].

---

## 📐 Architektura Techniczna

* **Runtime:** Electron.js / Node.js
* **Frontend:** HTML5, CSS3, JavaScript ES6+
* **Style:** Custom Dark Purple Glassmorphism[cite: 1, 6]
* **Autentykacja:** Google OAuth Integration[cite: 2, 7]

---

## ⚙️ Wymagania i Instalacja

### Wymagania
* **OS:** Windows 10 / Windows 11 (64-bit)
* **Node.js:** v18.0.0 lub nowszy (dla budowania ze źródeł)

### Instalacja (Developer Build)

```bash
# 1. Sklonuj repozytorium
git clone [https://github.com/TwojUsername/QiuX-AppCenter.git](https://github.com/TwojUsername/QiuX-AppCenter.git)

# 2. Wejdź do folderu
cd QiuX-AppCenter

# 3. Zainstaluj pakiety
npm install

# 4. Uruchom projekt
npm start<img width="150" height="150" alt="gemini-svg" src="https://github.com/user-attachments/assets/9e0989d7-e3d7-47cf-9cdb-b11bf88a117f" />
