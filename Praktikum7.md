Käesolevas praktikumis uurisin, kuidas lokaaleid ja võrgukettaid kasutada nii Windowsi kui ka Linuxi keskkonnas. 
Kuna ülesannete sooritamisel oli vaja olla TÜ sisevõrgus õppisin paigaldama ja lõpuks ühendasin oma arvuti VPN'iga TÜ sisevõrku.

Ülesanne 7.1.1 - Miks uued andmakandjad vajavad lähtestamist?

Lähtestamine aitab tuvastada ja parandada vigu, mis võivad andmekandjal olla, mis omakorda parandab andmete kvaliteeti. Vormistab andmekandjat ja tagab õige ühilduvuse, et andmekandja töötaks valitud masinaga

Ülesanne 7.1.2 - GPT eelised kasutamiseks võrreldes MBRiga
- GPT toetab suuremaid partitsioonisuurusi, kuni 9,4 zettabaiti (ZB), kui MBR toetab kuni 2,2 TB suurusi.
- GPT  toetab kuni 128 erinevat partitsiooni, võrreldes MBR’iga, mis toetab 3 põhi ja 1 lisa partitsiooni.
- GPT hoiab automaatselt kriitilisest infot liigseid koopiaid kettal peal, muutes vidage taastamise usaldusväärsemaks ja suurendab tervislikkuse kontrolle . Võrreldes MBR, kuna ta on kompaktne, siis tal neid sisseehitatud ei ole, mistõttu MBR kandja rikkumisel andmed kaovad
- GPT kasutab CRC32 kontrollsummasid, et kontrollida andmete terviklikkust ja võimaldada riknemistest taastumist, mis MBR’il puudub.

Ülesanne 7.3 - 
https://kodu.ut.ee/~karlmill/opsys/hdd.png 

Ülesanne 7.4 - käsk "ls -la /mnt/ut/public_html/opsys/"
<img width="956" height="598" alt="Kuvatõmmis 2025-10-31 131130" src="https://github.com/user-attachments/assets/adc41462-b02b-45c1-91c1-72e1fccfa38c" />

Ülesanne 7.5 - käsu 'mount' parameetrid -o ro ja -t auto
- Parameeter '-o ro' ütleb, et ühenduses olevat mälupulka ainult loetakse (read-only)
- Parameeter '-t auto' tuvastab automaatselt, mis failisüsteemi tüübiga on tegu.

Ülesanne 7.6 - ketta automaatne ühendamine arvuti käivitusel
<img width="950" height="590" alt="Kuvatõmmis 2025-11-05 124702" src="https://github.com/user-attachments/assets/55c78cf6-12c1-4489-805c-8bf6a4f603cd" />
