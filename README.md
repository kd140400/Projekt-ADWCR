# Projekt-ADWCR

Kroki:
1. Zainstalować Kafkę https://archive.apache.org/dist/kafka/3.5.1/kafka_2.13-3.5.1.tgz
2. Otworzyć wiersz poleceń nr 1
3. Wejść do folderu kafka - np. "cd C:\kafka\kafka_2.13-3.7.0"
4. Uruchomić Zookeeper - w wierszu poleceń nr 1 wpisać "bin\windows\zookeeper-server-start.bat config\zookeeper.properties"
5. Otworzyć wiersz poleceń nr 2
6. Uruchomić Kafkę - w wierszu poleceń nr 2 wpisać "bin\windows\kafka-server-start.bat config\server.properties"
7. Otworzyć wiersz poleceń nr 3
8. Sprawdzić, czy Kafka działa - w wierszu poleceń nr 3 wpisać "bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092", jeśli temat "hydro2" nie istnieje - utworzyć go - w wierszu poleceń nr 3 wpisać "bin\windows\kafka-topics.bat --create --topic hydro2 --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1"
9. Uruchomić kod producnta
10. Uruchomić kod konsumenta
11. Dane zapisują się w pliku CSV pn. "hydro2_dane"
