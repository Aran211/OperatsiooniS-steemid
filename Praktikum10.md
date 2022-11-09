**Ülesanne 3**
read -p "Palun sisestage oma nimi: " NIMI

read -p "Palun sisestage oma eriala: " ERIALA

read -p "Palun sisestage oma matrikli number: " MatrNumber

echo "Tere, $NIMI!"

echo "Eriala: $ERIALA"

echo "Matrikli Number: $MatrNumber"


Väljund:
![image](https://user-images.githubusercontent.com/112877689/200844609-6d404243-c5e4-4bc6-8c6d-207df09194c2.png)

**Ülesanne 4**
#!/bin/bash

read -p "Faili A nimetus:" A
#read -p "Faili B nimetus:" B

for A in *.txt; do
    mv "$A" "${A%.txt}.csv"
done

![image](https://user-images.githubusercontent.com/112877689/200851980-6c17568b-7d03-487c-b722-dfdc2526c35e.png)
Enne skripti jooksutamist fail test.txt
![image](https://user-images.githubusercontent.com/112877689/200852134-f1946542-b7fb-4395-8d0e-2058d8fd33d8.png)
Pärast skripti kasutamist, on test.csv

**Ülesanne 5**
#!/bin/bash

echo "Enter PID to search: "
read PID
search=$(ps --pid $PID -o comm=)

if [ $search ]
    then
        echo "Program: $search"
    else
        echo "No program found with PID: $PID"
fi
![image](https://user-images.githubusercontent.com/112877689/200899752-fb906f38-b1c8-4b79-9cf4-0c7c7b833e2c.png)

**Ülesanne 6**

![image](https://user-images.githubusercontent.com/112877689/200909902-460a7874-1299-43b4-ac57-a46150940a74.png)


aste () {
  a=$(($1 ** $2))
  echo  $a
}

a=$(aste 9 5)
b=$(aste $a 1)
echo $b

