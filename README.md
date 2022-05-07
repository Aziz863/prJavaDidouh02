# Pt3 Treballant amb branques de Git

## Instruccions utilitzades

#### Apartat 1

Aquesta ordre crea una branca amb el  nom seleccionat i fa el canvi a la branca per començar a treballar ràpidament.

```java
git checkout -b Branca00
```

Una alternativa sería crear la branca i després fer el canvi amb dos comandes:

```java
git branch Branca00
git checkout Branca00
```

#### Apartat 5

Com a alternativa que hem mencionat abans, `git checkout` i el nom de la branca ens permet canviar a la rama esmentada. En aquest cas:

```java
git checkout master
```

Per veure el historial de una branca concreta executem:

```java
git log
```
#### Apartat 10

La primera comanda per canviar a la branca master:

```java
git checkout merge
```

La segona comanda ens permet  fusionar el canvis de la branca seleccionada amb la branca actual:

```java
git merge Branca00
```

#### Apartat 14

Per pujar una branca del nostre repositori local a un repositori remot l'hem d'associar a una branca del repositori remot en el primer push que fem:

```java
git push --set-upstream origin Branca01
```

A partir del segon push ja no es necessari fer aquesta associació i es suficient amb la següent comanda:

```java
git push
```

## Respostes

#### Apartat 6

Des de vscode, actualitza el contingut del fitxer prjavaCognom02.java. Pots veure l'última línia afegida?. Per què?

- No està la nova línea, ja que els canvis estan només a la branca00 i per tenir-los a master hem de fusionar-les.

#### Apartat 7

Torna a la branca branca00. Des de vscode, actualitza el contingut del fitxer PrjavaCognom02.java. Pots veure l'última línia afegida?. Per què?

- Es pot veure la líne afegida anteriorment, ja que aquesta branca conserva tots els canvis realitzats en ella mateixa.

#### Apartat 12

Fes un push del repositori local al repositori remot. Des de Github, actualitza la pàgina web del projecte, i comprova que els canvis han estat realitzats correctament. Comprova que només s'ha actualitzat la branca master únicament. Per què?.

- Només s’ha actualitzat la branca master al repositori degut a que el push l’hem fet només d’aquesta branca amb els canvis de la branca00 gràcies al merge realitzat.
La branca branca00 la tenim actualitzada al nostre repositori local i hauríem de fer un push per tenir el canvis al repositori remot  igual que master.
