# Informacijski sustav za rezervaciju smještaja

## Kratki opis
Projekt prikazuje modeliranje informacijskog sustava za rezervaciju smještaja s naglaskom na dizajn relacijske baze podataka, ERA model, SQL upite i implementaciju poslovnih pravila pomoću okidača.

## Opis projekta
Ovaj projekt izrađen je kao studentski rad iz područja baza podataka i informacijskih sustava. Cilj projekta bio je osmisliti relacijsku bazu podataka koja podržava osnovne procese rezervacije smještaja, uključujući evidenciju objekata, smještajnih jedinica, gostiju, rezervacija i plaćanja.

Poseban naglasak stavljen je na modeliranje ERA modela, definiranje odnosa među entitetima te implementaciju poslovne logike na razini baze podataka.

## Cilj projekta
Cilj projekta bio je razviti model baze podataka koji omogućuje:
- upravljanje smještajnim objektima i jedinicama
- evidenciju rezervacija i plaćanja
- provjeru dostupnosti smještaja
- automatizaciju ključnih poslovnih pravila

## Korištene tehnologije
- PostgreSQL
- SQL
- DataGrip
- Draw.io

## Model baze podataka
Sustav je modeliran pomoću ERA modela koji uključuje sljedeće glavne entitete:
- korisnik
- gost
- vlasnik
- objekt smještaja
- jedinica smještaja
- rezervacija
- plaćanje
- sadržaj
- kalendar dostupnosti

Model uključuje različite vrste veza (1:N i M:N) te jasno definirane primarne i strane ključeve.

## Ključne funkcionalnosti
- evidencija objekata i smještajnih jedinica
- evidencija rezervacija i plaćanja
- pregled i filtriranje podataka putem SQL upita
- analiza popunjenosti smještaja
- povezivanje podataka kroz relacije između entiteta

## Poslovna pravila (implementirana kroz okidače)
- nije moguće unijeti rezervaciju koja se vremenski preklapa s postojećom
- ukupna cijena rezervacije automatski se izračunava na temelju trajanja boravka i cijene jedinice

## SQL upiti
Projekt uključuje primjere upita za:
- pregled svih objekata smještaja
- ispis jedinica određenog objekta
- pregled rezervacija
- povezivanje više tablica (JOIN)
- izračun broja noćenja i popunjenosti

## Sadržaj repozitorija
Repozitorij sadrži:
- projektnu dokumentaciju (PDF)
- prikaz ERA modela
- primjere SQL upita i okidača
