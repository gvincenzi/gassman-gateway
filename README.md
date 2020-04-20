# GasSMan - Gateway
## Technical Scope
GAS (Gruppo di Acquisto Solidale) Sales Management è un sistema Java basato su un'architettura MicroServices che alimenta due interfacce attraverso dei servizi REST : un bot di Telegram e un'interfaccia di amministrazione.
GasSMan ha come scopo quello di fornire ad un amminstratore di un GAS un'interfaccia per configurare la lista dei prodotti in distribuzione, e un bot grazie al quale gli inscritti possono consultare l'elenco dei prodotti disponibili ed effettuare gli ordini.

## Didactical Scope
Questo repository è un modulo di un progetto Java di esempio descritto nel libro (scritto in lingua italiana) **"Anche i microservizi nel loro piccolo s'incazzano - Guida alla comprensione dei principi di un'architettura in microservizi"** di [Giuseppe Vincenzi](https://gvincenzi.tumblr.com/).

## Technologies
Technologies used in this module of the project:
- Spring Boot
- Netflix Eureka Server
- Netflix Zuul
- Netflix Hystrix
- Maven

## Installation
### Start GasSMan - Gateway
Per lanciare il modulo e il server Eureka, basterà lanciare un comando install in MAVEN e, dopo aver posizionato il jar dove più conviene nel vostro file system, potrete lanciare il comando :

```
java -jar gassman-gateway-1.0.0.jar
```

Questo servizio deve essere lanciato con un Eureka Server già attivo e in ascolto, secondo quanto configurato nel file di properties (application.yml), sulla porta 8880.
Dopo aver correttamente lanciato questo modulo, potrete dunque andare sull'interfaccia di Eureka Server all'indirizzo http://localhost:8880 e verificare che il servizio gassman-gateway-service è presente nella lista dei servizi attivi.

## Build Information
**Travis Ci page** : [Click here to view build history](https://travis-ci.org/gvincenzi/gassman-gateway)

**Last build** : <img src="https://travis-ci.org/gvincenzi/gassman-gateway.svg?branch=master" alt="last build satus">
