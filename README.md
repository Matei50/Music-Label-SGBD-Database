# Proiect SGBD – Oracle 19c
## Sistem de gestiune pentru industria muzicală
---
Varianta in engleza: (README.en.md) [README.en.md] 

## Descriere generală
Proiectul implementează o bază de date relațională destinată gestionării activităților din industria muzicală: artiști, albume, piese, genuri muzicale, vânzări, manageri și distribuitori.

Soluția include modelarea conceptuală și logică a bazei de date, implementarea structurii în Oracle Database 19c și dezvoltarea componentelor avansate PL/SQL.

## Modelarea bazei de date
Proiectul conține:
- Diagramă conceptuală
- Diagramă Entitate–Relație
- Scripturi SQL pentru:
  - Crearea tabelelor
  - Definirea constrângerilor (chei primare, chei externe, constrângeri de integritate)
  - Inserarea datelor de test

## Funcționalități implementate

### Proceduri și funcții
- Procedură pentru generarea unui raport lunar al unui artist (utilizare colecții: VARRAY, Nested Table, Associative Array)
- Procedură bazată pe cursoare (implicit și parametrizat)
- Funcție pentru calcularea valorii unei vânzări cu tratarea excepțiilor predefinite:
  - NO_DATA_FOUND
  - TOO_MANY_ROWS
  - OTHERS
- Procedură complexă cu excepții definite de utilizator

### Colecții PL/SQL utilizate
- VARRAY
- Nested Table
- Associative Array (INDEX BY)

### Cursoare
- Cursor implicit (instrucțiune FOR cu SELECT)
- Cursor explicit parametrizat

### Triggeri
- Trigger LMD pentru interzicerea operațiilor DELETE în weekend
- Trigger compus pentru contorizarea rândurilor afectate și calculul valorii totale șterse
- Trigger LDD pentru restricționarea operației DROP TABLE la nivel de schemă

## Tehnologii utilizate
- Oracle Database 19c
- PL/SQL
- SQL Developer

## Structura proiectului
/sql – scripturi SQL și PL/SQL  
/diagrams – diagramele bazei de date  
/doc – documentația proiectului  

## Scop
Proiect realizat în cadrul disciplinei Sisteme de Gestiune a Bazelor de Date.

## Autor
Ardeleanu-Chirica Matei
