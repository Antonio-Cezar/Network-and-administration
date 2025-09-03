# Network-and-administrationd


# Operation Center (Bash Project)

Et læringsprosjekt i **Bash scripting** som simulerer et *ROOT administrator kontrollsenter* med innlogging, menyer og moduler for vanlige sysadmin-operasjoner.  

Prosjektet er bygget opp modulært: hovedscriptet (`root-operation-center`)

---

## 🚀 Funksjoner
- **Root-sjekk**: Scriptet avslutter hvis det ikke kjøres som root (via `id -u`)  
- **Innlogging**: Simulert admin-login med brukernavn og passord lagret i `admin_credentials.txt`
- **Menybasert grensesnitt** (via `case`) med valg som:
  - Legge til bruker  
  - Slette bruker  
  - Redigere root-admin bruker  
  - Verifisere root-admin gyldighet  
  - Backup av systemet  
  - Vise brukere  
  - Diskplass-sjekk  
  - Grep etter bruker  
  - Vise egen info  
  - NMAP TCP SYN-scan  
  - Vise varsler (Zenity)  
  - Avslutte root-senteret  

---

## 🛠️ Teknologi
- **Bash** som hovedspråk  
- Modulær struktur med eksterne script (eks. `./add_root`, `./delete-user`)  
- Bruk av `case` for menyvalg  
- Enkel **innloggingsmekanisme** med brukernavn/passord fra tekstfil  
- Enkel "2FA-effekt" gjennom ekstra verifisering (`verify_root_check`)  

---