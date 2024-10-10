
Ime projekta: Pozarko – Sistem za evakuacijo v primeru požara

Pozarko je aplikacija, zasnovana za pametne telefone, ki izboljšuje varnost in organizacijo evakuacij v primeru požara v podjetjih ali velikih zgradbah. Sistem deluje v povezavi z oddajniki signala, ki so nameščeni v stavbi, ter sledi lokaciji uporabnikov preko GPS-a. Ob sprožitvi požarnega alarma aplikacija prikaže evakuacijske poti in spremlja, kdo je že zapustil stavbo, ter pomaga vodji intervencije pri spremljanju stanja evakuacije.

 Ključne funkcionalnosti:

1. Obvestilo o evakuaciji: 
   - Ko sistem zazna požarni alarm, aplikacija pošlje takojšnje obvestilo na pametne telefone vseh zaposlenih v stavbi, da sproži evakuacijo.

2. Vizualni prikaz evakuacijske poti:
   - Aplikacija prikazuje zemljevid stavbe, kjer so označeni vsi izhodi za evakuacijo, in prilagaja poti glede na lokacijo uporabnika z uporabo GPS-a in oddajnikov (beaconov) za natančno notranjo navigacijo.

3. Spremljanje prisotnosti:
   - Aplikacija beleži, kdo je zapustil stavbo, in kdo še vedno ostaja znotraj zgradbe. To temelji na zaznavi GPS signala in signalov oddajnikov.
   - Uporabniki se lahko tudi ročno označijo kot "varni", ko dosežejo evakuacijsko točko zunaj stavbe.

4. Spremljanje lokacije v realnem času:
   - Vodja intervencije lahko v realnem času spremlja lokacijo vseh zaposlenih, ki še niso zapustili stavbe, in s tem optimizira reševalne operacije. GPS podatki in notranji oddajniki omogočajo sledenje natančnim lokacijam v stavbi.

5. Zaključek evakuacije:
   - Ko so vsi varno evakuirani, vodja intervencije prejme potrditve, ali so vsi udeleženci iz stavbe zunaj in na varnem. To omogoča lažje spremljanje in zagotavlja, da nihče ni ostal ujet znotraj.

6. Oddajniki signala (beaconi):
   - Sistem uporablja majhne oddajnike signala (Bluetooth beacons) znotraj stavbe za natančno sledenje zaposlenih. Beaconi pomagajo pri navigaciji znotraj stavbe in omogočajo natančno spremljanje pozicije, ko GPS signal ni dovolj natančen.

7. GPS integracija:
   - Ko zaposleni zapustijo stavbo, aplikacija preklopi na GPS signal in spremlja, ali so dosegli varno točko.

8. Alarm in zvočna obvestila:
   - Aplikacija lahko oddaja glasne zvočne signale za dodatno obveščanje, ko je sprožen alarm.

9. Dostop za vodjo intervencije:
   - Poseben dostop do aplikacije za vodjo intervencije omogoča pregled nad evakuacijo, prejemanje obvestil, kdo je že zunaj, ter pregled nad tem, kje so še osebe, ki niso evakuirane.

 Tehnologije

1. Mobilna aplikacija (iOS/Android):
   - Razvita z uporabo React Native, Flutter ali native kodiranja za zagotavljanje odzivnosti in široke dostopnosti na različnih mobilnih platformah.
   - GPS sledenje integrirano z Google Maps API za natančno določanje lokacije.

2. Bluetooth beaconi:
   - Oddajniki signala, nameščeni na ključnih lokacijah znotraj stavbe, omogočajo sledenje gibanju znotraj stavbe. Uporablja se tehnologija Bluetooth Low Energy (BLE) za minimalno porabo energije in natančno sledenje.

3. Backend strežnik:
   - Sistem temelji na Node.js, Django ali Laravel za spremljanje in shranjevanje podatkov v realnem času.
   - Uporaba WebSocket tehnologije za takojšnje obveščanje in sledenje uporabnikom v realnem času.
   - Baza podatkov (npr. PostgreSQL, MySQL) hrani informacije o uporabnikih, lokacijah, zgodovini evakuacij, in statusu posameznikov.

4. Firebase/Push Notifications:
   - Firebase Cloud Messaging (FCM) za pošiljanje obvestil v realnem času, ko je sprožen alarm ali se spremeni status evakuacije.

5. Cloud Storage:
   - Uporaba oblačne storitve (npr. AWS, Google Cloud) za varno shranjevanje podatkov, kot so lokacije posameznikov in varnostni podatki.

6. Web aplikacija za nadzor:
   - Razvita v React, Vue.js ali Angular za vodjo intervencije, kjer lahko v realnem času spremlja evakuacijo, status zaposlenih in prejema poročila o stanju v zgradbi.

 Prednosti sistema

- Hitro in zanesljivo obveščanje: Takoj po sprožitvi požarnega alarma so vsi zaposleni obveščeni o nujni evakuaciji.
- Natančno sledenje: Oddajniki in GPS omogočajo natančno sledenje, kar zagotavlja, da vodja intervencije ve, kje se nahajajo zaposleni in ali so že na varnem.
- Uporaba obstoječih pametnih naprav: Sistem temelji na pametnih telefonih, ki jih ljudje že nosijo s seboj, kar zmanjša potrebo po dodatni opremi.
- Enostavno upravljanje in pregled: Vodja intervencije ima vedno dostop do najnovejših podatkov o evakuaciji in lahko ustrezno ukrepa.

 Razvojna faza

Projekt je trenutno v razvoju. V prihodnjih mesecih bodo dodane naslednje funkcionalnosti:
- Optimizacija notranjega sledenja z Bluetooth beacon tehnologijo.
- Testiranje sistema s simulacijami evakuacije.
- Izboljšave uporabniškega vmesnika za preprosto in intuitivno uporabo.
