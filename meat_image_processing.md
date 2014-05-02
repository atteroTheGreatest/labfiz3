##Obróbka graficzna i analiza obrazów skanów mięsa

Wczytaliśmy obrazki do tablic bitów w odcieniach szarości, tzn.
każdy piksel był reprezentowany za pomocą liczb od 0 do 255.

Mając obrazki w takiej postaci mogliśmy oddać je późniejszej obróbce.

Pierwszym krokiem było odpowiednie wykadrowanie i przycięcie, żeby
obrazki pokazywały podobny obszar, w ten sam sposób (rozmiar obrazka, obrót).

Następnie przekształciliśmy obrazki używając progu, tak, że piksele o
wartości niższej dostały kolor czarny,
a piksele powyżej dostały kolor biały.

Taki zabieg nazywany jest thresholdingiem i pomaga w późniejszej analizie.

Kolejnym krokiem było wykrycie krawędzi wokół zamkniętych powierzchni.
Te powierzchnie przypominają konkretne elementy strukturalne mięsa.

Stwierdziliśmy, że oprócz czysto wizualnego określania tekstury może przydać
się bardziej numeryczny sposób do określenia "poszatkowania" i rozerwania
struktur w mięsie.

Przykład takiej analizy na obrazie niezgnieconego mięsa:
![1](http://imgur.com/5dxHggA.png)


Mięso po obróbce wysokim ciśnieniem:

![2](http://imgur.com/2fTzgtI.png)

Dodatkowo obliczyliśmy ilości wykrytych konturów i ich długości.
Mając długości konturów dalej przeanalizowaliśmy ich:

- średnie
- mediany
- wariancję
- rozkłady na histogramie

Więcej informacji i danych jest w notebooku.

