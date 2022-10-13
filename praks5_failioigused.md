**1.  Missuguseid õigusi (r,w,x) on Unixis omanikul minimaalselt vaja (d - directory, f - fail)**
          a) kataloogile /d faili /d/f lugemiseks ning - vaja (r,x)
          b) failile /d/f faili /d/f lugemiseks - (r,x)
          c) kataloogile /d faili /d/f kustutamiseks - (w,x)
          d) failile /d/f faili /d/f kustutamiseks? - (x)

**2. Miks chmod a=x skriptifailei ole piisav õigus shelli skriptifaili käivitamiseks? Millist õigust lisaks käivitamis-õigusele veel vaja läheb shelli skripti käivitamiseks? Põhjendage lühidalt?**
    - chmod a = x esmalt loeb skripti sisu ning alles, siis käivitab selle, näiteks chmod 755 aind kirjutab. käsus "a" on justkui lühend "all", "x" nagu "execute".

**3. Milleks on kasulik see, et igal kasutajal on omanimeline grupp? (teema: umask lõpp)**
    -  Unmaski default tehakse 644 õigustega faile (owner read/write, group read-only, other read-only). See on selleks, et iga kasutaja ei saaks teiste privaatseid faile.
    
**4. Milliseid on minimaalsed õigused (rwx), mis on vajalikud teie tavakasutajal (kuulub gruppi majasisene) (mitte root või peeter kasutajal, kausta ja faili omanikud) uusfail.txt sisu kuvamiseks. Esita ekraanivaade id, ls -la ja cat uusfail.txt käskude väljundist tõestamaks lahendust.**
    - r– 
5. Tehke screenshot tulemusest, kus oleks näha hinded.txt failiõigused ls -la hinded.txt ja jukuisa käivituskäsk koos väljundiga ning lisage see oma viki lehele. (teema: setuid ja setgid.)
     -
 
**6. Kas setuid või setgid kasutamine võib vähendada süsteemi turvalisust? Kui JAH, siis kuidas? kui EI, siis miks ei vähenda?**
     - Jah, sest kasutaja saab siiski õigusi, kuid mitte päris root õigusi.

**7. Kirjutage oma viki lehele kõik kasutajaid, kes saavad sticky bit õigustega yhiskaust kataloogist nüüd peeter kasutaja loodud faile kustutada. (teema: sticky bit)**

8. Uurige käsuga ls -la faili hinded.txt õigusi - mida märkate? Seejärel uurige õigusi täpsemalt, kasutades käsku getfacl ning kopeerige see tulemus oma vikilehele. (teema: ACL)

10.Kes saab chattr +i parameetriga faili sisu modifitseerida (kirjutada)? Milliste käskudega saate kustutada testfail-2 nimelise +i parameetriga faili.
  - Ainult root õigustega saab antud commandi panna. Kõik, aga write on keelatud.
