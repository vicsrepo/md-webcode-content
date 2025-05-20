# Vytvoření nové složky synchronizované s GitHub repozitářem pomocí **GitHub Desktop**

---

### **Krok 1: Vytvoření nového repozitáře**

1. **Otevřete GitHub Desktop** a klikněte na **File > New repository** (nebo tlačítko **Create a New Repository**).
2. Vyplňte údaje:
   - **Name**: Název repozitáře (např. `moje-slozka`).
   - **Local Path**: Vyberte cestu k nové složce na disku (např. `C:\Users\Jméno\Documents\GitHub\moje-slozka`).  
     *GitHub Desktop automaticky vytvoří tuto složku.*
   - **Initialize with a README**: Zaškrtněte, pokud chcete základní soubor `README.md`.
   - **Git Ignore** a **License**: Volitelné.
3. Klikněte na **Create Repository**.

---

### **Krok 2: Propojení s GitHubem**

Pokud jste **nevytvořili repozitář na GitHubu** během prvního kroku:

1. Klikněte v GitHub Desktop na **Publish repository** (vpravo nahoře).
2. Zaškrtněte **Keep this code private**, pokud chcete soukromý repozitář.
3. Klikněte na **Publish Repository**.  
   *Složka na vašem disku je nyní propojena s novým repozitářem na GitHubu.*

---

### **Krok 3: Přidání souborů/složek**

1. Otevřete složku repozitáře v Průzkumníku souborů:
   - Klikněte na **Repository > Show in Explorer** v GitHub Desktop.
2. Přesuňte soubory nebo složky do této lokální složky.
3. V GitHub Desktop uvidíte změny v sekci **Changes** (vlevo).

---

### **Krok 4: Synchronizace změn (commit + push)**

1. **Commit** (lokální uložení změn):
   - Do pole **Summary** napište popis (např. "Přidána nová složka").
   - Klikněte na **Commit to main** (nebo jinou větev).
2. **Push** (nahrání na GitHub):
   - Klikněte na **Push origin** vpravo nahoře.  
     *Vaše složka je nyní synchronizována s GitHubem.*

---

### **Důležité poznámky**

- **Prázdné složky**: Git je ignoruje. Pokud potřebujete prázdnou složku v repozitáři, vytvořte v ní prázdný soubor (např. `.gitkeep`).
- **Automatická synchronizace**: GitHub Desktop **neumožňuje plnou automatizaci** (musíte manuálně commitovat a pushovat). Pro automatizaci použijte:
  - **Skripty**: Naplánujte `git add`, `commit`, `push` přes **Task Scheduler**.
  - **GitHub Actions**: Pro automatické nasazení z jiných služeb.

---

### **Příklad: Synchronizace existujícího repozitáře**

Pokud už repozitář na GitHubu existuje:

1. V GitHub Desktop klikněte na **Clone a Repository**.
2. Vyberte repozitář ze seznamu nebo vložte URL (např. `https://github.com/username/repo-name.git`).
3. Zvolte **Local Path** pro novou složku na disku.
4. Klikněte na **Clone**.  
   *Složka se automaticky propojí s GitHubem.*

---

Pokud máte problémy s oprávněními nebo synchronizací, zkontrolujte:

1. Zda jste přihlášeni v GitHub Desktop.
2. Zda je repozitář veřejný/soukromý a máte k němu přístup.
3. Zda cestu k lokální složce neblokuje antivirus nebo firewall. 😊
