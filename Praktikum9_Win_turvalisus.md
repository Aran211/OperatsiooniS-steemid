1. Võrrelge Administrator ja SYSTEM privileege ning kirjutage vähemalt üks tegevus mille jaoks on vaja SYSTEM õigusi.
  - Näiteks on viimasel real: "SeDelegateSessionUserImpersonatePrivilege Obtain an impersonation token for another user in the same session Enabled", kuid tavalises adminstraatori aknas on antud väärtus DISABLED
  Avanenud aknas on palju rohkem näha Enabled väärtusi, võrreldes tavalise admistraatori cmd whoami /priv käsu väljudil. Näiteks on Sys õigusi vaja "SetTimeZonePrivilege" muutmisel.
  
2.Ekraanivaade turvalise kausta seadetest (ainult üks kasutaja saab teha kõike ja Ülemus ainult lugeda)
  -![image](https://user-images.githubusercontent.com/112877689/200669815-b0b237d6-94c0-46c6-8a0e-e8beee59b9b1.png)
  Vaade ülemuse õigustest
  - ![image](https://user-images.githubusercontent.com/112877689/200669937-8a8ca8ef-727a-44f5-8d99-bf46fd68eb4c.png)
  vaade Teise tavakasutaja õigustest(Selle nimega on ka kaust).
  
  
Kirjuta praktikumi aruandesse vähemalt 3 soovitust (muudatust), mida Microsoft soovitab Windowsi turve seadete juures parandada, suurendamaks Windows operatsioonisüsteemi turvalisust.
  - Kindlasti tuleks muuta reklaami-ID seadet, asukoht keelata ning vaadata, kellel on ligipääs kontaktidele.

Sobiv kasutajakonto kontrolli seadistus koos põhjendusega (Süsteem ja turve)
  - Valiksin vaikeseade, sest soovin teada kui rakendused proovivad tehea muudatusi või installida mingit tarkvara ning hea ise kursis olla toimuvaga.

Vali veel vähemalt 3 Local Security Policy seadistust, mida tuleks muuta või üle vaadata, et tagada arvutis olevate andmete ja kasutajate isikuandmete kaitse. Põhjenda oma valikuid. Ekspordi Local Security Policy tööriistast iga seadistuste kategooria kohta *.txt fail ning kopeeri AINULT asjassepuutuvate muudetud
  -Minimum password length	5 characters : parool võiks olla vähemalt 5 tähemärki või tähte.
  Minimum password length audit	30 characters - Võiks olla max 30 tähemärki, kuna rohkem on väga suur tõenäosus, et kasutaja unustab parooli või on see üles kirjutatud kuhugi ning see vähendab ka turvalisust
Maximum password age	90 days - kui  seadmes on olulisi või tähtsaid andmeid võiks parooli muuta vähemalt 3 kuu tagant
  

Minimaalselt 2 ekraanivaadet testimise käigus esinenud keeluteavitustest, koos selgitusega mida ning millise kasutajaga tehti.
![image](https://user-images.githubusercontent.com/112877689/200677947-c8597bd9-6a95-4f16-9109-9897e7a47673.png)
Üritasin installeerida Team Vieweri Läbi admin kasutaja.
![image](https://user-images.githubusercontent.com/112877689/200678839-9ac0048e-e266-4ebb-a96d-59b13a8b55a8.png)
Proovisin sama tavakasutajaga ning panin ka vale parooli.


Ekraanivaade Event Vieweri aknast, kus näha ebaõnnestunud sisselogimiskatsete logikirje
![image](https://user-images.githubusercontent.com/112877689/200679426-2be16750-deb9-426c-8f2b-3a72c23e66b6.png)


Tehke ekraanivaade DisplayLastLogonInfo registrivõtmest koos väärtusega 1.
![image](https://user-images.githubusercontent.com/112877689/200680772-fee963b6-b880-4b79-a0ab-0604dd9c21ce.png)
![image](https://user-images.githubusercontent.com/112877689/200681144-760ae216-1e46-4723-a134-65f07b2e6041.png)

