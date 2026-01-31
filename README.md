# Pac-Man 🎮
https://github.com/MSZM0/Pacman
## Opis Projektu

Pac-Man to klasyczna gra zręcznościowa zbudowana w Javie z wykorzystaniem biblioteki Swing. Gra łączy elementy strategii i refleksu, gdzie gracz musi zbierać punkty na mapie, unikając duchów, które go ścigają.

### Główne Cechy:
- 🎯 Zbieranie punktów i power-upów
- 👻 Cztery duchy z różnymi strategiami AI
- ⭐ System trzech żyć
- 🚀 Tryb pauzy oraz menu główne
- 🎨 Animacje i grafika w stylu retro
- 📊 System punktacji i scoreboard


## Instalacja i Uruchomienie

### 1. Klonowanie Repozytorium
```bash
git clone https://github.com/MSZM0/Pacman.git
cd Pacman
```

### 2. Kompilacja Projektu
Otwórz terminal/wiersz poleceń w katalogu projektu i wykonaj:

```bash
javac -cp src src/com/company/*.java
```

### 3. Uruchomienie Gry
```bash
java -cp src com.company.Main
```

Gra powinna się uruchomić w nowym oknie.

## Instrukcje Gry

### Sterowanie
- **W** - Ruch w górę
- **A** - Ruch w lewo
- **S** - Ruch w dół
- **D** - Ruch w prawo
- **SPACJA** - Pauza/Wznowienie gry

### Cel Gry
1. Zbierz wszystkie punkty (małe okręgi) na mapie
2. Unikaj czterech duchów 
3. Zbierz wzmocnienie aby tymczasowo móc jeść duchy i uzyskać dodatkowe punkty

### Zasady
- **Zbieranie Punktów**: Każda mała kropka = 10 punktów
- **Wzmocnienie (Power-up)**: Każde wzmocnienie = 50 punktów + możliwość jedzenia duchów
- **Jedzenie Ducha**: 200+ punktów (wartość wzrasta z każdym zjedzonym duchem +200)
- **Kolizja z Duchem**: Utrata jednego życia (masz 3 życia)
- **Koniec Gry**: Następuje po utracie wszystkich żyć lub zebraniu wszystkich punktów

## Charakterystyka Duchów

| Duch    | Kolor        | Zachowanie |
|---------|--------------|------------|
| Blinky  | Czerwony     | Zawsze bezpośrednio ściga Pac-Mana, ustawiając cel na jego aktualnej pozycji (najbardziej agresywny duch). |
| Pinky   | Różowy       | Przewiduje ruch Pac-Mana – celuje w pole oddalone o 2 kratki w kierunku aktualnego ruchu Pac-Mana. |
| Inky    | Niebieski    | Duch taktyczny – wyznacza punkt 2 kratki przed Pac-Manem, a następnie tworzy wektor od Blinky’ego do tego punktu i podwaja go, próbując flankować gracza. |
| Clyde   | Pomarańczowy | Zachowuje się nieprzewidywalnie – ściga Pac-Mana tylko gdy jest dalej niż 8 pól, w przeciwnym razie ucieka do swojego rogu planszy. |

## Autorzy:

Bartosz Hesse

Marcin Słowikowski
