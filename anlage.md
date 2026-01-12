# Vertragsanlage zum Service-Level-Agreement (SLA)

Diese Anlage gilt nur in Verbindung mit dem Service-Level-Agreement in der jeweils zwischen den Parteien vereinbarten Fassung mit demselben Stand.

Stand: 01. Januar 2026 (maßgeblich ist das Service-Level-Agreement mit demselben Stand)  
Auftraggeber: Example GmbH, Beispiellstraße 1, 12345 Berlin  
Auftragnehmer: Blunix GmbH, Glogauer Straße 21, 10999 Berlin

Das Git-Repository dieser Anlage ist gehostet unter: https://git.example.com/contracts/blunix-sla-anlage  

Das Playbook-Git-Repository ist gehostet unter: https://git.example.com/infrastructure/playbook-infrastructure-example-13

Tickets für die Infrastruktur: https://git.example.com/infrastructure/playbook-infrastructure-example-13/issues

Notfall-Rufnummer: 030 / 123 456 789  

Allgemeiner Chat-Raum (laufende Kommunikation): #example-chat:matrix.org  
Technischer Monitoring-Chat-Raum (Alarmierungen technisches Monitoring): #example-monitoring-tech:matrix.org  
SLA-Monitoring-Chat-Raum (Alarmierungen SLA-Monitoring und Verfügbarkeitsziele): #example-monitoring-sla:matrix.org

SLA Monitoring Dashboard: https://sla.monitoring.cus.pm

Technisches Monitoring Dashboard: https://tech.monitoring.cus.pm

## Technische Ansprechpartner

Blunix GmbH (Auftragnehmer)  
- Peter Thurner - p.thurner@blunix.com - @p.thurner.blunix:matrix.org

Example GmbH (Auftraggeber)  
- Max Mustermann - m.mustermann@example.com - 0175 / 123 456 79 - @m.mustermann.example:matrix.org  
- Emil Mustermann - e.mustermann@example.com - 0176 / 123 456 789 - @e.mustermann.example:matrix.org

## Gebuchte Reaktionszeiten (SLA 5.1)

Weitere Regelungen vgl. SLA Ziffer 5.1

| Zeitfenster                           | Gebuchte Reaktionszeit | Monatspauschale (netto) |
|---------------------------------------|------------------------:|-----------------------:|
| Werktage 10:00–20:00                  | Zwei Stunden            | 230,00 Euro            |
| Werktage 20:00–10:00                  | Zwei Stunden            | 310,00 Euro            |
| Wochenende/Feiertage 10:00–20:00      | Zwei Stunden            | 360,00 Euro            |
| Wochenende/Feiertage 20:00–10:00      | Zwei Stunden            | 450,00 Euro            |

Summe Reaktionszeit-Pauschalen pro Monat: 1.350,00 Euro netto

## Systeme

(Definitionen vgl. SLA, Ziffer 1.2. Wartungsfenster-Default vgl. SLA. Betriebs- und Wartungspauschale im Sinne von SLA Ziffer 3.2)

### Utility Stack

Pflicht-Stack für Betrieb und Administration. Keine HA-Garantie; Backups gemäß SLA-Standard, sofern nicht abweichend vermerkt.

