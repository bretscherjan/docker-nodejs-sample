# ToDo-Application mit Git, Docker und node.js 🐋

<br>

## Projektbeschreibung

In diesem Projekt wird mit node.js eine Programm ausgeführt, mit dem man eine ToDo-Liste erstellen kann und die Inhalte abkreuzen, die man bereits erledigt hat.

### Repository Clone

- SSH Link aus GitHub kopieren

- Kommandozeile öffnen (cmd)

- Aufs Verzeichnis mit dem richtigen Ordner Navigieren(C:\Daten\020_ZLI\010_projects\010_ToDoApplication) mit ```cd Path/docker-nodejs-sample```

- Mit befehl ```git clone ssh://username@host.xz/absolute/path/to/repo.git/``` Clone auf lokalen Rechner

### Docker-Konfiguration & -Installation

- Dockerdesktop-Installation für Intel (Docker Desktop for Windows - x86_64)

- Docker init in richtigem Verzeichnis in der cmd ausführen ```docker init```

- Fragen werden dargestellt wie unten. Mit den Angaben von unten ausfüllen:
```
? What application platform does your project use? Node
? What version of Node do you want to use? 18.0.0
? Which package manager do you want to use? npm
? What command do you want to use to start the app: node src/index.js
? What port does your server listen on? 3000
```

- ```docker compose up --build``` führt die Installation aus.

### Notwendige Pakete Installieren

Mit dem Befehl ```docker init``` werden automatisch diese Dateien installiert:
- `dockerignore`
- `Dockerfile`
- `compose.yaml`
- `README.Docker.md`

Ausserdem werden mit dem Befehl auch diese wichtigen Pakete im package.json installiert:

- `express`
- `pg`
- `sqlite3` (Version 5.0.0 ältere Version als defauld, sonst funktioniert nicht)
- `uuid`
- `wait-port`

### Application in Dockerconatainer Starten

- mit der Adresse [localhost:3000](http://localhost:3000/) kann man die Anwendung starten
<img src="images/Screenshot 2024-09-20 112934.png" alt="ToDo-Liste" width="550"/>

## Links

[Git Repository](https://github.com/bretscherjan/docker-nodejs-sample)
[Docker Anleitung](https://docs.docker.com/guides/language/nodejs/containerize/)