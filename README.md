# AR-Homework-4-Mips-processor
Fakultet elektrotehnike Tuzla - Arhitektura racunara 

## 1 Problem

```
Uz pomoc logisim-a i komponenti koje su koristene na vjezbama
konstruisati jednociklusni datapath sa kontrolom po principu rada MIPS
procesora sa ogranicenim skupom instrukcija. Slijediti upute sa
predavanja. Instrukcije koje procesor treba razumjeti su:
```
Jumps: J, JR, JAL^
Memory Load/Store: LW, SW^
Immediate arithmetic/logic: ADDIU, ANDI, ORI, XORI^
Register arithmetic/logic: ADDU, SUBU, AND, OR, XOR, NOR^
Shifts (constant only): SLL, SRL, SRA

```
Programski brojac (PC) realizovati pomocu registra (komponenta "Regis-
ter"). Inkrementiranje PC-a realizovati pomocu komponente "Incrementer".
Nova adresa instrukcije (PC) za jump tipove instrukcija se treba formirati u
bloku NextPC. Uocite da se u ovoj zadaci ne zahtijevaju branch instrukcije,
ali to moze biti dodatni zadatak za vjezbu te je prilozen fajl za testiranje i te
```
verzije procesora. Za pristup memoriji^ koristiti komponentu "RAM".^
Detaljne specifikacije komponenti pogledati na sljedecem linku. Operacije
koje ALU moze izvrsavati i odgovarajuci ALU op kodovi koje treba koristiti
su dati u sljedecoj tabeli:

Table 1: ALUop kodovi za koristenu ALU komponentu^

```
op^ C operation^ name^
0000 C = B << sa shift left logical
0010 C = A + B add
0100 C = B >> sa shift right logical
0101 C = B >>> sa shift right arithmetic
0110 C = A B subtract
1000 C = A & B and
1010 C = A j B or
1100 C = A ^ B xor
1110 C = ~(A j B) nor
```
```
Za testiranje funkcionalnosti moze se koristiti program projekat.s, a za te-
stiranje sa branch instrukcijama moze se koristiti program projekat branch.s.
```