**cus-util-prod-monitoring-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | technisches Monitoring (Überwachung interner technischer Kennzahlen und Systemzustände; keine Grundlage für die Berechnung von Verfügbarkeitszielen gemäß SLA 5.2; SLA 2.4.1) |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                       |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-monitoring-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | SLA-Monitoring (Überwachung der in dieser Anlage benannten Monitoring-Messgegenstände für Systeme, die in dieser Anlage als Produktiv-Systeme im Sinne von SLA 5.1 geführt werden und die überwacht werden sollen; einschließlich der Monitoring-Messgegenstände, die für Verfügbarkeitsziele nach SLA 5.2 maßgeblich sind; Betrieb bei einem von cus-util-prod-monitoring-1 und den übrigen Systemen abweichenden Hosting- oder Cloud-Provider; SLA 2.4.1) |
| Cloud-Provider                          | IONOS Cloud                                                                   |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-backup-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Backup-System (Primär) zur Sicherung der in dieser Anlage bezeichneten Systeme (SLA 2.4.2) |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-backup-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Backup-System (Sekundär/Failover) zur redundanten Sicherung der in dieser Anlage bezeichneten Systeme (SLA 2.4.2) |
| Cloud-Provider                          | IONOS Cloud                                                                   |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-git-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Git/Repos (Konfiguration/Docs, insbesondere Playbook-Git-Repository und Anlagen-Repository; SLA 2.4.4) |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-gitci-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | CI/CD für Playbooks/Deployments (GitLab-Runner o.Ä.; SLA 2.4.5)              |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-log-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Zentrales Log-Archiv/Viewer (SLA 2.4.3)                                      |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | keine öffentlichen TLS-Zertifikate (Zugriff nur intern/VPN)                  |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-gateway-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | VPN/Bastion/Gateway für administrativen Zugriff auf die in dieser Anlage bezeichneten Systeme (SLA 2.4.6) |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | vom Auftragnehmer verwaltete Let’s-Encrypt-Zertifikate für interne/VPN-Zugänge |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-gateway-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Gateway (Sekundär/Failover) für administrativen Zugriff auf die in dieser Anlage bezeichneten Systeme (SLA 2.4.6) |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 0,00 Euro (technisch im Wesentlichen identisch zu cus-util-prod-gateway-1; Pauschale dort berücksichtigt) |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | vom Auftragnehmer verwaltete Let’s-Encrypt-Zertifikate für interne/VPN-Zugänge |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


**cus-util-prod-deploy-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Deploy-/Release-Orchestrierung (SLA 2.4)                                     |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| Verfügbarkeitsziel (SLA 5.2)            | keines                                                                        |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Ja                                                                            |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Nein                                                                          |


Summe Betriebs- und Wartungspauschalen Utility Stack pro Monat: 400,00 Euro netto

Produktiv-Systeme für Notfallreaktionszeiten: Nein

### Produktivsysteme

#### cus-tool-prod-matomo-1

**cus-tool-prod-matomo-1**  

| Parameter                                   | Wert                                         |
|---------------------------------------------|----------------------------------------------|
| Zweck                                       | Debian 13, VM; Matomo Web-Analytics (Produktion) |
| Cloud-Provider                              | Hetzner Cloud                                |
| Produktiv-System für Notfallreaktionszeiten | Nein                                         |
| Verfügbarkeitsziel (SLA 5.2)                | keines                                       |
| Monitoring (SLA 2.4.1)                      | Dashboard siehe Kopfbereich dieser Anlage    |
| Wartungsfenster-Override (SLA 5.3)          | keiner (Default)                             |
| Betriebs- und Wartungspauschale (SLA 3.2)   | 50,00 Euro                                      |
| Backups (SLA 2.4.2)                         | keine Abweichungen                           |
| TLS-Zertifikate (SLA 4.2.9)                 | Let’s Encrypt                                |
| Automatische apt Versionsupdates (SLA 4.2.4)    | Ja                                           |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Ja                                                         |
| Backup- und DR-Testläufe (SLA 4.5)          | Nein                                         |


#### cus-www-prod-web cluster

Verfügbarkeitsziel, Monitoring-Messobjekt, Messintervall, Toleranzen und Monitoring-Dashboard werden für jedes nachfolgend bezeichnete System gesondert ausgewiesen.


**cus-www-prod-lb-1**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VM; Loadbalancer/Reverse Proxy (Produktion)                       |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - HTTPS https://app.example.com/health -> HTTP-Status 200<br>- Gültigkeit des öffentlichen TLS-Zertifikats für app.example.com |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-lb-1                        |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro                                                                     |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| TLS-Zertifikate (SLA 4.2.9)             | vom Auftraggeber bereitgestellte TLS-Zertifikate                             |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |


**cus-www-prod-lb-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VM; Loadbalancer/Reverse Proxy (Produktion, Failover)             |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - HTTPS https://app.example.com/health -> HTTP-Status 200<br>- Gültigkeit des öffentlichen TLS-Zertifikats für app.example.com |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-lb-2                        |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 0,00 Euro (technisch identisch zu cus-www-prod-lb-1; Pauschale dort berücksichtigt) |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| TLS-Zertifikate (SLA 4.2.9)             | vom Auftraggeber bereitgestellte TLS-Zertifikate                             |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |


