# Automatizace schvalování dovolené pomocí Power Automate

Tento projekt demonstruje proces automatizace schvalování dovolené ve firmě pomocí Microsoft Power Automate a integrace se SharePoint. Projekt zahrnuje popis všech kroků od vyplnění žádosti zaměstnancem až po schválení nebo zamítnutí žádosti nadřízeným.

## Struktura repozitáře

### Složky a soubory

- `Postup řešení/`  
  Obsahuje dokumentaci k celému postupu implementace automatizace schvalování dovolené.
  
  - `1. Vyplnění formuláře/`  
    Obsahuje soubory vztahující se k prvnímu kroku, kde zaměstnanec vyplňuje formulář žádosti o dovolenou.
    
  - `2. SharePoint - Čeká na vyřízení/`  
    Popisuje stav, kdy žádost čeká na schválení a je uložena na SharePoint.
    
  - `3. Přijetí e-mailu nadřízeným/`  
    Tento krok zahrnuje přijetí e-mailu nadřízeným s notifikací o nové žádosti o dovolenou.
    
  - `4. Schválení dovolené nadřízeným/`  
    Popisuje proces, kdy nadřízený schválí žádost o dovolenou.
    
  - `5. Zaměstnanec obdrží kladné vyjádření/`  
    Tento krok zahrnuje notifikaci zaměstnanci o schválení jeho dovolené.
    
  - `6. SharePoint - Schváleno/`  
    Aktualizace stavu žádosti na SharePointu na "Schváleno".
    
  - `7. Zaměstnanec obdrží záporné vyjádření/`  
    Tento krok zahrnuje notifikaci zaměstnanci o zamítnutí jeho dovolené.
    
  - `8. SharePoint - Zamítnuto/`  
    Aktualizace stavu žádosti na SharePointu na "Zamítnuto".

- `Power Automate setup/`  
  Obsahuje konfiguraci Power Automate flow a další související soubory.

  - `flow-src/`  
    Zdrojové soubory pro Power Automate flow.
    
    - `Schéma flow.PNG`  
      Schéma, které znázorňuje průběh automatizovaného procesu.
      
    - `Vyřízený požadavek - tělo e-mailu se změní.PNG`  
      Ukázka, jak se změní obsah e-mailu po vyřízení žádosti.
    
  - `Microsoft.Flow/flows/`  
    Složka obsahující Microsoft Flow konfiguraci.

- `README.md`  
  Soubor s popisem struktury flow.

- `manifest.json`  
  Konfigurační soubor pro Microsoft Power Automate.

### Další poznámky

Tento projekt je postaven na integraci se SharePoint a Power Automate, což umožňuje automatizované workflow pro schvalování žádostí o dovolenou v rámci firmy. Každý krok procesu je detailně dokumentován v jednotlivých složkách repozitáře.
