### **Stap 1: Download het compose.yaml-bestand**

Klik op het compose.yaml bestand hierboven, download dan het bestand (zie afbeelding)

![image](https://i.imgur.com/7h1X4Xt.png)


Klik vervolgens op de "Download" knop om het bestand op je computer op te slaan.

### **Stap 2: Installeer Docker Desktop**
Voordat je SQL Server in Docker kunt uitvoeren, moet je Docker Desktop installeren op je Windows- of macOS-computer. Ga naar de officiële Docker-website en download Docker Desktop voor jouw besturingssysteem:

- Voor Windows: [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/)
- Voor macOS: [Docker Desktop for Mac](https://docs.docker.com/desktop/install/mac-install/)

### **Stap 3: Open Docker Desktop**
Na de installatie open je Docker Desktop. Zorg ervoor dat het correct is opgestart en actief is.

### **Stap 4: Gebruik Docker via de Terminal**
Open een terminalvenster op je computer (dit kan PowerShell op Windows of Terminal op macOS zijn).

Navigeer naar de locatie waar je het "compose.yaml" bestand hebt gedownload met behulp van het `cd`-commando. Bijvoorbeeld:

```
cd pad/naar/compose.yaml
```

Gebruik vervolgens de volgende Docker-opdrachten om SQL Server in Docker te beheren:

- Om SQL Server op te starten, voer je uit:

```
docker-compose up
```

Dit zal SQL Server starten op basis van de configuratie in het "compose.yaml" bestand (je moet dus in de map zitten waar het compose.yaml bestand staat).

- Om SQL Server te stoppen (zonder de containers te verwijderen, je behoudt dus de data in je database), voer je uit:

```
docker-compose stop
```

- Om SQL Server en de bijbehorende containers volledig te verwijderen, voer je uit (al je database data is dan weg):

```
docker-compose down
```

**Let op:** Zorg ervoor dat je in de map bent waarin het "compose.yaml" bestand zich bevindt voordat je de bovenstaande Docker-opdrachten uitvoert.

Dit zijn de basisstappen om SQL Server in Docker uit te voeren met behulp van jouw "compose.yaml" bestand. Studenten kunnen deze stappen volgen om aan de slag te gaan met SQL Server in een gecontaineriseerde omgeving.



**Stap 5: Verbinden met SQL Server via Azure Data Studio**

Nu je SQL Server succesvol in Docker hebt gestart, kun je verbinding maken met de database met behulp van Azure Data Studio, een krachtige tool voor databaseontwikkeling en -beheer. Hier is hoe je dat kunt doen:

1. **Download en Installeer Azure Data Studio**:

   Ga naar de officiële website van Azure Data Studio en download de versie die overeenkomt met je besturingssysteem (Windows, macOS, of Linux):

   [Azure Data Studio Download](https://docs.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio)

   Volg de installatie-instructies om Azure Data Studio op je computer te installeren.

2. **Open Azure Data Studio**:

   Start Azure Data Studio na de installatie. Als het voor de eerste keer wordt gestart, kan het zijn dat je enkele basisinstellingen moet configureren, zoals thema en taal.

3. **Verbind met SQL Server**:
![image](https://i.imgur.com/I10UbG4.png)
   In Azure Data Studio kun je nu een nieuwe verbinding maken met de SQL Server die in Docker draait. Volg deze stappen:

   a. Klik op "New Connection" (Nieuwe verbinding) in het zijpaneel

   b. Vul de volgende informatie in:

      - **Server**: localhost
      - **Authentication Type**: SQL Login
      - **Username**: sa
      - **Password**: Grasmaaier99!
      - **Trust Server Certificate**: true

   c. Klik op "Connect" (Verbinden) om verbinding te maken met SQL Server.
   
    

4. **Verkennen van de Database**:

   Zodra je bent verbonden, kun je de databases en objecten in SQL Server verkennen en query's uitvoeren met behulp van Azure Data Studio.

Nu ben je klaar om met SQL Server in Docker te werken via Azure Data Studio. Deze krachtige combinatie biedt een geweldige omgeving voor het ontwikkelen en beheren van databases. Veel succes met je databaseproject!
