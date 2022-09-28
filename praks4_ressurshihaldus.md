| Küsimus  | Linux  |  Windows | Linuxis kasutatud käsklus  | 	Windowsis kasutatud tööriist | 
|---|---|---|---|---|---|---|
| Mitu protsessi kokku arvutis käib?  |207  |128|  ps -e wc -l | Task Manager|
| Milline on kõige esimesena käivitatud protsess?  |root 1  0  0 21:56 ? 00:00:01 /sbin/init splash | Süsteemi jõudeoleku protsess|   |  ps -ef grep init |Task Manager|
| Mitu ja milliste kasutajate protsesse arvutis käib?  |Ron, root, Systemd -r, -t,-o, syslog, rtkit, kernoops, lp, avahi|Local Service 22, DWB-1 1, Network service 8, ülejäänud System ja minu user|   |htop  |   |   |   |   |   |   |   |   |   |
| Kui kaua on arvuti järjest töötanud (up time) ? (Alternatiivselt võib vastata ka millal (kuupäev ja kellaaeg) arvuti viimati käima pandi?)?  | 23:52:34 up 24 min,  1 user,  load average: 1,25, 0,68, 0,69  |35 minutit|uptime |   |   |   |   |   |   |   |   |   |   |
| Milline protsess käivitati kõige hiljem (viimasena)? | ron         2784  0.0  0.1  22460  5444 pts/0    Ss   22:32   0:00 bash
ron         2798  0.0  0.1  24124  3964 pts/0    R+   22:36   0:00 ps -aux(viimased 2 igaks juhuks)|svchost.exe |ps -aux |   |   |   |   |   |   |   |   |   |   |
| Milline on kõige rohkem protsessoriaega võttev protsess?  |   1309 ron       20   0 4565696 391424 138056 S  14,6  13,1   **1:05.73** gnome-s+|Microsoft edge|top|   |   |   |   |   |   |   |   |   |   |
| Milline on kõige rohkem virtuaalmälu (aadressiruumi, commit, Virtual Size) võttev protsess?  |1309 ron 20 0 **4569004** 394804 141468 S 9,6  13,3   1:22.13 gnome-s+|227676kb, image|top|   |   |   |   |   |   |   |   |   |   |
| Milline on kõige rohkem füüsilist mälu (working set) võttev protsess?  |1309 ron 20 0 4569004 394804 141468 S 9,6 **13,3** 1:22.13 gnome-s+|SearchHost.exe,188244KB |Top|Resource Manager|   |   |   |   |   |   |   |   |   |
| Kui palju füüsilisest mälust (Physical Memory) on vaba?  |2978608 kB|1851MB|Teenuse host: Win update   |grep MemTotal /proc/meminfo|   |   |   |   |   |   |   |   |   |
| Kui palju on põhikettal (C:, /) vaba ruumi mahult (GB) ja protsentuaalselt?|total used free shared buff/cache available Mem:2,8Gi 812Mi 778Mi 45Mi 1,3Gi **1,8Gi**, 64,3%|41524MB, 64.1% |free -g -h -t|   |   |   |   |   |   |   |   |   |   |
| Milline on kõige suurem kõvakettal olev fail ja kõige suurem kaust?  |1612M	/usr/lib/x86_64-linux-gnu ja kõige suurem kaust /usr   |   |sudo du -aBm / 2>/dev/null  sort -nr  head -n 10|   |   |   |   |   |   |   |   |   |   |
|  Võrrelge terminali käskude: sha1sum /dev/zero | sha1sum /dev/zero ja sha1sum /dev/urandom | sha1sum /dev/urandom protsessori nõudlust. Avage teine terminaliaken ja top samaaegseks käivitamiseks. Uurige millisele CPU alamtegevusele us, sy, id, wa, st jne kulub enim protsessori aega ja mitu protsenti kulub kummagi käsu korral?  |   |   |   |   |   |   |   |   |   |   |   |   |   |
| Milline protsess kõige rohkem salvestusseadmele kirjutab, kõige rohkem salvestusseadmelt loeb? Millisesse faili antud protsess kõige rohkem kirjutab, millisest failist kõige rohkem loeb? (Ainult Windowsis)  |   |   |   |   |   |   |   |   |   |   |   |   |   |
| Millise protsessi poolt tekitatud võrguliiklus on suurima mahuga? Vali antud protsessi poolt kasutatavatest ühendustest üks ning kirjuta välja järgnev: kohalik IP-aadress, kohalik port, ühenduse teise poole IP-aadress, port, latents ja antud ühenduse poolt kasutatav võrguliikluse kogumaht.  |   |   |   |   |   |   |   |   |   |   |   |   |   |
| Sõber kurdab, et tema arvuti on oluliselt aeglasem kui varasemalt. Millise programmiga ja millise parameetrite abil saate tuvastada milline protsess või teenus muudab arvuti aeglaseks?  |   |   |   |   |   |   |   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |   |   |   |   |   |   |   |




