# Takie tam przypiski
```
%e           - liczba eulera
%pi          - liczba pi
%f / %F      - wartość boolean na False
%t / %T      - wartość boolean na True
%i / 1i / 1j - liczby urojone ( dla 3i = 3* %i
```
# Zadanko PIERWSZE
```
M1=ones(10,10)*8-3*eye(10,10)
inv(M1) - tutaj twoaj macierz robi fiflaka o 180 stopni, inaczej mówiąc jest odwrócona
det(M1) - to Ci liczy wyznacznik z Macierzy
```

# Zadanko DRUGIE
```
v=%e.^[0:99] #wektor w przediale 0 do 99 podniesiony do potęgi e (kropka wymagana, bo inaczej scilab wypierdala fikoła
u=1./(%pi.^[0:99]) #wektor w przediale 0 do 99 podniesiony do potęgi pi (kropka wymagana, bo inaczej scilab wypierdala fikoła
u*v' #ciapek wymagany, bo inaczej nie działa
```
# Zadanko TRZECIE
```
A=[%T %T %F %F]; wpierw przypisujesz tej jebanej gangrenie a i b wartości, tak jakbyś to robił metodą tabelek
B=[%T %F %T %F];
(~(A&B))==(A|B)
A=[%T %T %T %T %F %F %F %F]; wpierw przypisujesz tej jebanej gangrenie a i b wartości, tak jakbyś to robił 
B=[%T %T %F %F %T %T %F %F]; metodą tabelek, tylko tutaj robisz to dla 3 wartości
C=[%T %F %T %F %T %F %T %F];
(~((A==B)|(A==C)))==((~(A==B))&(~(A==C)))
```
# Zadanko CZWARTE
```
M1=ones(10,10)*8-3*eye(10,10)
inv(M1) - tutaj twoaj macierz robi fiflaka o 180 stopni, inaczej mówiąc jest odwrócona
det(M1) - to Ci liczy wyznacznik z Macierzy
```
# Zadanko PIĄTE
```
// Definiowanie zakresu zmiennej x
x = -1:0.1:4; // Zakres od -1 do 4 z krokiem 0.1

// Definiowanie funkcji
y1 = x.^2 + 1; // Funkcja x^2 + 1
y2 = -x + 5;   // Funkcja -x + 5

// Tworzenie wykresu
plot(x, y1, "b", "LineWidth", 2); // Wykres y1 w kolorze niebieskim
hold on; // Utrzymanie poprzedniego wykresu
plot(x, y2, "g", "LineWidth", 2); // Wykres y2 w kolorze zielonym
hold off;

// Dodawanie etykiet i legendy
xlabel("x");
ylabel("y");
title("Wykresy x^2 + 1 oraz -x + 5");
legend(["x^2 + 1", "-x + 5"], "location", "top");
xgrid();
```
