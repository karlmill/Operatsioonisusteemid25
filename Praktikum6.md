Käesolevas praktikumis uurisin ja katsetasin erinevaid protsesse ja lahedasin praktikumitöö lõpus olevad ülesanded.

Ülesanne 6.1 - gedit ja SIGCONT käsureal
<img width="951" height="594" alt="Kuvatõmmis 2025-10-29 233724" src="https://github.com/user-attachments/assets/5929bb99-5ad5-4848-b517-5a05ddbda99f" />

Ülesanne 6.2 - gedit ja SIGHUP käsureal
<img width="955" height="593" alt="Kuvatõmmis 2025-10-28 220716" src="https://github.com/user-attachments/assets/b6273c9b-6e2f-457f-a635-bb5e01e1206a" />

Ülesanne 6.3 - käsu "ps -axu | grep daemon" modifitseerimine
<img width="953" height="595" alt="Kuvatõmmis 2025-10-28 222416" src="https://github.com/user-attachments/assets/25c2974f-b3c0-42a2-a765-d4b7131bb13d" />

Ülesanne 6.4 - käsu "ip a | grep ... | cut ... jne" koostamine faili salvestamine ja pingimine

Et arvuti IP-aadress kätte seada kasutasin käsku: ip a | grep 'inet ' | grep -v '127.0.0.1' | awk '{print $2}' | cut -d'/' -f1
<img width="952" height="596" alt="Kuvatõmmis 2025-10-28 233718" src="https://github.com/user-attachments/assets/be04b283-714a-4b9c-bd49-abdd1cf21165" />

Ülesanne 6.5 - teated0ut.txt sõnumite uurimine

Sõnum 1: 23:51:55.089,512,"WM_MOUSEMOVE",1,12321285
  - saadetakse/kirjutatakse, kui kursor liigub.
  - wParam: 1 - tähendab, et vasak hiirenupp on alla vajutatud
  - IParam: 12321285 - hiire koordinaadid ühe arvuna, koordinaatide asukohad loetakse  pikslite kaupa ülevalt vasakult nurgast. 
  - info link: https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-mousemove

Sõnum 2: 23:51:55.108,132,"WM_NCHITTEST",0,28181234
  - saadetakse/kirjutatakse, kui toimub akna raami liigutamine, kasutatakse akna ja/või piiri määramisel, et saada aru, kas klikk toimub tava alal, või aknal.
  - wParam: 0 - seda parameetrit selle funktsiooniga ei kasutata.  
  - IParam: 28181234, hiire koordinaadid ühe arvuna, koordinaatide asukohad loetakse  pikslite kaupa ülevalt vasakult nurgast
  - info link: https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-nchittest 

Suutsin paar ??? sõnumit saada, mille ID on väiksem kui 45000.
 - 00:44:20.371,513,"???",1,2556233
 - 00:44:20.597,514,"???",0,7799307
 - 00:44:33.504,522,"???",7864323,27002182
 - 00:44:33.545,519,"???",19,7209110
 - 00:44:33.650,520,"???",3,7209110
