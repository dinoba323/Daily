# Daily – radni podsjetnik

Privatna web aplikacija s tri kolone:

- **Zadaci** – to-do lista s rokovima i prioritetima, plus podsjetnici iz CRM-a (datum ponovnog kontakta).
- **Pošta** – najnoviji emailovi iz Outlooka (Microsoft 365), razvrstani na *hitno*, *treba odgovoriti* i *informativno*, povezani sa zadacima i tragovima.
- **CRM** – tržišni tragovi (Tragovi / Aktuelno / Staro), uređivanje s računara i telefona, izvoz u .xlsx.

Aplikacija je objavljena kao Claude artifact (`index.html`) i koristi:

- `db` – bazu za zadatke (`tasks`), tragove (`leads`), analizu pošte (`mailtriage`) i status sinhronizacije (`meta/sync`);
- `mcp` – Microsoft 365 `outlook_email_search` za čitanje pošte;
- `sample` – Claude za razvrstavanje emailova;
- `downloads` – izvoz tragova u Excel.

Zakazani zadatak svaki sat (radnim danima 7–19 h) dvosmjerno sinhronizuje kolekciju `leads` s `D:\Dropbox\PRODAJA\TRAGOVI\Prodajni_tragovi.xlsx`.
