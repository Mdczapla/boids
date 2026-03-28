# Boids Simulation: Predator vs. Prey Logic 🐦🚀

Symulacja sztucznego życia (Artificial Life) zrealizowana w **Unreal Engine 5**. Projekt implementuje klasyczny algorytm **Boids**, rozszerzony o dynamiczne interakcje między dwoma gatunkami: ofiarami (Victims) oraz drapieżnikami (Predators).

## 🧠 O projekcie: Algorytm Boids
Symulacja opiera się na trzech fundamentalnych zasadach ruchu stadnego:
1. **Separacja (Separation):** Unikanie kolizji z sąsiadami.
2. **Spójność (Cohesion):** Poruszanie się w stronę środka masy lokalnej grupy.
3. **Wyrównanie (Alignment):** Dostosowanie kierunku i prędkości do reszty stada.

Dodatkowo, system został wzbogacony o **logikę unikania zagrożeń** (dla ofiar) oraz **logikę pogoni** (dla drapieżników), co tworzy złożony i nieprzewidywalny ekosystem.

## 🚀 Kluczowe cechy
* **Dynamiczny Spawner:** Blueprint na mapie startowej automatycznie generuje populację kwadratów o zdefiniowanej liczebności.
* **Wizualna Identyfikacja:**
    * 🟩 **Zielone kwadraty (Victims):** Realizują klasyczny flocking oraz ucieczkę przed zagrożeniem.
    * 🟧 **Pomarańczowe kwadraty (Predators):** Aktywnie wyszukują i ścigają najbliższe cele.
* **Pełna Skalowalność:** Możliwość testowania wydajności silnika i algorytmu przy dużej liczbie agentów jednocześnie.

## ⚙️ Parametry Symulacji
Z poziomu panelu *Details* w edytorze użytkownik może dowolnie konfigurować parametry początkowe:
* **Num Of Predators:** Liczba drapieżników wprowadzonych do systemu.
* **Num Of Victims:** Liczba ofiar tworzących stada.

## 🛠 Technologie
* **Silnik:** Unreal Engine 5
* **Logika:** UE5 Blueprints / Vector Math (implementacja wektorów sił i kierunków).

## 💻 Jak uruchomić
1. Sklonuj repozytorium.
2. Otwórz projekt w **Unreal Engine 5**.
3. Załaduj mapę o nazwie **StartingMap**.
4. Wybierz Actora Spawnera na scenie, ustaw preferowaną liczbę jednostek w panelu *Details* i naciśnij **Play**.
