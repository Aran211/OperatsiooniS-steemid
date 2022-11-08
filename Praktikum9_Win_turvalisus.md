1. Võrrelge Administrator ja SYSTEM privileege ning kirjutage vähemalt üks tegevus mille jaoks on vaja SYSTEM õigusi.
  - Näiteks on viimasel real: "SeDelegateSessionUserImpersonatePrivilege Obtain an impersonation token for another user in the same session Enabled", kuid tavalises adminstraatori aknas on antud väärtus DISABLED
  Avanenud aknas on palju rohkem näha Enabled väärtusi, võrreldes tavalise admistraatori cmd whoami /priv käsu väljudil. Näiteks on Sys õigusi vaja "SetTimeZonePrivilege" muutmisel.
  
2.Ekraanivaade turvalise kausta seadetest (ainult üks kasutaja saab teha kõike ja Ülemus ainult lugeda)
  -![image](https://user-images.githubusercontent.com/112877689/200669815-b0b237d6-94c0-46c6-8a0e-e8beee59b9b1.png)
  Vaade ülemuse õigustest
  - ![image](https://user-images.githubusercontent.com/112877689/200669937-8a8ca8ef-727a-44f5-8d99-bf46fd68eb4c.png)
  vaade Teise tavakasutaja õigustest(Selle nimega on ka kaust).
 
  
  
  
  
  
  
  
Kirjuta praktikumi aruandesse vähemalt 3 soovitust (muudatust), mida Microsoft soovitab Windowsi turve seadete juures parandada, suurendamaks Windows operatsioonisüsteemi turvalisust.
Sobiv kasutajakonto kontrolli seadistus koos põhjendusega (Süsteem ja turve)
Kirjelda 3 Local Security Policy lisaseadistust turvalisuse tagamiseks, koos põhjendustega.
Minimaalselt 2 ekraanivaadet testimise käigus esinenud keeluteavitustest, koos selgitusega mida ning millise kasutajaga tehti.
Ekraanivaade Event Vieweri aknast, kus näha ebaõnnestunud sisselogimiskatsete logikirje
Tehke ekraanivaade DisplayLastLogonInfo registrivõtmest koos väärtusega 1.
