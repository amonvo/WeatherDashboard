# Weather Dashboard

Weather Dashboard je jednoduchá Java aplikace, která umožňuje získat aktuální informace o počasí pro zadané město. Data o počasí jsou získávána z externího API a aplikace je postavena na platformě JavaFX.

---

## 🛠 Funkce aplikace

- **Zobrazení aktuální teploty** – Uživatel zadá název města a aplikace zobrazí aktuální teplotu v °C.
- **Minimální a maximální teplota** – Zobrazují se minimální a maximální teploty pro aktuální den.
- **Vlhkost a tlak** – Informace o aktuální vlhkosti a tlaku vzduchu v daném městě.
- **Souřadnice města** – Zobrazení zeměpisné šířky a délky města.

---

## 💾 Požadavky

Než spustíte aplikaci, ujistěte se, že máte nainstalováno následující:

1. **Java Development Kit (JDK)**:
   - Doporučeno: JDK 11 nebo novější (např. Amazon Corretto).
2. **JavaFX SDK**:
   - Použito: `javafx-sdk-23.0.1`.
   - Ke stažení z: [https://gluonhq.com/products/javafx/](https://gluonhq.com/products/javafx/).
3. **Maven**:
   - Používá se pro správu závislostí a sestavení projektu.
4. **Integrované vývojové prostředí (IDE)**:
   - Doporučeno: IntelliJ IDEA (Community Edition je dostačující).

---

## 📝 Instalace

1. **Naklonování repozitáře**:
   Naklonujte repozitář na svůj lokální počítač:
   ```bash
   git clone https://github.com/uzivatel/weather-dashboard.git
   cd weather-dashboard
   
2. **Stažení JavaFX SDK**
Stáhněte a nastavte JavaFX SDK:

Stáhněte JavaFX SDK z oficiálních stránek:
https://gluonhq.com/products/javafx/

Rozbalte stažený soubor do vámi preferované složky. Například:


C:\javafx-sdk-23.0.1
Ověřte, že složka lib v adresáři JavaFX obsahuje potřebné .jar soubory.

3. **Nastavení projektu v IntelliJ IDEA**
Otevřete projekt v IntelliJ IDEA:
Pokud ještě nemáte projekt otevřený, spusťte IntelliJ IDEA a otevřete složku vašeho projektu.

Nastavte JDK:

Přejděte na File > Project Structure > Project.
Ujistěte se, že jako Project SDK máte vybraný JDK (např. Amazon Corretto 11 nebo vyšší).
Přidejte JavaFX knihovny:

Přejděte na File > Project Structure > Libraries.
Klikněte na + > Java a vyberte složku lib z JavaFX SDK, kterou jste stáhli (např. C:\javafx-sdk-23.0.1\lib).
Potvrďte kliknutím na OK.

4. **Spuštění Maven buildu**
Otevřete terminál (buď v IntelliJ IDEA nebo samostatný).
Ujistěte se, že Maven má přístup ke všem závislostem:
bash

mvn clean install
Pokud je vše nastaveno správně, Maven stáhne všechny potřebné knihovny a připraví aplikaci ke spuštění.

5. **Konfigurace spuštění v IntelliJ IDEA**
Vytvořte novou konfiguraci pro spuštění aplikace:

Otevřete Run > Edit Configurations....
Klikněte na + > Application.
Vyplňte následující údaje:
Name: WeatherDashboard
Main class: ui.WeatherApp
VM options:
text

--module-path "C:\javafx-sdk-23.0.1\lib" --add-modules javafx.controls
Working directory: Složka vašeho projektu.
Uložte konfiguraci kliknutím na OK.

▶️ **Spuštění aplikace**
Spusťte aplikaci pomocí Run nebo klávesové zkratky (např. Shift + F10).
Po spuštění zadejte název města do textového pole.
Klikněte na tlačítko Vyhledat.
Výsledky o počasí se zobrazí přímo v aplikaci.
