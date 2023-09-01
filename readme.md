**Stap 1: Download het compose.yaml-bestand**

Ga naar de volgende GitHub-pagina: [GitHub Repository](https://github.com/DuxSec/sql-server-docker/blob/main/compose.yaml).

![Imgur](https://imgur.com/7h1X4Xt)


Klik vervolgens op de "Download" knop om het bestand op je computer op te slaan.

**Stap 2: Installeer Docker Desktop**
Voordat je SQL Server in Docker kunt uitvoeren, moet je Docker Desktop installeren op je Windows- of macOS-computer. Ga naar de officiële Docker-website en download Docker Desktop voor jouw besturingssysteem:

- Voor Windows: [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/)
- Voor macOS: [Docker Desktop for Mac](https://docs.docker.com/desktop/install/mac-install/)

**Stap 3: Open Docker Desktop**
Na de installatie open je Docker Desktop. Zorg ervoor dat het correct is opgestart en actief is.

**Stap 4: Gebruik Docker via de Terminal**
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

Dit zal SQL Server starten op basis van de configuratie in het "compose.yaml" bestand.

- Om SQL Server te stoppen (zonder de containers te verwijderen), voer je uit:

```
docker-compose stop
```

- Om SQL Server en de bijbehorende containers volledig te verwijderen, voer je uit:

```
docker-compose down
```

**Let op:** Zorg ervoor dat je in de map bent waarin het "compose.yaml" bestand zich bevindt voordat je de bovenstaande Docker-opdrachten uitvoert.

Dit zijn de basisstappen om SQL Server in Docker uit te voeren met behulp van jouw "compose.yaml" bestand. Studenten kunnen deze stappen volgen om aan de slag te gaan met SQL Server in een gecontaineriseerde omgeving.








