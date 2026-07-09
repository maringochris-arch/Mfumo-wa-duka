# 🏪 Mfumo wa Duka

Mfumo kamili wa usimamizi wa biashara/duka — unafanya kazi **bila mtandao (offline)** kama PWA (Progressive Web App). Data zote zinahifadhiwa moja kwa moja kwenye kifaa chako (localStorage) — hakuna internet inayohitajika baada ya kufungua mara ya kwanza.

## ✨ Vipengele (Features)

- **🔐 Login yenye Watumiaji** — kila mfanyakazi ana akaunti yake, na kuna ngazi mbili za matumizi:
  - **Meneja (Admin)** — anaona na kudhibiti kila kitu, ikiwemo usimamizi wa watumiaji
  - **Karani** — anaweza kuandika mauzo/manunuzi lakini kuhariri/kufuta rekodi zake mwenyewe tu
- **🏠 Muhtasari (Dashboard)** — jumla ya mauzo, faida halisi, madeni ya kudai/kulipa, thamani ya stoki, gharama za usafiri, hasara, na chati ya mwenendo wa mauzo
- **🛒 Mauzo** — kuandika mauzo, kuchagua bidhaa moja kwa moja kutoka stoki, na kutoa risiti
- **📦 Manunuzi** — kurekodi ununuzi wa bidhaa, gharama za usafiri, na hasara/uharibifu
- **🗄️ Stoki na Bidhaa** — ufuatiliaji wa idadi ya bidhaa, bei ya kununulia/kuuzia, na tahadhari ya "stoki chini" au "imeisha"
- **📤 Madeni ya Kudai** — wateja wanaodaiwa na duka
- **📥 Madeni ya Kulipa** — madeni ambayo duka linadaiwa na wengine
- **👥 Usimamizi wa Watumiaji** *(Admin tu)* — kuongeza/kuondoa wafanyakazi
- **🌗 Dark Mode** — mwonekano wa giza kwa matumizi ya usiku
- **📴 Offline kamili** — mfumo unafanya kazi hata bila mtandao baada ya kufunguliwa mara ya kwanza

## 🔑 Akaunti za Majaribio (Demo Login)

| Wadhifa | Jina la Mtumiaji | Nywila |
|---|---|---|
| Meneja (Admin) | `admin` | `admin123` |
| Karani | `karani` | `karani123` |

> ⚠️ Kumbuka: badilisha nywila hizi kabla ya kutumia mfumo kwa biashara halisi, kwa usalama zaidi.

## 📁 Faili za mfumo
- `index.html` — mfumo wenyewe (React app, faili moja tu)
- `manifest.json` — taarifa za app (jina, icons, rangi) kwa ajili ya "Add to Home Screen"
- `sw.js` — service worker inayohifadhi faili kwenye kifaa ili zifanye kazi offline
- `icon-192.png`, `icon-512.png` — icons za app

## 📲 Jinsi ya kutumia OFFLINE
1. Fungua mfumo mara moja ukiwa na mtandao (kupitia GitHub Pages au server) — hii inaruhusu service worker kuhifadhi faili zote kwenye kifaa.
2. Baada ya hapo, unaweza kufunga mtandao na mfumo utaendelea kufanya kazi kikamilifu.
3. Kwenye simu: fungua kwenye Chrome/Safari kisha chagua **"Ongeza kwenye Home Screen" / "Add to Home Screen"** ili iwe kama app halisi, inayofunguka bila kuhitaji browser.

## ☁️ Jinsi ya ku-host bure kwa GitHub Pages
1. Nenda kwenye repo yako GitHub → **Settings** → **Pages**
2. Chini ya "Branch", chagua `main` na folda `/ (root)`, kisha **Save**
3. Baada ya dakika chache, mfumo utapatikana kwenye:
   `https://maringochris-arch.github.io/Mfumo-wa-duka/`

## 💾 Kuhusu Data
Data zote (mauzo, stoki, madeni, watumiaji) zinahifadhiwa kwenye **localStorage** ya kivinjari chako — yaani zipo kwenye kifaa chako tu, si kwenye server ya nje. Kama ukifuta "cache/data" ya kivinjari, data zitapotea — hivyo ni vizuri ku-**backup** mara kwa mara (mfano: kuchukua screenshot au kuandika kwenye daftari kwa usalama).

## 🛠️ Teknolojia
Imejengwa kwa HTML, CSS na JavaScript (React bila build step) — faili moja tu, rahisi kubeba na kutumia popote.
