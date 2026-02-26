# CLAUDE.md — Upute za projekt

## O projektu

Ovaj repozitorij sadrži sve materijale za radionicu **"AI kao pomoćnik u župnom radu"** namijenjenu župnim suradnicima Zagrebačke nadbiskupije. Radionica traje 90 minuta, kombinira teorijski uvod s praktičnim radom, a cilj joj je osposobiti sudionike za samostalno korištenje AI alata (ponajprije Claude, besplatna verzija) u svakodnevnim župnim zadacima.

## Ciljana publika

Župni suradnici: tajnici, katehetice i katehete, animatori, voditelji župnih vijeća, komunikatori na društvenim mrežama, volonteri uključeni u administraciju. Tehnička razina je početna do srednja. Većina sudionika nema iskustva s AI alatima. Očekuje se do 15 sudionika.

## Struktura radionice

| Blok | Trajanje | Sadržaj | Format |
|------|----------|---------|--------|
| 1 — Uvod i demistifikacija | 20 min | Demonstracija uživo, objašnjenje što je AI, prednosti, ograničenja, etička dimenzija | Prezentacija i demo |
| 2 — Kako pisati dobre promptove | 15 min | UZKO okvir (Uloga, Zadatak, Kontekst, Oblik), usporedba lošeg i dobrog prompta | Prezentacija s primjerima uživo |
| 3 — Praktična radionica | 35 min | Tri vježbe iz župne prakse (društvene mreže, email, slobodan izbor) | Rad u parovima ili individualno |
| 4 — Generiranje slika | 10 min | Demonstracija alata za generiranje slika (Copilot/DALL-E), mogućnosti i ograničenja | Demo uživo, publika predlaže promptove |
| 5 — Zaključak | 10 min | Tri ključne poruke, resursi, QR kod, pitanja i razmjena iskustava | Diskusija |

---

## Datoteke u repozitoriju

Repozitorij sadrži sljedeće datoteke. Svaka je opisana u nastavku zajedno s detaljnim uputama za izradu.

### 1. `README.md`

Opis repozitorija za GitHub. Sadrži:
- Naslov projekta i kratki opis (2 do 3 rečenice)
- Informacije o radionici (trajanje, publika, kontekst)
- Popis svih datoteka u repozitoriju s kratkim opisom svake
- Linkove na sve resurse (relativni linkovi unutar repoa)
- Informacije o licenci (CC BY-NC-SA 4.0 ili slično)
- Jezik: hrvatski

### 2. `prezentacija/ai-u-zupnom-radu.pptx`

PowerPoint prezentacija od 21 slajda. Služi kao vizualna pratnja radionici. Dizajn treba biti moderan, čist i profesionalan, s toplim tonovima (tamno plava, bijela, akcent u toploj zlatnoj ili narančastoj boji). Bez pretjeranog teksta na slajdovima — prezentacija služi kao vizualna podrška, ne kao skripta za čitanje.