| Küsimus|Linux|Windows|Linuxis kasutatud käsklus|Windowsis kasutatud tööriist|
|---|---|---|---|---|
|Mitu protsessi kokku arvutis käib?|207|128|ps -e wc -l|Task Manager|
|Milline on kõige esimesena käivitatud protsess?|root 1  0  0 21:56 ? 00:00:01 /sbin/init splash|Süsteemi jõudeoleku protsess|ps -ef grep init|Task Manager|
|Mitu ja milliste kasutajate protsesse arvutis käib?|Ron, root, Systemd -r, -t,-o, syslog, rtkit, kernoops, lp, avahi|Local Service 22, DWB-1 1, Network service 8, ülejäänud System ja minu user|Htop|Task Manager|
|Kui kaua on arvuti järjest töötanud (up time)?|23:52:34 up 24 min,  1 user,  load average: 1,25, 0,68, 0,69|35 minutit|uptime|Task Manager|
|Milline protsess käivitati kõige hiljem (viimasena)?| ron 2784 0.0 0.1 22460 5444 pts/0 Ss 22:32 0:00 bash ron 2798 0.0 0.1 24124 3964 pts/0 R+ 22:36 0:00 ps -aux(viimased 2 igaks juhuks)|svchost.exe|ps -aux|Task Manager|
|Milline on kõige rohkem protsessoriaega võttev protsess?|1309 ron 20 0 4565696 391424 138056 S  14,6  13,1 **1:05.73** gnome-s+|Microsoft edge|Top|Task Manager|
|Milline on kõige rohkem virtuaalmälu (aadressiruumi, commit, Virtual Size) võttev protsess?|1309 ron 20 0 **4569004** 394804 141468 S 9,6  13,3   1:22.13 gnome-s|227676kb, image|top|Task Manager|
|Milline on kõige rohkem füüsilist mälu (working set) võttev protsess?|1309 ron 20 0 4569004 394804 141468 S 9,6 **13,3** 1:22.13 gnome-s+|SearchHost.exe,188244KB|Top|Resource Manager|
|Kui palju füüsilisest mälust (Physical Memory) on vaba?|2978608 kB|1851MB|Teenuse host: Win update|grep MemTotal /proc/meminfo| Resource Manager
|Kui palju on põhikettal (C:, /) vaba ruumi mahult (GB) ja protsentuaalselt?|otal used free shared buff/cache available Mem:2,8Gi 812Mi 778Mi 45Mi 1,3Gi **1,8Gi**, 64,3%|41524MB, 64.1%|free -g -h -t|Resource Manager|
|Milline on kõige suurem kõvakettal olev fail ja kõige suurem kaust?  |1612M	/usr/lib/x86_64-linux-gnu ja kõige suurem kaust /usr|1612M	/usr/lib/x86_64-linux-gnu ja kõige suurem kaust /usr||sudo du -aBm / 2>/dev/null  sort -nr  head -n 10|   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
