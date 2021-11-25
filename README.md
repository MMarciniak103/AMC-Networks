# Metody analizy społeczności w mediach społecznych

## 1. (5 pkt) Budowa sieci społecznych
Dla wybranego z hashtagów w posiadanym zbiorze danych, używając dowolnego, wybranego narzędzia do budowy sieci (np. networkX, igraph, graph-tool - benchmark [tutaj](https://www.timlrx.com/blog/benchmark-of-popular-graph-network-packages)).

a) **(2 pkt)** zbuduj sieć łączącą użytkowników:
* jako węzły sieci przyjmij poszczególnych użytkowników, 
* niech krawędzie symbolizują wybrane relacje między użytkownikami. 

W zależności od posiadanych danych może być to np. relacja wspólnej dyskusji w obrębie jednej konwersacji, relacja wspominania się w swoich wzmiankach, relacja polubienia swoich wpisów itp. W przypadku zbioru o niskiej jakości, możesz użyć kombinacji różnych relacji

b) **(1 pkt)** zaraportuj podstawową charakterystykę uzyskanej sieci:
* ilość węzłów,
* ilość krawędzi,
* histogram stopnia węzłów.

c) **(2 pkt)** zwizualizuj tak otrzymaną sieć w formie graficznej. Możesz użyć podzbioru użytkowników w celu zapewnienia czytelności prezentacji (np. najpopularniejszych).

## 2. (4 pkt) Detekcja społeczności
Odkryj społeczności występujące w stworzonych sieciach, np. implementując samodzielnie lub używając jednej z zaimplementowanych w użytej bibliotece metod ([więcej informacji o metodach](https://memgraph.com/blog/community_detection-algorithms_with_python_networkx)).

Zaraportuj podstawowe charakterystyki stworzonych społeczności (ilość węzłów i krawędzi)

## 3. (1 pkt) Budowa grupowania użytkowników wg. tematyki wypowiedzi
Używając wyników modelowania tematycznego z poprzednich zajęć, pogrupuj użytkowników - przyjmij, że osoby udzielające się w obrębie jednego tematu należą do jednej grupy. Grupy mogą się nakładać. 

## 4. (4 pkt) Analiza porównawcza wykrytych społeczności
Sprawdź, na ile grupowanie stworzone w pkt 2 nakłada się z grupowaniem stworzonym w pkt 3. 

a) **(2 pkt)** dokonaj porównania zbiorów użytkowników każdy-z-każdym. Możesz użyć dowolnej miary porównania zbiorów, np. [miary Jaccarda](https://pl.wikipedia.org/wiki/Indeks_Jaccarda)

b) **(1 pkt)** przeanalizuj, jak wygląda struktura tematów poruszanych w obrębie grup społecznych - czy istnieje jakiś dominujący temat, czy jest to raczej losowy podział?

c) **(1 pkt)** oceń, jak wygląda struktura sieci społecznych poruszających dane tematy - czy któryś z tematów został zawłaszczony przez którąś z grup społecznych, czy jest to raczej rozkład równomierny?

Spróbuj zagłębić się w analizy i porównania, badając użytkowników i ich wpisy, by zweryfikować poprawność grupowań.

## 5. (6 pkt) Badanie podobieństwa społeczności
Używając dostępnych danych o społecznościach (np. rozkład tematów, charaterystyki sieciowe) zaproponuj miarę porównania dwóch społeczności. Wskaż najbardziej i najmniej podobne grupy. Uzasadnij swoją propozycję miary.

## Zadanie dodatkowe 
### (dodatkowe 5 pkt) Uwzględnienie wydźwięku w grupowaniu
Użyj danych o wydźwięku wpisów, by rozszerzyć grupowanie z pkt 3 o dodatkowy wymiar - zbuduj grupy tematyczne bazując nie tylko na wspólnym poruszaniu danego tematu, ale też podobnym sentymencie tekstów. Zweryfikuj, jak zmieniła się sytuacja w zakresie zadań 4 (i 5 jeśli jest to zasadne).