#### Upute za dizajn
- Koristiti python-pptx biblioteku
- Dimenzije: widescreen 16:9
- Font: Calibri ili equiv. sans-serif
- Boje: primarna tamno plava (#1B3A5C), sekundarna bijela (#FFFFFF), akcent topla zlatna (#D4A843), tekst tamno sivi (#2D2D2D), pozadina svijetlo siva (#F5F5F5)
- Svaki slajd ima naslov i minimalan tekst, vizualno je čist
- Koristiti oblike, linije i boje za vizualnu hijerarhiju umjesto velikih blokova teksta
- Slajdovi s primjerima promptova mogu imati više teksta jer je sam prompt sadržaj

#### Sadržaj po slajdovima

**Slajd 1 — Naslovnica**
- Naslov: AI kao pomoćnik u župnom radu
- Podnaslov: Praktična radionica za župne suradnike
- Detalji: Zagrebačka nadbiskupija, 2026.

**Slajd 2 — Što ćemo danas naučiti**
- Četiri točke u vizualnom rasporedu (ikone ili brojevi):
  1. Razumjeti što AI jest i što nije
  2. Naučiti razgovarati s AI alatom
  3. Isprobati AI na stvarnim župnim zadacima
  4. Vidjeti kako AI stvara slike

**Slajd 3 — Počnimo s primjerom**
- Naslov koji signalizira live demo
- Vizualni prikaz: simulacija chat sučelja ili jednostavna ikona monitora
- Napomena za voditelja: ovdje se prebacuje na live demo u Claudeu

**Slajd 4 — Što je zapravo AI**
- Tri razine objašnjenja vizualno prikazane (npr. tri kartice ili stupca):
  - Treniran na ogromnoj količini teksta
  - Predviđa najkorisniji odgovor
  - Nema svijest, uvjerenja ni vjeru
- Analogija: osoba koja je pročitala svaku knjigu ali nikada nije izašla iz kuće

**Slajd 5 — Što AI radi dobro**
- Vizualni popis s ikonama (6 stavki):
  - Pisanje i prepisivanje tekstova
  - Sažimanje dugih dokumenata
  - Prilagodba tona i stila
  - Brainstorming i ideje
  - Prijevod i jezična pomoć
  - Strukturiranje raspršenih misli

**Slajd 6 — Što AI ne radi dobro**
- Vizualni popis s ikonama upozorenja (5 stavki):
  - Činjenična točnost (izmišlja s uvjerenjem)
  - Teološka preciznost (miješa perspektive)
  - Pastoralni sud (ne poznaje ljude)
  - Aktualne informacije (nema pristup internetu)
  - Matematika i precizni izračuni

**Slajd 7 — Etička dimenzija**
- Četiri točke:
  - Vatikan i AI: poruka pape Franje za Svjetski dan mira 2024.
  - Privatnost: nikada ne unosite osobne podatke župljana
  - Transparentnost: budite iskreni o korištenju AI-ja
  - AI ne zamjenjuje osobni susret

**Slajd 8 — Što je prompt**
- Jednostavna definicija: uputa koju tipkate u AI alat
- Analogija s davanjem uputa novom volonteru
- Vizualni element: strelica od prompta prema rezultatu

**Slajd 9 — UZKO okvir za dobar prompt**
- Vizualni okvir s četiri elementa (svaki u svojoj boji ili kartici):
  - U = Uloga (Tko je AI u ovom razgovoru?)
  - Z = Zadatak (Što točno trebate?)
  - K = Kontekst (Koji su relevantni detalji?)
  - O = Oblik (Ton, duljina, stil?)
- Kratak primjer uz svaki element

**Slajd 10 — Loš prompt vs dobar prompt**
- Dva stupca ili dva okvira:
  - Lijevo (crvenkasto): "Napiši nešto o misi."
  - Desno (zelenkasto): Puni prompt s UZKO elementima za Facebook objavu o blagdanu sv. Josipa
- Napomena: ovdje se radi live usporedba u Claudeu

**Slajd 11 — Dodatni savjeti**
- 5 do 6 kratkih savjeta:
  - Razgovarajte, ne šaljite samo jednu poruku
  - Dajte mu svoj tekst da poboljša
  - Tražite više verzija
  - Zadajte format izričito
  - Ako nešto ne valja, recite mu
  - Koristite AI za zadatke za koje nemate vremena

**Slajd 12 — Upute za praktični rad**
- Kratke organizacijske upute:
  - Otvorite claude.ai na svom uređaju
  - Tko nema uređaj, radi u paru s kolegom
  - UZKO okvir ostaje na ekranu kao podsjetnik
  - Ako zapnete, podignite ruku

**Slajd 13 — Vježba 1: Objava za društvene mreže**
- Zadatak: napišite Facebook/Instagram objavu za župni događaj
- Korak po korak: odaberemo događaj, gradimo prompt zajedno, pokrenemo, usavršimo
- Vrijeme: 12 minuta

**Slajd 14 — Vježba 2: Službeni email ili pismo**
- Tri opcije:
  - A: Zahvalnica volonterima
  - B: Poziv na sastanak pastoralnog vijeća
  - C: Obavijest o promjeni rasporeda misa
- Vrijeme: 12 minuta

**Slajd 15 — Vježba 3: Odaberite svoj izazov**
- Izbornik opcija:
  1. Sažetak crkvenog dokumenta
  2. Priprema za katehezu
  3. Razmišljanje za bilten
  4. Ideje za aktivnosti
  5. Prepisivanje za drugu publiku
  6. Slobodan izbor
- Vrijeme: 11 minuta

**Slajd 16 — AI može i stvarati slike**
- Kratko objašnjenje mogućnosti
- Koje alate koristiti: ChatGPT (DALL-E), Microsoft Copilot, Canva
- Napomena: Claude besplatna verzija ne generira slike

**Slajd 17 — Demonstracija generiranja slika**
- Naslov koji signalizira live demo
- Vizualni element: placeholder za prikaz generiranih slika
- Napomena za voditelja: ovdje se koristi Copilot ili drugi alat uživo

**Slajd 18 — Ograničenja kod slika**
- Vizualni popis:
  - Ruke i prsti često neispravni
  - Tekst u slici nečitljiv
  - Lica ponekad neprirodno izgledaju
  - Ilustracije rade bolje od fotorealističnog stila
  - Uvijek pregledajte prije objave

**Slajd 19 — Tri stvari za zapamtiti**
- Tri velika vizualna elementa (kartice ili ikone):
  1. AI je alat, vi ste stručnjak
  2. Dobar prompt = dobar rezultat (UZKO)
  3. Uvijek pregledajte, nikada ne šaljite bez provjere

**Slajd 20 — Vaši resursi**
- QR kod (placeholder) za digitalni letak
- Popis resursa: Claude (claude.ai), ChatGPT, Microsoft Copilot, Canva
- Kontakt voditelja radionice

**Slajd 21 — Pitanja i razmjena iskustava**
- Potpitanja za diskusiju:
  - Što vas je najviše iznenadilo?
  - Za koji biste zadatak prvi koristili AI?
  - Imate li nedoumice?
- Završna poruka: "Hvala na sudjelovanju!"

---

### 3. `tekst/ai-u-zupnom-radu-opis.md`

Deskriptivni dokument koji opisuje sadržaj radionice u formi stručnog teksta (stilski blizak stručnom radu ili članku). Ovo nije prezentacija ni vodič, nego cjelovit opis koji se može koristiti za objavu, izvještaj ili dokumentaciju.

#### Struktura dokumenta

**Naslov:** AI kao pomoćnik u župnom radu: radionica za župne suradnike Zagrebačke nadbiskupije

**Sažetak (apstrakt):** 150 do 200 riječi. Opisuje kontekst, cilj, sadržaj i očekivane ishode radionice.

**1. Uvod**
Kontekstualizacija teme: širenje AI alata u svakodnevnom životu i radu, relevantnost za crkvene zajednice, potreba za edukacijom župnih suradnika. Referenca na stav Katoličke crkve prema tehnologiji (poruka pape Franje za Svjetski dan mira 2024.). Cilj radionice: demistificirati AI i osposobiti suradnike za praktičnu uporabu.

**2. Teorijski okvir**
2.1. Što je umjetna inteligencija: objašnjenje velikih jezičnih modela pristupačnim jezikom, analogije, razgraničenje između onoga što AI jest i što nije.
2.2. Mogućnosti AI alata u kontekstu župnog rada: pisanje, sažimanje, brainstorming, prilagodba tona, prijevod. Konkretni primjeri iz župne prakse.
2.3. Ograničenja i rizici: halucinacije, teološka nepreciznost, nedostatak pastoralnog suda, privatnost podataka.
2.4. Etička dimenzija: stav Crkve, pitanje transparentnosti, odnos AI alata i osobnog susreta u pastoralu.

**3. Metodologija radionice**
3.1. Format i trajanje: 90 minuta, kombinacija predavanja, demonstracije uživo i praktičnog rada.
3.2. Ciljana skupina: župni suradnici bez prethodnog iskustva s AI alatima, do 15 sudionika.
3.3. Alati: Claude (besplatna verzija) za tekstualni rad, Microsoft Copilot za demonstraciju generiranja slika.
3.4. Priprema sudionika: prethodno kreiranje računa, parni rad za one bez uređaja.

**4. Sadržaj radionice**
4.1. Uvod i demistifikacija (20 min): opis pristupa, live demo, objašnjenje, etika.
4.2. Pisanje dobrih promptova (15 min): UZKO okvir, usporedba lošeg i dobrog prompta, savjeti za iterativni rad.
4.3. Praktična radionica (35 min): tri vježbe (objava za društvene mreže, službeni email, slobodan izbor), opis svake vježbe i facilitacijske napomene.
4.4. Generiranje slika (10 min): demonstracija, mogućnosti, ograničenja.
4.5. Zaključak (10 min): ključne poruke, resursi, otvorena diskusija.

**5. Očekivani ishodi**
Što sudionici trebaju znati i moći nakon radionice: samostalno koristiti Claude za osnovne tekstualne zadatke, primijeniti UZKO okvir, prepoznati ograničenja AI-ja i uvijek pregledati generirani sadržaj.

**6. Zaključak**
Refleksija o ulozi AI-ja u crkvenoj zajednici, naglasak na komplementarnosti tehnologije i osobnog susreta, poticaj na nastavak učenja.

#### Stil pisanja
- Stručan ali pristupačan, ne pretjerano akademski
- Treće lice ili bezlični oblik
- Podnaslovi i paragrafi, bez bullet lista
- Duljina: oko 2500 do 3500 riječi
- Jezik: hrvatski

---

### 4. `tekst/vodic-za-voditelja.md`

Detaljan vodič za voditelja radionice. Ovo je operativni dokument koji voditelj koristi tijekom pripreme i provedbe radionice. Sadrži sve što treba znati za svaki slajd: što reći, što pokazati, na što paziti, koliko vremena potrošiti.

#### Struktura dokumenta

Dokument prati strukturu prezentacije slajd po slajd. Za svaki slajd sadrži:

- **Naslov slajda** i broj
- **Ključne poruke** koje voditelj treba prenijeti
- **Što reći** — konkretni razgovorni tekst, ne za čitanje naglas nego kao detaljni podsjetnik. Uključuje analogije, primjere i fraze koje dobro funkcioniraju.
- **Što pokazati** — upute za live demo dijelove (koji prompt upisati, što očekivati kao rezultat, kako reagirati na neočekivane rezultate)
- **Facilitacijske napomene** — savjeti za interakciju s grupom, česta pitanja, moguće poteškoće, tajming
- **Prijelaz** — kako povezati ovaj slajd sa sljedećim

Za blokove s vježbama dokument sadrži:
- Točan opis svake vježbe
- Pripremljene scenarije i primjere promptova
- Upute za cirkulaciju i pomoć sudionicima
- Plan za sudionike bez uređaja
- Vremenske oznake (koliko minuta za svaki korak)

Na kraju dokumenta:
- Kontrolna lista za pripremu prije radionice (tehnika, materijali, email sudionicima)
- Plan B za tehničke probleme (internet ne radi, Claude ne odgovara, itd.)
- Predložak emaila za slanje sudionicima prije radionice

#### Stil pisanja
- Direktan, praktičan, u drugom licu jednine (obraća se voditelju)
- Konkretan i specifičan, izbjegavati općenite savjete
- Duljina: oko 4000 do 5500 riječi
- Jezik: hrvatski

---

## Tehnički zahtjevi

### Za prezentaciju (.pptx)
- Koristiti python-pptx biblioteku
- Widescreen format 16:9
- Fontovi: Calibri za naslove i tekst
- Vizualno čist dizajn s minimalnim tekstom
- Oblike i boje koristiti za vizualnu hijerarhiju
- Svaki slajd mora imati konzistentan layout

### Za markdown dokumente
- UTF-8 enkodiranje
- Standardni markdown (kompatibilan s GitHub renderingom)
- Bez HTML-a osim ako je nužan za specifičan prikaz

### Struktura direktorija

```
ai-u-zupnom-radu/
├── README.md
├── CLAUDE.md
├── prezentacija/
│   └── ai-u-zupnom-radu.pptx
└── tekst/
    ├── ai-u-zupnom-radu-opis.md
    └── vodic-za-voditelja.md
```

## Napomene

- Sav sadržaj je na hrvatskom jeziku
- Izbjegavati anglizme gdje postoji hrvatski ekvivalent, osim za ustaljene tehničke termine (prompt, AI, chatbot)
- Tonalitet je profesionalan ali pristupačan, prikladan za crkveni kontekst
- Svi primjeri promptova u dokumentima trebaju biti konkretni i realistični za župni rad
- Referenca na papu Franju i Svjetski dan mira 2024. treba biti točna
