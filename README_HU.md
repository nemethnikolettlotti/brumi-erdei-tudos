# Brumi, az erdei tudós 🐻

Kétnyelvű (magyar/angol) webalkalmazás AI-válaszokkal, böngészős hangos felolvasással és opcionális mikrofonos kérdezéssel.

## Fontos
- Az API-kulcsot kizárólag szerveroldali környezeti változóként add meg. Ne tedd az `index.html` fájlba, és ne töltsd fel nyilvános repóba.
- Az OpenAI API használata külön számlázású lehet. Állíts be költségkeretet/értesítést az API-fiókodban.
- Ez egy oktatási prototípus. Mielőtt gyerekekkel használod, teszteld, ellenőrizd a válaszokat, és tartsd be az iskolai adatvédelmi szabályokat. Ne kérjen és ne gyűjtsön személyes adatokat.
- A mikrofon és a felolvasás működése böngészőfüggő; a mikrofon jellemzően HTTPS-en vagy localhoston működik.

## Helyi indítás
1. Telepítsd a Node.js 20 vagy újabb verzióját.
2. A mappában futtasd: `npm start`
3. Állítsd be az `OPENAI_API_KEY` környezeti változót a terminálban, mielőtt elindítod a szervert.
4. Nyisd meg: `http://localhost:3000`

### API-kulcs beállítása (példa)
macOS/Linux:
```bash
export OPENAI_API_KEY="a_sajat_kulcsod"
npm start
```
Windows PowerShell:
```powershell
$env:OPENAI_API_KEY="a_sajat_kulcsod"
npm start
```

## Éles tárhely
A szervernek Node.js-t támogató tárhely kell. Az `OPENAI_API_KEY` értékét a tárhely szolgáltatói felületén, szerveroldali környezeti változóként állítsd be. Soha ne add át a kulcsot a böngészőnek. Az ingyenes tárhelyek alvó módja, limitjei és az API költségei változhatnak.