**cus-www-prod-web-1, cus-www-prod-web-2, cus-www-prod-web-3, cus-www-prod-web-4**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VMs; Web-Applikationsserver (Produktion)                          |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - HTTP-Health-Checks auf die von den Loadbalancern weitergeleiteten Backends<br>- HTTP-Aufruf http://localhost/health auf jedem Web-Node |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-web-1                       |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 100,00 Euro (für alle vier Systeme zusammen)                                   |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| TLS-Zertifikate (SLA 4.2.9)             | terminieren am Loadbalancer (keine direkten öffentlichen TLS-Zertifikate)    |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |


**cus-www-prod-db-1, cus-www-prod-db-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VMs; Datenbank-Cluster (Produktion)                               |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - TCP-Verbindung auf den Datenbankport des primären Cluster-Knotens<br>- erfolgreiche Ausführung einer einfachen Leseabfrage (z.B. SELECT 1 auf einer Healthcheck-Tabelle) |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-db-1                        |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 100,00 Euro (für beide Systeme zusammen)                                       |
| Backups (SLA 2.4.2)                     | zusätzlich zum Standard stündliche Sicherungen für 1 Woche; tägliche Sicherungen für 1 Monat |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                   |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |


**cus-www-prod-nfs-1, cus-www-prod-nfs-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VMs; NFS-Storage/Shared Filesystem (Produktion)                   |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - Erreichbarkeit und Mount-Status des NFS-Exports auf Web- und Applikationsservern<br>- erfolgreicher Lesezugriff auf einen definierten Testpfad im Shared Filesystem |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-nfs-1                       |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro (für beide Systeme zusammen)                                        |
| Backups (SLA 2.4.2)                     | tägliche Sicherungen der NFS-Volumes für 30 Tage                             |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |


**cus-www-prod-redis-1, cus-www-prod-redis-2**  

| Parameter                               | Wert                                                                          |
|-----------------------------------------|-------------------------------------------------------------------------------|
| Zweck                                   | Debian 13, VMs; Redis-Cluster (Caching/Session Store, Produktion)            |
| Cloud-Provider                          | Hetzner Cloud                                                                 |
| Verfügbarkeitsziel (SLA 5.2)            | 99,95 % pro Kalendermonat                                                    |
| Messobjekt/Prüfung (SLA 5.2.1)          | - Antwort auf REDIS PING auf den virtuellen Cluster-Endpunkt<br>- erfolgreiches Setzen und Lesen eines Testschlüssels im Cluster |
| Messintervall (SLA 5.2.1)               | 60 Sekunden                                                                  |
| Toleranz (SLA 5.2.1)                    | Ausfall ab zwei aufeinanderfolgenden fehlgeschlagenen Messpunkten (abweichend vom Standard) |
| Monitoring (SLA 2.4.1)                  | Dashboard https://monitoring.cus.pm/cus-www-prod-redis-1                     |
| Wartungsfenster-Override (SLA 5.3)      | keiner (Default)                                                              |
| Betriebs- und Wartungspauschale (SLA 3.2) | 50,00 Euro (für beide Systeme zusammen)                                        |
| Backups (SLA 2.4.2)                     | keine Abweichungen                                                            |
| TLS-Zertifikate (SLA 4.2.9)             | Let’s Encrypt                                                                 |
| Automatische apt Versionsupdates (SLA 4.2.4) | Nein                                                                         |
| Automatische apt Kernel-Version-Update reboots (SLA 4.2.4) | Nein                                                         |
| Backup- und DR-Testläufe (SLA 4.5)      | Ja, alle 12 Wochen                                                            |

Produktiv-Systeme für Notfallreaktionszeiten: Ja

## Monatliche Gesamtkostenrechnung

| Position                                      | Betrag        |
|----------------------------------------------|--------------:|
| Reaktionszeit-Pauschalen (Kapitel 1)         | 1.350,00 Euro    |
| Betriebs- und Wartungspauschalen Utility Stack (Kapitel 2.1) | 400,00 Euro      |
| Betriebs- und Wartungspauschale cus-tool-prod-matomo-1       | 50,00 Euro       |
| Betriebs- und Wartungspauschalen cus-www-prod-web cluster    | 350,00 Euro      |
| Summe Betriebs- und Wartungspauschalen Produktivsysteme      | 400,00 Euro      |
| Monatliche Gesamtkosten (netto)              | 2.150,00 Euro    |
| Zzgl. Umsatzsteuer 19 %                      | 408,50 Euro      |
| Monatliche Gesamtkosten (brutto)             | 2.558,50 Euro    |
