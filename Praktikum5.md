Käesolevas praktikumis uurisin ja katsetasin failiõiguseid Linuxis. Kasutasin praktikumitöö sooritamiseks Ubuntu Linux virtuaalmasinat. 
Praktikumitööd tehes vastasin kontrollküsimustele.

Ülesanne 5.1

1) Minimaalne õigus, kataloogile et minufail.txt’d lugeda on “x” - execute, et kataloogi siseneda ja failile ligi pääseda. 
   Minimaalne õigus failile on “r” - read, et faili lugeda.
2) Minimaalne kataloogile et minufail.txt’d kustutada on “x” - execute, et kataloogi siseneda ja failile ligi pääseda.
   Failile pole õiguseid vaja, sest kustutamiseks pole vaja faili minna, protsess toimub kataloogis.

Ülesanne 5.2

“chmod a=x skriptifail” ei ole piisav, kuna Shelli skriptifaild on tekstifailid, mille täitmiseks on neid vaja rida-realt lugeda. Vaja läheb veel ka lugemisõigust(“r”).

Ülesanne 5.3

Omanimelised grupid hoiavad ära ebavajalike inimeste jms ligipääsu, kes faile võiksid kuritarvitada.

Ülesanne 5.4

Minimaalsed õigused tavakasutajal, kes kuulub gruppi majasisene, on “r” ja "x".
<img width="954" height="598" alt="Kuvatõmmis 2025-10-22 011550" src="https://github.com/user-attachments/assets/fa921c7b-1f26-4f6b-a61b-1d0bb042a2ca" />

Ülesanne 5.5

Pilt fail hinded.txt õigused ja jukuisa käivituskäsk.
<img width="780" height="508" alt="Kuvatõmmis 2025-10-22 021649" src="https://github.com/user-attachments/assets/011ba789-b153-44f2-8718-af9072eea517" />


Ülesanne 5.6

Setuid kasutamine vähendab turvalisust, kuna ta annab tavakasutajale, kel ei peaks olema õigust faili lugeda, omaniku õigused, millega saab ta faili ja õiguseid kuritarvitada.

Ülesanne 5.7

Peeter, opetaja ja root.

Ülesanne 5.8

# file: hinded.txt
# owner: opetaja
# group: opetaja
user:: rw-
group::- - -
other: - - -

<img width="92" height="72" alt="Kuvatõmmis 2025-10-22 233949" src="https://github.com/user-attachments/assets/e2808e10-8ea3-4bf9-b75e-f8b83b168e54" />


Ülesanne 5.9

Faili ei saa muuta mitte keegi, isegi root-kasutaja, sest kuna on lisatud +i (immutable, muutmatu) atribuut.
Ei saa fili kirjutada, kustutada, ümber nimetada ja linkida.
Faili saab kustutada kahes etapis: eemaldada immutability (+1) ja siis saab kustutada faili.
1) sudo chattr -i testfail-2
2) sudo rm testfile-2
3) kustutatud
