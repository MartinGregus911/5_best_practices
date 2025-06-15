# Vyhodnotenie osvedčených praktík – Task 5

Každý bod obsahuje :
- [✔ / ✖] či ide o osvedčenú prax
- riziká alebo dôsledky
- odporúčané riešenie

---

1. **Pouzívanie hardoced hodnôt v ETL procesoch pre biznis pravidlá**
✖ NIE je best practice
➡ Riziko: zlá údržba, ťažká škálovatelnosť
✅ Riešenie: parametrizovať vstupy, použiť config súbory, prípadne metadáta

2. **Neindexovanie stľpcov, ktoré sú často dotazované vo veľkých tabuľkách**
✖ NIE je best practice
➡ Riziko: pomaly bežiace dotazy, zbytočné full scan-y
✅ Riešenie: pridať indexy na frekventované stĺpce

3. **Ukladanie logov a záloh na rovnaký server ako produkčná databáza**
✖ NIE je best practice 
➡ Riziko: výpadky, strata dát pri problémoch na serveri
✅ Riešenie: použíť separátne úložisko alebo dedikovaný server

4. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: nezistitelnosť, kto čo urobil (žiadne audity)
✅ Riešenie: individuálne účty, audit trail

5. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: strata dát pri chybe
✅ Riešenie: retry logika, error handling, checkpointy

6. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: únik údajov, neúmyselné prepísanie dát
✅ Riešenie: role-based access control

7. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: Zlá kvalita dát, zlyhanie ETL
✅ Riešenie: schémová validácie pri importe, typová kontrola

8. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice	
➡ Riziko: nízky výkon, zastaralé logiky
✅ Riešenie: pravidelné refactoringy, revízie

9. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: zmätok, vyššie náklady na ukladanie
✅ Riešenie: archivačná politika, označovanie verzií

10. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: tiché zlyhanie bez vedomia tímu
✅ Riešenie: alerting cez email, slack, monitoring

11. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: GDPR pokuty, únik údajov
✅ Riešenie: šifrovanie at rest a in transit (napr. AES, TLS)

12. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: nevalidné alebo nesprávne uložené údaje
✅ Riešenie: explicitné definovanie typov

13. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: deadlocky, cyklické spúšťania
✅ Riešenie: DAG (acyklický graf), kontrola závislotí

14. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: výpadký, spomalenie systému
✅ Riešenie: použiť staging (medzivrstvy)

15. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: prílišná zložitosť alebo slabá výkonnosť
✅ Riešenie: zvoliť model podľa prípadu použitia

16. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: neefektívne ukladanine, ťažšie indexovanie
✅ Riešenie: zvoliť primeraný max. počet znakov

17. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: nízka kvalita dát, prebytočné stĺpce
✅ Riešenie: vybrať len relevantné stĺpce

18. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: pomaly bežiace dotazy
✅ Riešenie: particionovanie podľa dátumu / dimenzií

19. **Používanie zdieľaných servisných účtov na pripojenie k databázam v ETL nástrojoch**
✖ NIE je best practice
➡ Riziko: zlyhania, nemožnosť rollbacku
✅ Riešenie: používať version control (napr. git), CI/CD
