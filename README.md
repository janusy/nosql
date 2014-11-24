# NoSQL

#Zadanie 1

##a)Import danych z pliku CSV 
Polecenie:
```
cat Train.csv | tr "\n" " " | tr "\r" "\n" | head -n 6034196 > correct_train.csv

mongoimport -d train -c train -type csv -file correct_train.csv --headerline
```
##b)Ilość zaimportowanych rekordów:
```
imported 6034195 objects
```
