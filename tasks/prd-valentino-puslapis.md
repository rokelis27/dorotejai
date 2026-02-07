# PRD: Valentino Dienos Puslapis

## Įvadas

Interaktyvus vieno puslapio web-aplikacija, kurioje paklausiama „Ar būsi mano Valentinė?" su dviem mygtukais: TAIP ir NE. NE mygtukas pabėga nuo pelės/piršto, todėl jį neįmanoma paspausti. Paspaudus TAIP, atsiveria romantiškas puslapis su bendromis nuotraukomis ir atidarytimu meilės laišku. Viskas lietuvių kalba.

**Hostinimas:** Nemokamai per GitHub Pages (nereikia pirkti domeno).

## Tikslai

- Sukurti veikiantį vieno puslapio web app be jokio backend'o
- Romantiškas dizainas su cute/juokingu elementu (pabėgantis NE mygtukas)
- Rodyti 4-8 bendrų nuotraukų galeriją
- Turėti atidaromą meilės laišką su template tekstu
- Viskas lietuvių kalba
- Nemokamas hostinimas per GitHub Pages

## User Stories

### US-001: Pagrindinis klausimo ekranas
**Aprašymas:** Kaip lankytojas, noriu matyti gražiai pateiktą klausimą „Ar būsi mano Valentinė?" su dviem mygtukais, kad galėčiau atsakyti.

**Priėmimo kriterijai:**
- [ ] Centruotas klausimas „Ar būsi mano Valentinė?" dideliu šriftu
- [ ] Du mygtukai: „Taip" (žalias/rožinis) ir „Ne" (pilkas/mažesnis)
- [ ] Animuotos širdutės fone (subtilus efektas)
- [ ] Responsyvus — veikia telefone ir kompiuteryje
- [ ] Patikrinti naršyklėje

### US-002: Pabėgantis NE mygtukas
**Aprašymas:** Kaip kūrėjas, noriu kad NE mygtukas pabėgtų nuo pelės/piršto, kad būtų juokinga ir neįmanoma paspausti NE.

**Priėmimo kriterijai:**
- [ ] Kompiuteryje: kai pelė artėja prie NE mygtuko, jis pašoka į atsitiktinę kitą poziciją
- [ ] Telefone: kai paspaudžia NE mygtuką, jis pašoka į kitą vietą (nes nėra hover)
- [ ] Mygtukas visada lieka matomas ekrane (nepabėga už ribų)
- [ ] Kiekvienas pabėgimas turi skirtingą juokingą lietuvišką tekstą (pvz. „Pagalvok dar kartą!", „Tikrai ne?", „Pabandyk dar!")
- [ ] Patikrinti naršyklėje

### US-003: TAIP rezultato ekranas su nuotraukomis
**Aprašymas:** Kaip lankytojas paspaudęs TAIP, noriu matyti gražią nuotraukų galeriją su bendromis nuotraukomis.

**Priėmimo kriterijai:**
- [ ] Paspaudus TAIP, sklandus perėjimas į naują ekraną
- [ ] Džiaugsmingas pasveikinimas viršuje (pvz. „Žinojau! ❤️")
- [ ] 4-8 nuotraukų galerija grid arba masonry layout
- [ ] Nuotraukos su placeholder'iais — lengva pakeisti savo nuotraukomis
- [ ] Responsyvus — veikia telefone ir kompiuteryje
- [ ] Patikrinti naršyklėje

### US-004: Meilės laiškas
**Aprašymas:** Kaip lankytojas, noriu atidaryti meilės laišką su romantiška žinute.

**Priėmimo kriterijai:**
- [ ] Mygtukas „Atidaryti laiškelį" po nuotraukų galerijos
- [ ] Paspaudus, atsiveria laiškas su animacija (voko atidarymas arba fade-in)
- [ ] Laiško template lietuvių kalba su placeholder tekstu kurį lengva pakeisti
- [ ] Gražus laiško dizainas (kaip tikras laiškas/vokas)
- [ ] Patikrinti naršyklėje

## Funkciniai reikalavimai

- FR-1: Visas app'as — vienas `index.html` failas (HTML + CSS + JS inline), be jokių išorinių priklausomybių
- FR-2: Nuotraukos saugomos `photos/` aplanke, nuorodos HTML kode
- FR-3: NE mygtukas reaguoja į `mouseenter` (desktop) ir `touchstart`/`click` (mobile) — pašoka į naują atsitiktinę poziciją ekrane
- FR-4: TAIP mygtukas perjungia iš klausimo ekrano į rezultato ekraną (be puslapio perkrovimo)
- FR-5: Konfeti arba širdučių animacija paspaudus TAIP
- FR-6: Laiško turinys lengvai redaguojamas — pažymėtas komentarais kode
- FR-7: Visa kalba — lietuvių

## Ne-tikslai (už ribų)

- Jokio backend'o ar duomenų bazės
- Jokio prisijungimo ar autentifikacijos
- Nereikia muzikos ar garso efektų
- Nereikia dark mode
- Nereikia daugiakalbystės (tik lietuvių)

## Dizaino pastabos

- **Spalvos:** Rožinė, raudona, balta — Valentino dienos nuotaika
- **Šriftai:** Google Fonts — kažkas romantiškas/elegantiškas (pvz. `Playfair Display` arba `Dancing Script`)
- **Animacijos:** Širdutės fone, konfeti paspaudus TAIP, sklandūs perėjimai
- **Stilius:** Romantiškas su cute/juokingu elementu (pabėgantis mygtukas)

## Techninės pastabos

- Vienas HTML failas — paprasčiausias deploy'inimas
- Nuotraukos atskiri failai `photos/` aplanke (kad būtų lengva keisti)
- CSS ir JS inline arba `<style>`/`<script>` taguose
- Naudoti CSS animacijas kur įmanoma (veikia greičiau nei JS animacijos)
- Google Fonts per `<link>` tagą (vienintelė išorinė priklausomybė)

## Hostinimas (GitHub Pages)

1. Sukurti GitHub repozitoriją
2. Įkelti `index.html` + `photos/` aplanką
3. Settings → Pages → Deploy from main branch
4. Gauni URL: `https://username.github.io/valentine`
5. Nusiųsti šią nuorodą merginai

## Sėkmės metrikos

- Mergina paspaudžia TAIP (100% conversion rate expected 😄)
- Puslapis veikia be klaidų telefone ir kompiuteryje
- Nuotraukos ir laiškas rodomi teisingai

## Atviri klausimai

- Nėra — galima pradėti implementaciją!
