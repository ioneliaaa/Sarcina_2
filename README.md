# Sarcina_2
# Sarcina – Testare API în Postman

Această sarcină verifică funcționalitatea API-ului de la https://reqres.in folosind Postman și date externe.

## 🔧 Colecția conține:
- ✅ GET request: verificare cod 200
- ✅ PUT request: test actualizare (cod 200)
- ✅ DELETE request: test ștergere (cod 200)
- ❌ POST request: eșuat cu 401 Unauthorized

## 🔁 Date externe:
- Fișierul `users.json` conține 10 utilizatori diferiți (nume + job)
- Fiecare test POST se rulează cu date diferite, automat

## 🧪 Testele POST verificate:
1. Codul răspunsului să fie 201
2. ID-ul returnat să fie numeric
3. `createdAt` să fie o dată ISO validă

➡️ Toate aceste teste au eșuat deoarece serverul a returnat `401 Unauthorized`. Cauza posibilă: neacceptarea datelor externe sau lipsa unui token.

## 📁 Fișiere incluse:
- `collection.json` – colecția exportată
- `users.json` – datele de test extern
- `run-results.json` – rezultatul exportat din Runner
- `results.png` – captură de ecran cu testele rulate

## ✅ Pași pentru rulare:
1. Deschide Postman
2. Importă `collection.json`
3. Mergi în Runner
4. Încarcă `users.json` ca fișier de date
5. Rulează cu 10 iterări
6. Vezi rezultatele și exportează dacă e necesar

Testul este complet și funcțional, chiar dacă unele assertions au eșuat.
