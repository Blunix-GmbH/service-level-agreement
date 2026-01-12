# Service-Level-Agreement

Zwischen:

Example GmbH EDITME  
Beispiellstraße 1 EDITME  
12345 Berlin EDITME

Nachfolgend „Auftraggeber“ genannt, und:

Blunix GmbH  
Glogauer Straße 21  
10999 Berlin

Nachfolgend „Auftragnehmer“ genannt.

Stand:			    01. Januar 2026 EDITME  
Anlage-Link:		https://git.example.com/contracts/blunix-sla EDITME



# 1. Einleitung


## 1.1 Gegenstand und Geltungsbereich

Dieses Service Level Agreement (im Folgenden SLA) legt die Rechte und Pflichten der Vertragsparteien im Zusammenhang mit dem Betrieb, der Wartung, der Unterstützung und der Entstörung von IT-Systemen des Auftraggebers durch den Auftragnehmer fest. Es regelt Art und Umfang der in diesem SLA beschriebenen Leistungsarten des Auftragnehmers in diesen Bereichen sowie die hierfür geltenden qualitativen und organisatorischen Anforderungen und die hierfür erforderlichen Mitwirkungspflichten, Bereitstellungspflichten und Beistellpflichten des Auftraggebers. Welche der in diesem SLA beschriebenen Leistungen im Einzelfall vom Auftragnehmer zu erbringen sind, ergibt sich aus diesem SLA in Verbindung mit der Anlage.

Die Anlage zu diesem SLA ist Bestandteil des SLA. Sie legt für die dort jeweils abgebildeten Systeme des Auftraggebers fest, in welchem Umfang sie von diesem SLA erfasst werden und welche in diesem SLA vorgesehenen servicebezogenen Parameter für diese Systeme jeweils gelten.

Für die in der Anlage abgebildeten Systeme, die von diesem SLA erfasst sind, gelten ausschließlich die Regelungen dieses SLA einschließlich Anlage; die Allgemeinen Geschäftsbedingungen für Beratungs-, Support- und Notfallleistungen der Blunix GmbH finden auf diese Leistungen keine Anwendung.


## 1.2 Begriffsbestimmungen

Für dieses SLA einschließlich der zu diesem SLA gehörenden Anlage gelten die folgenden Begriffsbestimmungen:

Als System gilt eine lauffähige Installation des Betriebssystems Debian GNU/Linux, unabhängig davon, ob sie auf physischer Hardware, in einer virtuellen Maschine oder als Cloud-Instanz betrieben wird. Hypervisor-Hosts für Virtualisierung (zum Beispiel Proxmox, KVM) gelten ebenfalls als Systeme, auch wenn sie ihrerseits weitere Systeme in virtuellen Maschinen betreiben. Container, einschließlich Docker-Container und vergleichbarer Technologien, gelten nicht als individuelle Systeme sondern als auf Systemen betriebene Software.

Die Zeitzone für alle Zeitangaben in diesem SLA und der Anlage ist Europe/Berlin (CET/CEST); maßgeblich ist die jeweils am Sitz des Auftragnehmers (Berlin, Deutschland) geltende gesetzliche Zeit.

Werktage sind die Kalendertage Montag bis Freitag mit Ausnahme der gesetzlichen Feiertage am Sitz des Auftragnehmers (Berlin, Deutschland). Gesetzliche Feiertage (Berlin) sind die am Sitz des Auftragnehmers jeweils geltenden gesetzlichen Feiertage.

Das Playbook-Git-Repository bezeichnet ein vom Auftraggeber bereitgestelltes Git-Repository (in der Regel auf einem GitLab-System des Auftraggebers), in dem insbesondere Terraform- und Ansible-Configuration-Management-Code sowie betriebsrelevante Dokumentation abgelegt werden.

Infrastruktur bezeichnet die Gesamtheit der in der Anlage abgebildeten Systeme, welche mittels Configuration-Management Code im Playbook-Git-Repository erstellt und verwaltet werden, sowie deren Zusammenspiel.

Der Standardsatz bezeichnet eine Vergütung von 50,00 Euro je angefangene 30 Minuten Arbeitszeit des Auftragnehmers, soweit in diesem SLA oder der Anlage für bestimmte Leistungen keine abweichende Vergütung geregelt ist. Soweit in diesem SLA oder der Anlage nichts anderes angegeben ist, verstehen sich alle genannten Vergütungen und Entgelte zuzüglich gesetzlicher Umsatzsteuer.


## 1.3 Technische Ansprechpartner

Technischer Ansprechpartner des Auftragnehmers für dieses SLA ist:

Name: Max Mustermann EDITME  
Telefon: +49 30 / 123 456 789 EDITME  
E-Mail: m.mustermann@blunix.com EDITME

Der Auftraggeber benennt mindestens einen technischen Ansprechpartner, der mit den in der Anlage abgebildeten Systemen und den darauf betriebenen Anwendungen vertraut ist und dem Auftragnehmer als fachlicher Ansprechpartner für technische Rückfragen sowie für Änderungs- und Erweiterungswünsche zur Verfügung steht. Die technischen Ansprechpartner des Auftraggebers werden in der Anlage benannt; Änderungen der technischen Ansprechpartner erfolgen durch Anpassung der Anlage gemäß Ziffer 3.1. Fällt ein in der Anlage benannter technischer Ansprechpartner dauerhaft weg (insbesondere durch Ausscheiden aus dem Unternehmen, längere Abwesenheit oder Wegfall der Zuständigkeit), verpflichtet sich der Auftraggeber, unverzüglich einen Ersatz zu benennen und die Anlage entsprechend gemäß Ziffer 3.1 anzupassen.

Die technischen Ansprechpartner des Auftraggebers werden in der Anlage mit E-Mail-Adresse, Chat-Kennung und Mobilfunknummer aufgeführt und dienen als technische Ansprechpartner bei Störungen und Notfällen.

Der Auftraggeber stellt sicher, dass der benannte technische Ansprechpartner über die fachliche und technische Kompetenz verfügt, um die in diesem SLA und in der Anlage beschriebenen Anforderungen zu verstehen und die dort vorgesehenen Mitwirkungs- und Freigabepflichten zu erfüllen.

## 1.4 Kommunikation

Formgebundene Erklärungen im Zusammenhang mit diesem SLA (insbesondere Kündigungen, Fristsetzungen und sonstige rechtserhebliche Erklärungen) sind in Textform per E-Mail abzugeben. Erklärungen an den Auftragnehmer sind an legal@blunix.com, Erklärungen an den Auftraggeber an m.mustermann@example.com EDITME zu richten. Für die Einhaltung von Fristen ist der Zeitpunkt maßgeblich, zu dem die E-Mail den Mailserver der jeweils anderen Vertragspartei erreicht und mit SMTP 250 OK angenommen wird.

Änderungswünsche in Bezug auf die Anlage nach Ziffer 3.1 werden durch Issues sowie Pull-/Merge-Requests in dem in der Anlage bezeichneten Git-Repository der Anlage kommuniziert; zusätzlich sind die in der Anlage benannten technischen Ansprechpartner des Auftraggebers hierüber per E-Mail zu informieren. Ergänzend gelten die Regelungen in Ziffer 3.1.

Änderungswünsche, technische Abstimmungen, Erweiterungswünsche und sonstige fachliche Anforderungen im Zusammenhang mit den von diesem SLA und der Anlage erfassten Systemen und Leistungen werden über Issues im Playbook-Git-Repository erfasst und nachverfolgt. Das Playbook-Git-Repository ist so zu konfigurieren, dass das Anlegen, Ändern und Updaten von Issues Benachrichtigungs-E-Mails an die für das Git-Repository hinterlegten Projektbeteiligten auslöst.

Sonstige laufende Kommunikation, insbesondere kurzfristige Nachfragen und allgemeine Abstimmungen, erfolgt über den in der Anlage bezeichneten allgemeinen Chat-Raum. Die Nutzung dieses Chat-Raums ersetzt weder formgebundene Erklärungen im Sinne dieses SLA noch die nach Ziffer 5.1.1 erforderliche Notfallmeldung. Die in Ziffer 5.1.1 geregelte Nutzung des SLA-Monitoring-Chat-Raums als Bestandteil einer Notfallmeldung bleibt hiervon unberührt.

Für Notfallmeldungen und die Auslösung der in Ziffer 5.1.2 beschriebenen Notfallreaktionszeiten gelten ausschließlich die Regelungen in Ziffer 5.1.1.



# 2. Technische Grundlagen und Blunix Hosting Stack


## 2.1 Vom Auftraggeber beauftragte Provider

Der Auftragnehmer stellt im Rahmen dieses SLA keine eigene Rechenzentrums-, Cloud-, Netzwerk-, Storage- oder andere Cloud-Provider Infrastruktur bereit. Dies umfasst ohne Ausnahme alle zum Betrieb der Systeme erforderlichen Ressourcen, einschließlich Rechenzentrums-, Cloud-, Netzwerk-, Storage-, DNS-, Mail- und sonstiger technischer Infrastruktur- oder Plattformdienste.

Die Auswahl dieser Anbieter, deren vertragliche Einbindung, die fortlaufende Vertragsdurchführung (insbesondere die Zahlung sämtlicher Entgelte) sowie die Einhaltung der vertraglichen und gesetzlichen Pflichten im Verhältnis zu diesen Anbietern obliegen ausschließlich dem Auftraggeber. Der Auftragnehmer übernimmt keine Gewähr für Verfügbarkeit, Leistungsumfang, Sicherheit oder Rechtskonformität der von diesen Anbietern erbrachten Leistungen; Ausfälle aus deren Verantwortungsbereich stellen keine vom Auftragnehmer zu vertretenden Ausfälle dar.

Sämtliche Systeme im Sinne der Begriffsbestimmungen nach Ziffer 1.2 werden auf durch den Auftraggeber beauftragten Cloud- oder Hosting-Anbietern betrieben, die von durch den Auftraggeber beauftragten Dritten zur Verfügung gestellt wird. Alternativ kann der Auftraggeber eine eigene In-House Server-Infrastruktur bereitstellen, wobei die Wartung dieser durch den Auftraggeber oder durch ihn beauftragte Dritte erfolgt. Der Auftragnehmer erbringt keine Vor-Ort-Hardwareleistungen und schuldet keine Hardware‑Expertise; Hardwarediagnose und ‑reparatur vor Ort sind nicht Gegenstand dieses SLA. Der Auftragnehmer unterstützt den Auftraggeber jedoch im Rahmen der vereinbarten Leistungen bei der Fehleranalyse und Eingrenzung von Störungen und wirkt bei der Abstimmung und der technischen Kommunikation mit dem jeweiligen Provider mit.

Der Auftraggeber stellt sicher, dass die von ihm gewählten Provider die zur Leistungserbringung nach diesem SLA erforderlichen technischen Voraussetzungen erfüllt und dem Auftragnehmer die in Ziffer 6.3 beschriebenen administrativen Zugriffsrechte eingeräumt werden.


## 2.2 Playbook-Git-Repository

Das in Ziffer 1.2 definierte Playbook-Git-Repository dient als zentrale, versionierte Arbeitsgrundlage für die Konfiguration und den Betrieb der in der Anlage abgebildeten Systeme. Es enthält insbesondere Infrastrucure-As-Code Konfigurationen zur Erstellung der Systeme mit deren jeweiligen Cloud- oder Hosting-Providern sowie die Ansible-Konfigurationen wie Playbooks, Rollen-Einbindungen, Inventories und Variablen, die für Aufbau, Änderung und Wiederaufbau der Infrastruktur erforderlich sind.

Soweit technisch möglich, nimmt der Auftragnehmer Konfigurations- und Betriebsänderungen an den von ihm betreuten Systemen vorrangig über den im Playbook-Git-Repository verwalteten Ansible-Code vor. Unmittelbare, nicht über das Playbook nachvollzogene Eingriffe auf Systemebene (zum Beispiel Notfallmaßnahmen per SSH) werden im Anschluss – soweit die Änderungen dauerhaft bestehen bleiben sollen – im Playbook-Git-Repository nachgezogen.

Der Auftraggeber weist sein technische Mitarbeiter an, Änderungen an den Systemen grundsätzlich über das Playbook‑Git‑Repository vorzunehmen und manuelle Eingriffe auf den Systemen nur dann durchzuführen, wenn diese zur unverzüglichen Behebung einer Störung erforderlich sind. Erfolgen manuelle Änderungen, hat der Auftraggeber hierfür unverzüglich ein Issue im Playbook‑Git‑Repository zu eröffnen und die Änderungen dort zu dokumentieren bzw. nachzuziehen.

Der Auftragnehmer ist berechtigt, Konfigurationsänderungen jederzeit auf Grundlage des im Playbook-Git-Repository verwalteten Stands auszurollen. Berücksichtigt werden ausschließlich Änderungen, die über einen Pull-/Merge-Request im Playbook-Git-Repository eingebracht und einem technischen Ansprechpartner des Auftragnehmers zugewiesen wurden. Manuelle Änderungen des Auftraggebers oder seiner Mitarbeiter werden vorab nicht geprüft und können jederzeit überschrieben oder zurückgesetzt werden. Für hieraus resultierende Ausfälle oder Beeinträchtigungen übernimmt der Auftragnehmer keine Haftung; im Übrigen gelten die Haftungsregelungen in Ziffer 8.


## 2.3 Ansible-Rollen

Der Auftragnehmer stellt unter der GitHub-Organisation „Blunix-GmbH“ (https://github.com/Blunix-GmbH/) Ansible-Rollen bereit, die für den Aufbau und Betrieb der vom Auftragnehmer betreuten Systeme genutzt werden. Diese Rollen werden während der Laufzeit dieses SLA vom Auftragnehmer gepflegt und – soweit für den sicheren und stabilen Betrieb der in der Anlage abgebildeten Systeme erforderlich – angepasst oder erweitert.

Die Bereitstellung und Erreichbarkeit der über GitHub veröffentlichten Ansible‑Rollen hängt von der Verfügbarkeit der Plattform GitHub ab. Für Ausfälle, Einschränkungen oder Störungen bei GitHub übernimmt der Auftragnehmer keine Verantwortung; daraus resultierende Verzögerungen oder Beeinträchtigungen begründen keine Haftung des Auftragnehmers. Im Übrigen gelten die Haftungsregelungen in Ziffer 8.

Der konkrete Einsatz der Ansible-Rollen für die Systeme des Auftraggebers ergibt sich aus dem im Playbook-Git-Repository hinterlegten Ansible-Code und den Festlegungen in der Anlage.

Der Auftragnehmer kann für den Auftraggeber kundenspezifische Code entwickeln, zum Beispiel Ansible-Rollen zur Abbildung individueller Anwendungen oder Infrastrukturkomponenten. In diesem Fall entscheidet der Auftraggeber, ob der Auftragnehmer diesen Code in unter seiner GitHub-Organisation veröffentlichen darf.


## 2.4 Utility-Stack

Der „Utility-Stack“ besteht aus Ansible-Rollen des Auftragnehmers nach Ziffer 2.3 sowie den hierzu im Playbook-Git-Repository nach Ziffer 2.2 hinterlegten Konfigurationen. Er dient als Hosting-Toolkit, mit dem nach der professionellen Einschätzung des Auftragnehmers die für den Hosting-Betrieb erforderlichen Basisdienste bereitgestellt werden.

Zum Utility-Stack gehören, sofern nicht in der Anlage abweichend festgelegt, die folgenden Systeme:

EDITME
| System | Beschreibung |
|---|---|
| EDITME cus-util-prod-monitoring-1 | Monitoring-Server für technisches Monitoring |
| EDITME cus-util-prod-monitoring-2 | Monitoring-Server für SLA-relevantes Monitoring |
| EDITME cus-util-prod-backup-1 | Primärer Backup-Server |
| EDITME cus-util-prod-backup-2 | Sekundärer Backup-Server mit von EDITME cus-util-prod-backup-1 abweichender Backup-Software sowie Hosting- oder Cloud-Provider |
| EDITME cus-util-prod-log-1 | Zentraler Log Server |
| EDITME cus-util-prod-gateway-1 | VPN-Server |
| EDITME cus-util-prod-gateway-2 | Sekundärer VPN-Server |
| EDITME cus-util-prod-git-1 | optionaler GitLab-Server (oder Auftragnehmer nutzt Github) |
| EDITME cus-util-prod-gitci-1 | Optionale GitLab-Runner (mehrere möglich) |
| EDITME cus-util-prod-deploy-1 | Optionaler Deploy-Server für das playbook-git-repository |

Welche dieser Systeme betrieben werden, ergibt sich aus der Anlage.

### 2.4.1 Monitoring-System

Der Auftragnehmer richtet für die in der Anlage abgebildeten Systeme im vertraglich vereinbarten Umfang zwei Monitoring-Tools ein:

- ein technisches Monitoring-Tool auf dem in der Anlage als „cus-util-prod-monitoring-1“ EDITME abgebildete System zur Überwachung interner technischer Kennzahlen und Systemzustände (z.B. CPU-Last, Arbeitsspeicher- und Plattenauslastung) und
- ein SLA Monitoring-Tool auf dem in der Anlage als „cus-util-prod-monitoring-2“ EDITME abgebildete System zur Überwachung der in der Anlage benannten Monitoring-Messgegenstände für Systeme, die in der Anlage als „Produktiv-System: Ja“ geführt werden und die der Auftraggeber gemäß Anlage überwachen lässt (einschließlich, aber nicht beschränkt auf die Monitoring-Messgegenstände, die für Verfügbarkeitsziele nach Ziffer 5.2 maßgeblich sind); dieses System wird bei einem von cus-util-prod-monitoring-1 EDITME abweichenden Hosting- oder Cloud-Provider betrieben; eine Übereinstimmung mit dem für cus-util-prod-backup-2 EDITME genutzten Hosting- oder Cloud-Provider ist zulässig.

Verweise auf die Monitoring-Dashboards des technischen Monitoring-Tools und des SLA Monitoring-Tools werden in der Anlage aufgeführt.

Das technische Monitoring-System wird nach bestem fachlichen Ermessen des Auftragnehmers eingerichtet, gewartet und betrieben. 

Alarmierungen aus dem technischen Monitoring erfolgen an den in der Anlage benannten technischen Monitoring-Chat-Raum.

Der Auftragnehmer prüft kritische Alamierungen des technischen Monitoring-Tools nach Möglichkeit zeitnah und reagiert darauf nach fachlichem Ermessen; hierdurch wird jedoch keine Notfallmeldung im Sinne von Ziffer 5.1.1 ersetzt. Notfälle sind ausschließlich nach Maßgabe des Meldewegs gemäß Ziffer 5.1.1 zu melden.

Für Systeme, für die in der Anlage Verfügbarkeitsziele im Sinne von Ziffer 5.2 festgelegt sind, werden die dort beschriebenen Monitoring-Messgegenstände, Erfolgskriterien, Messintervalle, Toleranzschwellen in der Anlage abgebildet, anschließend in das Playbook-Git-Repository überführt und auf das SLA Monitoring-Tool angewendet. Für alle übrigen Systeme, die in der Anlage als „Produktiv-System: Ja“ geführt werden, erfolgt die Festlegung und Anpassung der Monitoring-Messgegenstände, Erfolgskriterien, Messintervalle und Toleranzschwellen unmittelbar im Playbook-Git-Repository. Änderungen an diesen Parametern erfolgen mittels Pull-/Merge-Requests; sie gelten als abgestimmt, wenn sie von einem in der Anlage als technisch verantwortlich benannten Ansprechpartner des Auftraggebers freigegeben wurden. Systeme, die in der Anlage als „Produktiv-System: Nein“ geführt werden, werden nicht im SLA Monitoring-System geführt.

Alarmierungen aus dem SLA-Monitoring erfolgen an den in der Anlage benannten SLA Monitoring-Chat-Raum.

Kritische Alarmierungen aus dem SLA Monitoring-Tool werden innerhalb der in der Anlage gebuchten Notfallreaktionszeiten vom Auftragnehmer geprüft und nach fachlichem Ermessen bearbeitet; hierdurch wird jedoch keine Notfallmeldung im Sinne von Ziffer 5.1.1 ersetzt. Notfälle sind ausschließlich nach Maßgabe des Meldewegs gemäß Ziffer 5.1.1 zu melden.

Für die Berechnung und den Nachweis von Service Levels, insbesondere von Verfügbarkeitszielen, sind ausschließlich die Messwerte des SLA-Monitorings auf dem System „cus-util-prod-monitoring-2“ maßgeblich. Die Messwerte des technischen Monitorings bilden keinen Nachweis über die Einhaltung oder Nichterfüllung von Service Levels, insbesondere nicht von Verfügbarkeitszielen im Sinne von Ziffer 5.2.

Technische Störungen von Drittanbietern (insbesondere Chat-, E-Mail- oder Cloud-/Rechenzentrums-Providern) können gleichwohl im Einzelfall zu verzögerten oder ausbleibenden Alarmierungen führen. Weitergehende Ansprüche ergeben sich hieraus nur im Rahmen der Ziffer 8.


### 2.4.2 Backup-Systeme

Der Auftragnehmer richtet auf den in der Anlage als „cus-util-prod-backup-1“ EDITME und „cus-util-prod-backup-2“ EDITME abgebildete System für alle weiteren in der Anlage abgebildeten Systeme zwei voneinander unabhängige, technisch unterschiedliche Sicherungslösungen (Backup-Programme) ein, die die Sicherungen automatisiert durchführen; die beiden Sicherungslösungen werden auf zwei verschiedenen Hosting- bzw. Cloud-Providern betrieben. Daten, die nicht direkt aus dem Dateisystem gesichert werden können und daher vorab per Skript zu erzeugen werden müssen (z. B. Datenbank‑Dumps), werden von beiden Backup‑Programmen jeweils unmittelbar vor dem Sicherungslauf einmal erstellt.

Sofern in der Anlage nichts Abweichendes geregelt ist, gilt der folgende Standardsicherungsrhythmus: Es erfolgt täglich eine Sicherung zwischen 00:00 Uhr und 07:00 Uhr. Die Aufbewahrung umfasst sieben tägliche Sicherungsstände, anschließend für vier Wochen drei Sicherungsstände pro Woche und anschließend für zwölf Monate zwei Sicherungsstände pro Monat. Abweichungen hiervon werden in der Anlage je System festgelegt. Aufbewahrung bedeutet, dass die jeweiligen Sicherungsstände für Wiederherstellungszwecke vorgehalten werden. Nach Ablauf der Aufbewahrungsfristen werden die betreffenden Sicherungsstände im Rahmen der regulären System‑/Dateisystemverwaltung gelöscht; ein sicheres Überschreiben oder eine physische Vernichtung der Datenträger wird nicht geschuldet.

Wiederherstellungen kann der Auftraggeber eigenständig aus den Sicherungen durchführen; auf Wunsch übernimmt der Auftragnehmer die Wiederherstellung. Die hierfür anfallenden Leistungen des Auftragnehmers werden zum Standardsatz vergütet. Die Dauer einer Wiederherstellung hängt insbesondere von Art und Umfang der Daten, dem verwendeten Wiederherstellungsverfahren (zum Beispiel Dateisystem- oder Datenbank-Restore) sowie den verfügbaren Ressourcen der beteiligten Provider ab und liegt nicht im Einflussbereich des Auftragnehmers; feste Wiederherstellungsdauern (Recovery Time Objectives) werden nicht geschuldet. Die Wiederherstellung erfolgt auf Basis der jeweils letzten vollständig und fehlerfrei erstellten Sicherung; Datenänderungen nach diesem Zeitpunkt können verloren gehen (Recovery Point Objective).

Die ordnungsgemäße Durchführung der Sicherungsläufe wird über das nach Ziffer 2.4.1 betriebene technische Monitoring überwacht. Stellt der Auftragnehmer auf dieser Grundlage fest, dass Sicherungsläufe wiederholt fehlschlagen oder keine aktuellen Sicherungen mehr erzeugt werden, informiert er den Auftraggeber hierüber und arbeitet im Rahmen der vereinbarten Leistungen an der Behebung der Störung.

Der Auftraggeber informiert den Auftragnehmer mindestens fünf Werktage im Voraus über planbare Neuzugänge untypisch hoher Datenmengen oder sonstige Änderungen, die den Sicherungsumfang wesentlich beeinflussen (zum Beispiel Einführung datenintensiver Anwendungen oder erhebliche Vergrößerung von Datenspeichern), damit der Auftragnehmer die Sicherungskonfiguration und die Kapazitätsplanung der Sicherungslösungen entsprechend anpassen kann.

Der Auftragnehmer schuldet weder das Gelingen jeder einzelnen Sicherung noch die Wiederherstellbarkeit von Daten, soweit die Sicherung oder Konsistenz der Daten durch vom Auftraggeber zu vertretende Umstände beeinträchtigt wird. Dies gilt insbesondere für Änderungen, Fehlkonfigurationen oder Deployments an Anwendungen oder Datenbanken, die der Auftraggeber oder von ihm beauftragte Dritte außerhalb des Playbook‑Git‑Repositorys vornehmen und die der Auftragnehmer nicht kennt oder nicht prüfen kann, sowie für Störungen der vom Auftraggeber eingesetzten Infrastruktur. Im Übrigen gelten die Haftungsregelungen in Ziffer 8.

Optionale Backup- und Desaster-Recovery-Testläufe sind in Ziffer 4.5 geregelt.

### 2.4.3 Zentrales Logging System

Der Auftragnehmer betreibt auf dem in der Anlage als „cus-util-prod-log-1“ EDITME abgebildete System ein zentrales Logging-Tool zur zentralisierten Speicherung von Logdaten. Alle in der Anlage abgebildeten Systeme werden so konfiguriert, dass ihre systemd-Journal-Logs auf dem jeweiligen System selbst lokal gespeichert werden und an das zentrale Logging-Tool übertragen werden.

Der Auftraggeber kann seine Anwendungen so konfigurieren, dass diese in das systemd-Journal des jeweiligen Systems schreiben, sodass diese Logs von der beschriebenen Mechanik erfasst werden.

Das zentrale Logging System enthält im Standard keine Auswertungs-, Korrelations- oder Alarmierungsregeln; es dient ausschließlich der Sammlung und Einsicht von Logdaten durch Auftraggeber und Auftragnehmer.

Sofern in der Anlage nichts Abweichendes geregelt ist, werden Logdaten auf allen Systemen selbst sowie auf dem zentralen Logging System für 360 Tage vorgehalten. Darüber hinaus werden die Daten dieses Systems durch die nach Ziffer 2.4.2 eingerichteten Backup-Systeme gesichert; die Aufbewahrungszeiträume dieser Sicherungen ergeben sich aus Ziffer 2.4.2 sowie den hierzu in der Anlage getroffenen Festlegungen. Abweichende oder ergänzende Aufbewahrungsdauern können in der Anlage festgelegt werden.

### 2.4.4 Gitlab System

Soweit in der Anlage ein Gitlab-System „cus-util-prod-git-1“ EDITME aufgeführt ist, betreibt der Auftragnehmer darauf eine Gitlab Installation, die insbesondere das Playbook-Git-Repository nach Ziffer 2.2 und das Git-Repository der Anlage nach Ziffer 3.1 hostet. Das Gitlab System kann als Git-Hosting-Platform für weitere vom Auftraggeber genutzte und verwaltete Git-Repositories dienen. Ansible-Rollen und weiterer Code, welche der Auftragnehmer im Auftrag durch den Auftraggeber erstellt hat, können ebenfalls auf dem Gitlab System gehostet und verwaltet werden.

Der Auftraggeber verwaltet die Inhalte, Berechtigungen und Nutzerkonten der von ihm angelegten oder verwalteten Repositories eigenverantwortlich. Der Auftragnehmer installiert und aktualisiert das Gitlab‑System, kontrolliert jedoch nicht, welche Benutzer, Projekte, Repositories oder Inhalte der Auftraggeber dort anlegt oder betreibt. Der Auftragnehmer prüft Inhalte nur in den Repositories der Anlage und des Playbook‑Git‑Repositorys, soweit dies für die Erfüllung dieses SLA erforderlich ist oder gesondert beauftragt wird. Für Fehler in Programmen, Konfigurationen oder sonstigen Inhalten, die der Auftraggeber in solchen Repositories oder im Gitlab‑System verwaltet und die nicht vom Auftragnehmer erstellt oder geändert wurden, trägt der Auftraggeber die Verantwortung. Im Übrigen gelten die Haftungsregelungen in Ziffer 8.

### 2.4.5 Gitlab-Runner-Systeme

Soweit in der Anlage Gitlab-Runner-Systeme (zum Beispiel „cus-util-prod-gitci-1“ EDITME) aufgeführt sind, richtet der Auftragnehmer diese initial so ein, dass sie als Runner im Gitlab System registriert sind und für dort konfigurierte Pipelines verwendet werden können.

Der Auftraggeber ist für die inhaltliche Ausgestaltung der in Gitlab definierten Pipelines und Jobs verantwortlich, sofern er diese Pipelines und Jobs selbst eingerichtet hat und für eigene, nicht durch den Auftragnehmer verwaltete Repositories nutzt.

### 2.4.6 VPN-Gateway-Systeme

Auf den in der Anlage „cus-util-prod-gateway-1“ EDITME und „cus-util-prod-gateway-2“ EDITME abgebildeten Systemen betreibt der Auftragnehmer VPN-Gateway-Tools.

Zugriff auf sämtliche Asprekte der Infrastruktur, insbesondere administrative Zugriffe auf alle Systeme sowie sonstige Firmen-interne Dienste (zum Beispiel Gitlab, Monitoring und SSH-Zugänge, Staging-Webhosting-Umgebungen) durch Mitarbeiter des Auftraggebers und des Auftragnehmers, erfolgt grundsätzlich ausschließlich über die VPN-Gateways. Dienste die öffentlich im Internet bereitgestellt werden (zum Beispiel öffentlich erreichbare Webanwendungen des Auftraggebers), werden hiervon explizit ausgenommen.

Zugriffsberechtigte Personen und deren Rechte werden im Playbook-Git-Repository konfiguriert. Der Auftraggeber ist verpflichtet dafür zu sorgen, dass Änderungen, die die Vergabe oder Sperrung von VPN-Zugängen betreffen (insbesondere Ein- und Austritte, Rollenwechsel oder der Bedarf zur Sperrung eines bestehenden Zugangs), unverzüglich im Playbook-Git-Repository nachgeführt und dem Auftragnehmer angezeigt werden.

Besteht die Notwendigkeit der sofortigen Sperrung eines VPN-Zugangs, hat der Auftraggeber dies zusätzlich als Notfall gemäß Ziffer 5.1.1 über die dort geregelte Notfall-Rufnummer sowie per E-Mail an den technischen Ansprechpartner des Auftragnehmers zu melden.

### 2.4.7 Deploy-System

Soweit in der Anlage ein Deploy-System „cus-util-prod-deploy-1“ EDITME aufgeführt ist, kann das System genutzt werden, um von dort Ansible-Kommandos unter Verwendung des Playbook-Git-Repositorys auszuführen und damit die Infrastruktur zu verwalten.



# 3. Anlage zum SLA


## 3.1 Zweck und Funktion der Anlage

Die Anlage ist integraler Bestandteil dieses SLA. Sie dient der Abbildung der vom Auftraggeber durch den Auftragnehmer zu betreuenden Systeme sowie der für diese Systeme geltenden Parameter.

Der Vertragstext dieses SLA bildet die Grundlage für alle in der Anlage abgebildeten Systeme. Die Anlage konkretisiert für die dort abgebildeten Systeme die Anwendung der in diesem SLA vorgesehenen Leistungsarten und Parameter und kann diese – soweit in der Anlage ausdrücklich geregelt – ergänzen oder abweichend festlegen. Soweit die Anlage keine abweichende oder ergänzende Regelung trifft, gelten ausschließlich die in diesem SLA beschriebenen Regelungen.

Die Anlage wird in einem Git-Repository unter dem im Kopf dieses SLA bezeichneten Anlage-Link verwaltet; verbindlich ist die jeweils im Git-Branch „main“ gespeicherte Fassung. Änderungen der Anlage erfolgen durch Git-Pull-/Merge-Requests und werden verbindlich, sobald ein solcher Pull-/Merge-Request von der jeweils anderen Vertragspartei akzeptiert und in den Branch „main“ zusammengeführt wurde; ab diesem Zeitpunkt gelten die darin enthaltenen Regelungen als zwischen den Vertragsparteien vereinbart. Wird ein Pull-/Merge-Request nicht akzeptiert und nicht in den Branch „main“ zusammengeführt, treten die darin vorgeschlagenen Änderungen nicht in Kraft; bis zu einer erfolgreichen Zusammenführung bleibt die bisherige Fassung der Anlage maßgeblich. Die Vertragsparteien können in diesem Fall über eine angepasste Fassung der Anlage verhandeln.

Die Parteien sind sich darüber einig, dass die Freigabe eines Pull-/Merge-Requests durch eine in der Anlage als hierzu berechtigt bezeichnete Person der Schrift- und Textform genügt und einer von beiden Vertragsparteien unterzeichneten Änderungsvereinbarung gleichsteht. Die Anlage benennt für jede Partei die Personen, die zur Freigabe von Pull-/Merge-Requests befugt sind; nur von diesen Personen freigegebene Pull-/Merge-Requests entfalten Bindungswirkung.
Die Parteien stellen sicher, dass für die in der Anlage als zur Freigabe von Pull-/Merge-Requests befugten Benutzerkonten im jeweils genutzten Git-System eine Zwei-Faktor-Authentifizierung aktiviert ist. Verstöße hiergegen begründen keine Unwirksamkeit bereits freigegebener Pull-/Merge-Requests, können aber bei der Haftungsverteilung (Mitverschulden) berücksichtigt werden.

Änderungen der Anlage dürfen auf Seiten des Auftraggebers ausschließlich durch die in der Anlage benannten technischen Ansprechpartner initiiert werden, insbesondere durch das Erstellen von Pull-/Merge-Requests im hierfür vorgesehenen Git-Repository.


## 3.2 Inhalt und Struktur der Anlage

Die Anlage enthält allgemeine, nicht systemspezifische Parameter, insbesondere:

- die je Zeitfenster gebuchten Notfallreaktionszeiten nach Ziffer 5.1.2, die einheitlich für alle Systeme gelten, die in der Anlage als „Produktiv-System: Ja“ geführt werden,
- eine zusammenfassende Übersicht der sich aus den gewählten Parametern ergebenden monatlichen Pauschalen (insbesondere Reaktionszeit-Pauschalen und Betriebs- und Wartungspauschalen je System oder Systemgruppe), aus der sich der monatlich zu entrichtende Gesamtbetrag ergibt,

sowie systemspezifische Angaben für jedes in der Anlage aufgeführte System, insbesondere:

- Plattform/Zweck: Betriebssystem, Betriebsart (physische Hardware, virtuelle Maschine oder Cloud-Instanz), eingesetzter Hosting-Provider bzw. das Rechenzentrum sowie die Rolle des Systems,
- Wartungsfenster-Override: abweichende oder ergänzende Wartungsfenster nach Ziffer 5.3,
- Betriebs- und Wartungspauschale: die je System, Systemgruppe oder vergleichbarer in der Anlage bezeichneter Einheit vereinbarte monatliche Pauschalvergütung für die Einbindung in die Betriebs-, Wartungs- und Überwachungsprozesse des Auftragnehmers. Die Pauschale ist unabhängig vom im Einzelfall tatsächlich angefallenen Zeitaufwand geschuldet; ein Anspruch des Auftraggebers auf die Erbringung eines bestimmten Mindestumfangs an Wartungsleistungen oder auf Ausschöpfung eines bestimmten Zeitvolumens besteht nicht. Nicht in Anspruch genommene Wartungsleistungen werden weder gutgeschrieben noch auf andere Monate, Systeme, Systemgruppen oder Leistungsarten übertragen und können nicht auf Projektarbeiten, Incident-Bearbeitung oder sonstige Einzelleistungen angerechnet werden,
- Regelungen zu Backups: Anwendung des Standards gemäß Ziffer 2.4.2 oder abweichende bzw. ergänzende Sicherungsrhythmen und Aufbewahrungsfristen,
- gegebenenfalls vereinbarte Verfügbarkeitsziele bzw. Uptime-Garantien nach Ziffer 5.2 einschließlich der hierfür festgelegten Messobjekte, Prüfmethode, Erfolgskriterien, Messintervalle, Toleranzen und Verweise auf die zugehörigen Monitoring-Dashboards nach Ziffer 2.4.1, wie in den jeweiligen Systemzeilen der Anlage ausgewiesen,
- gegebenenfalls weitere konkretisierende Angaben zum Monitoring nach Ziffer 2.4.1,
- die Kennzeichnung, ob das System in der Anlage als „Produktiv-System: Ja“ oder „Produktiv-System: Nein“ geführt wird.

Ändern sich während eines laufenden Kalendermonats aufgrund einer gemäß Ziffer 3.1 wirksam gewordenen Änderung der Anlage die in der Anlage ausgewiesenen monatlichen Pauschalen oder sonstigen monatlichen Zuschläge (insbesondere Reaktionszeit-Pauschalen, Betriebs- und Wartungspauschalen und Verfügbarkeitszuschläge nach Ziffer 5.2.2), werden diese für den betreffenden Kalendermonat zeitanteilig nach Kalendertagen berechnet. Maßgeblich für den Beginn der Wirksamkeit der geänderten Pauschalen und Zuschläge ist das Datum der Zusammenführung des entsprechenden Pull-/Merge-Requests in den in Ziffer 3.1 bezeichneten Branch „main“.

Die Abrechnung der nach diesem SLA geschuldeten monatlichen Pauschalen und sonstigen monatlichen Zuschläge erfolgt monatlich zu Beginn des folgenden Kalendermonats per E-Mail; der Rechnungsbetrag ist innerhalb von 30 Kalendertagen nach Zugang der Rechnung zur Zahlung fällig.

Eine Verpflichtung zur Protokollierung der im Rahmen der Betriebs- und Wartungspauschale erbrachten Leistungen besteht nicht.

Die Nutzung von Infrastruktur- und Hosting-Angeboten Dritter (insbesondere Cloud-, Server- und Storage-Provider) erfolgt ausschließlich auf Rechnung und im Namen des Auftraggebers.

Die Festlegung oder Änderung der in der Anlage ausgewiesenen Monitoring-Messgegenstände, Erfolgskriterien, Messintervalle, Toleranzschwellen und Monitoring-Dashboards erfolgt in Abstimmung zwischen den Vertragsparteien. Der Auftraggeber wirkt hierbei mit, indem er die fachlichen Anforderungen benennt und die vom Auftragnehmer vorgeschlagenen Monitoring-Parameter prüft. Die endgültige Auswahl der Messgegenstände und Erfolgskriterien erfolgt durch den Auftraggeber; er trägt die Verantwortung dafür, dass diese im Hinblick auf seine fachlichen Anforderungen geeignet sind, die für ihn relevanten Verfügbarkeitsziele abzubilden.



# 4. Betriebs- und Wartungsleistungen


## 4.1 Allgemeiner Betriebs- und Wartungsumfang

Der Auftragnehmer betreibt und wartet die in der Anlage abgebildeten Systeme im vertraglich vereinbarten Umfang und nach Maßgabe dieses SLA. Art und Umfang der laufenden Betriebs- und Wartungsleistungen ergeben sich insbesondere aus den technischen Grundlagen nach Ziffer 2; die Anlage konkretisiert diese Grundlagen für die dort abgebildeten Systeme und kann sie abweichend oder ergänzend regeln.

Der Auftragnehmer erbringt die Betriebs- und Wartungsleistungen mit der Sorgfalt eines ordentlichen und fachkundigen IT-Dienstleisters. Darüber hinausgehende Leistungen, insbesondere Betrieb, Weiterentwicklung und fachliche Betreuung der auf den Systemen betriebenen Anwendungen des Auftraggebers, schuldet der Auftragnehmer nur, soweit sie in diesem SLA oder in der Anlage ausdrücklich vereinbart sind.


## 4.2 Sicherheits- und Versionsupdates

### 4.2.1 Begriffsdefinition von Sicherheitsupdates und Versionsupdates

„Sicherheitsupdates“ sind Updates, Upgrades oder sonstige Aktualisierungen von Softwarekomponenten, die vom jeweiligen Hersteller, Distributor, Paket- oder Repositoriumsbetreiber als sicherheitsrelevant gekennzeichnet sind oder nach allgemein anerkannter fachlicher Einschätzung der Behebung von Sicherheitslücken dienen, deren Ausnutzung zu unberechtigtem Zugriff, Datenverlust, Systemmanipulation, Ausfall oder vergleichbaren Beeinträchtigungen führen kann.

„Versionsupdates“ sind Updates, Upgrades oder sonstige Aktualisierungen von Softwarekomponenten ohne unmittelbaren Sicherheitsbezug, zum Beispiel neue Funktionsversionen oder Bugfix-Releases.

### 4.2.2 Vergütung von Nacharbeiten aufgrund von Sicherheitsupdates oder Versionsupdates

Die in der Anlage je System ausgewiesene Betriebs- und Wartungspauschale deckt die regulär zu erwartenden Tätigkeiten im Zusammenhang mit der Installation typischer Sicherheitsupdates sowie üblicher Versionsupdates ab.

Kommt es im Zusammenhang mit Sicherheitsupdates oder Versionsupdates zu Störungen, Ausfällen oder Fehlfunktionen von Systemen oder Anwendungen, die ein unverzügliches Eingreifen erfordern, weil sie zu einer Nichtverfügbarkeit geführt haben oder voraussichtlich zeitnah zu einer Nichtverfügbarkeit führen können, sind die hierfür erforderliche Fehleranalyse, Störungsbeseitigung, Rollbacks oder sonstige Nacharbeiten nicht von der Betriebs- und Wartungspauschale umfasst. Solche Tätigkeiten werden vollständig nach Zeitaufwand zum Standardsatz gesondert vergütet.

### 4.2.3 Ausfallzeiten durch Sicherheitsupdates

Ausfallzeiten, die ausschließlich durch die Durchführung von Sicherheitsupdates im Sinne von Ziffer 4.2.1 entstehen, gelten nicht als Ausfallzeiten im Sinne der Verfügbarkeitsziele nach Ziffer 5.2. Dies umfasst auch Ausfallzeiten, die durch bei fachlich sorgfältiger Vorbereitung nicht vorhersehbare, im Zusammenhang mit den jeweiligen Sicherheitsupdates notwendige Nacharbeiten verursacht werden.

Dies gilt unabhängig davon, ob die Sicherheitsupdates automatisiert nach Ziffer 4.2.4 oder manuell nach Ziffer 4.2.5 eingespielt werden und unabhängig davon, ob sie innerhalb der gemäß Ziffer 5.3 oder abweichend in der Anlage vereinbarten Wartungszeiten oder aufgrund ihrer Dringlichkeit ausnahmsweise außerhalb dieser Zeiten durchgeführt werden.

### 4.2.4 Automatische Installation von Debian-Linux-Sicherheitsupdates durch das apt-unattended-upgrades-Softwarepaket

Der Auftragnehmer richtet, soweit technisch möglich, auf den in der Anlage abgebildeten Systemen den Debian-Paketmanager „apt“ mit dem Paket „unattended-upgrades“ so ein, dass stündlich auf verfügbare Sicherheitsupdates geprüft und diese automatisch installiert werden.

Soweit nach der jeweiligen Paketkonfiguration Neustarts von Programmen oder Diensten beziehungsweise Systemneustarts erforderlich sind, werden diese automatisiert durchgeführt, zum Beispiel um sicherheitsrelevante Kernel-Versionen zu aktualisieren. Hierdurch verursachte kurzfristige Unterbrechungen des Betriebs gelten als Ausfallzeiten im Zusammenhang mit Sicherheitsupdates im Sinne von Ziffer 4.2.3.

Für Systeme, die in der Anlage als „Produktiv-System: Nein“ geführt sind, darf der Auftragnehmer „apt“/„unattended-upgrades“ so konfigurieren, dass bei der Installation von Kernel-Updates ein automatischer Neustart des Systems erfolgt.

Für Systeme, die in der Anlage als „Produktiv-System: Ja“ geführt sind, erfolgen erforderliche Neustarts nach Kernel-Updates ausschließlich manuell durch den Auftragnehmer innerhalb der Wartungszeiten nach Ziffer 5.3; der Neustart ist spätestens innerhalb von sieben Kalendertagen durchzuführen.

### 4.2.5 Manuelle Installation von Sicherheitsupdates

Sicherheitsupdates, die nicht durch automatisierte Mechanismen erfasst oder installiert werden, werden – unabhängig von den vereinbarten Wartungszeiten nach Ziffer 5.3 – nach Möglichkeit unverzüglich eingespielt, sobald der Auftragnehmer Kenntnis von deren Veröffentlichung durch den jeweiligen Hersteller oder Software-Publisher erlangt.

Ist bei der unverzüglichen Durchführung eines solchen Sicherheitsupdates mit einer Beeinträchtigung oder Nichtverfügbarkeit von Systemen zu rechnen, die in der Anlage als „Produktiv-System: Ja“ geführt werden, informiert die jeweils ausführende Vertragspartei die jeweils andere Vertragspartei, soweit dies nach Lage des Einzelfalls machbar und sinnvoll ist, vorab über den in der Anlage bezeichneten allgemeinen Chat-Raum. Bleibt eine Rückmeldung innerhalb von fünf Minuten nach Absendung der Nachricht aus, ist die ausführende Vertragspartei gleichwohl berechtigt, das Sicherheitsupdate unmittelbar, auch außerhalb der Wartungszeiten, ohne vorherige Zustimmung oder Rückmeldung der jeweils anderen Vertragspartei durchzuführen.

### 4.2.6 Versionsupdates von durch den Auftragnehmer verwalteter Software

Nicht sicherheitsrelevante Versionsupdates (Funktions- oder sonstige Versionswechsel ohne unmittelbaren Sicherheitsbezug) werden grundsätzlich als Wartungsarbeiten im Sinne von Ziffer 5.3 behandelt und ausschließlich innerhalb der dort geregelten Wartungszeiten durchgeführt.

Versionsupdates, bei denen nach fachlicher Einschätzung des Auftragnehmers keine oder nur eine geringfügige, zumutbare Beeinträchtigung des produktiven Betriebs zu erwarten ist, können innerhalb der Wartungszeiten ohne gesonderte individuelle Ankündigung durchgeführt werden; im Übrigen gelten die Ankündigungsregelungen in Ziffer 5.3.
Soweit Versionen von Paketen oder Komponenten im Playbook-Git-Repository ausdrücklich festgelegt („gepinnt“) sind, werden Versionsupdates durch Anpassung der dort hinterlegten Versionsangaben vorbereitet und anschließend über den Konfigurations-Code ausgerollt. Soweit im Playbook-Git-Repository lediglich die Installation eines Pakets ohne Festlegung einer konkreten Version vorgesehen ist, erfolgen Versionsupdates typischerweise durch Paketaktualisierungen auf den Systemen, ohne dass hierdurch eine Änderung des Playbook-Git-Repository erforderlich wird.

Größere Versionssprünge und Änderungen mit potenziell wesentlichen Auswirkungen (insbesondere Kernel-Hauptversionen, Datenbank-Hauptversionen sowie vergleichbare Upgrades von Middleware-Komponenten, bei denen absehbar ist, dass sie die Lauffähigkeit der vom Auftraggeber auf den Systemen betriebenen Anwendungen beeinträchtigen können, etwa weil ein Upgrade der Datenbanksoftware zu einer vorübergehenden Nichtverfügbarkeit einer Website führen kann) erforderlich ist) bedürfen der vorherigen Abstimmung mit dem Auftraggeber und gelten, sofern nicht in der Anlage abweichend vereinbart, als gesondert zu vergütende Leistungen zum Standardsatz. Solche Maßnahmen werden vom Auftragnehmer nur nach ausdrücklicher Beauftragung oder aufgrund einer gesonderten Vereinbarung durchgeführt.

Soweit in der Anlage für ein System der Parameter „Automatische Versionsupdates: Ja“ festgelegt ist, ist der Auftragnehmer berechtigt, die von ihm verwalteten Pakete und Komponenten für dieses System innerhalb der Wartungszeiten nach Ziffer 5.3 automatisiert zu aktualisieren, ohne dass es einer individuellen Ankündigung bedarf. Der Auftragnehmer berücksichtigt dabei nach seiner fachlichen Einschätzung die zu erwartenden Auswirkungen auf den produktiven Betrieb.

Ausfallzeiten, die ausschließlich durch im Rahmen der Wartungszeiten nach Ziffer 5.3 oder abweichend in der Anlage vereinbarten Wartungszeiten durchgeführte Versionsupdates nach dieser Ziffer verursacht werden, gelten als Wartungszeiten im Sinne von Ziffer 5.3 und bleiben bei der Berechnung der Verfügbarkeitsziele nach Ziffer 5.2 unberücksichtigt.

### 4.2.7 Sicherheitsupdates von durch den Auftraggeber verwalteter Software

Sicherheitsupdates der vom Auftraggeber in eigener Verantwortung betriebenen oder deployten Anwendungen (insbesondere eigener oder durch Dritte bereitgestellter Anwendungscode, Bibliotheken und sonstige Abhängigkeiten), soweit diese nicht in der Anlage ausdrücklich als vom Auftragnehmer verwaltet vereinbart sind, werden ausschließlich durch den Auftraggeber vorgenommen.

Der Auftragnehmer wirkt an solchen Sicherheitsupdates nur im Rahmen einer gesonderten Beauftragung mit; entsprechende Leistungen werden nach Zeitaufwand zum Standardsatz gesondert vergütet.

Ausfälle oder Beeinträchtigungen, die auf unterlassene, verspätete oder fehlerhafte Sicherheitsupdates solcher vom Auftraggeber verwalteter Komponenten zurückzuführen sind, gelten nicht als Verletzung eines vom Auftragnehmer geschuldeten Verfügbarkeitsziels; im Übrigen gelten die Regelungen der Ziffern 5.2 und 8.

Verweigert der Auftraggeber Sicherheitsupdates für von ihm verwaltete Anwendungen oder Komponenten dauerhaft oder wiederholt oder betreibt er bewusst Software, für die vom Hersteller, Distributor oder Paketbetreiber keine Sicherheitsupdates mehr bereitgestellt werden, übernimmt der Auftragnehmer hierfür keine Verantwortung. Sicherheitsvorfälle, Ausfälle oder sonstige Beeinträchtigungen, die auf solche nicht oder nicht mehr gewarteten Komponenten zurückzuführen sind, gelten nicht als Verletzung von Pflichten aus diesem SLA.

### 4.2.8 Versionsupdates von durch den Auftraggeber verwalteter Software

Versionsupdates der vom Auftraggeber in eigener Verantwortung betriebenen oder deployten Anwendungen (insbesondere eigener oder durch Dritte bereitgestellter Anwendungscode, Bibliotheken und sonstige Abhängigkeiten, soweit diese nicht vom Auftragnehmer im Sinne der Ziffern 2.5.1 und 2.5.3 verwaltet werden) werden ausschließlich durch den Auftraggeber vorgenommen.

Der Auftragnehmer wirkt an solchen Versionsupdates nur im Rahmen einer gesonderten Beauftragung mit; entsprechende Leistungen werden nach Zeitaufwand zum Standardsatz gesondert vergütet.

Ausfälle oder Beeinträchtigungen, die auf solche vom Auftraggeber eigenständig vorgenommenen Versionsupdates zurückzuführen sind, gelten nicht als Verletzung eines vom Auftragnehmer geschuldeten Verfügbarkeitsziels; im Übrigen gelten die Regelungen der Ziffern 5.2 und 8.

### 4.2.9 Updates von TLS-Zertifikaten

Die Erneuerung von TLS-Zertifikaten für durch den Auftragnehmer verwaltete Dienste erfolgt, soweit technisch möglich, innerhalb der nach Ziffer 5.3 vereinbarten Wartungszeiten. Let’s-Encrypt-Zertifikate werden durch den Auftragnehmer regelmäßig im Rahmen der Wartungszeiten erneuert, in der Regel im Zeitraum von vierzehn bis acht Tagen vor Ablauf.
Soweit der Auftraggeber eigene TLS-Zertifikate bereitstellt, ist der Auftraggeber verpflichtet, diese spätestens 30 Tage vor Ablauf des jeweils zu erneuernden TLS-Zertifikats zur Verfügung zu stellen; der Auftragnehmer übernimmt in diesem Fall die Einbindung der TLS-Zertifikate im Rahmen der Wartung innerhalb der Wartungszeiten nach Ziffer 5.3. Der turnusmäßige Austausch solcher TLS-Zertifikate gilt als laufende Wartung und ist im Rahmen der in der Anlage gemäß Ziffer 3.2 vereinbarten Betriebs- und Wartungspauschale abgedeckt.
Pflichten und Haftung des Auftragnehmers im Zusammenhang mit Wartungsarbeiten, Sicherheitsupdates, Versionsupdates und sonstigen Updates richten sich im Übrigen nach Ziffer 8.


## 4.3 Kapazitäts- und Ressourcenmanagement

Der Auftragnehmer beobachtet im Rahmen der Wartung für die in der Anlage abgebildeten Systeme die verfügbaren und genutzten Kapazitäten, die technische Ausstattung sowie die Leistungsressourcen anhand des in Ziffer 2.4.1 beschriebenen technischen Monitoring-Systems. Vom Auftraggeber eigenständig eingerichtete oder betriebene Monitoring- oder Logging-Lösungen (insbesondere anwendungsinterne Metriken) bleiben hierbei unberücksichtigt, soweit nicht in der Anlage ausdrücklich etwas anderes vereinbart ist.

Stellt der Auftragnehmer absehbare Kapazitätsengpässe fest, informiert er den in der Anlage benannten technischen Ansprechpartner des Auftraggebers zeitnah über den in der Anlage bezeichneten allgemeinen Chat-Raum und spricht Empfehlungen zur Kapazitätsanpassung aus. Die Entscheidung über die Umsetzung solcher Maßnahmen obliegt dem Auftraggeber.

Ist ein Kapazitätsengpass so akut, dass ohne unverzügliches Eingreifen ein Ausfall oder eine erhebliche Beeinträchtigung des Betriebs zu erwarten ist und ist der Auftraggeber nicht rechtzeitig erreichbar, ist der Auftragnehmer berechtigt, die zur Aufrechterhaltung des Betriebs und zur Erfüllung seiner Pflichten aus diesem SLA erforderlichen und verhältnismäßigen Maßnahmen eigenständig durchzuführen (insbesondere Erhöhung von Speicherkontingenten, Erweiterung oder Anhängen von Datenträgern, Hochskalieren betroffener Ressourcen). Der Auftragnehmer beschränkt sich dabei auf das technisch notwendige Mindestmaß und informiert den in der Anlage benannten technischen Ansprechpartner des Auftraggebers unverzüglich über den in der Anlage bezeichneten allgemeinen Chat-Raum.

Maßnahmen zur Kapazitätserweiterung, welche der Abwendung akuter Kapazitätsengpässe nach dem vorstehenden Absatz dienen, gelten nicht als laufende Wartung und werden nach Aufwand zum vereinbarten Stundensatz abgerechnet; hierdurch entstehende Provider- und Nutzungsentgelte sowie die vertragliche Beziehung zum jeweiligen Provider trägt ausschließlich der Auftraggeber. Im Übrigen bleiben vereinbarte Wartungsumfänge und Kapazitätsanpassungen, die auf Veranlassung des Auftraggebers geplant und abgestimmt werden, unberührt.


## 4.4 Dokumentation

Die betriebsrelevante Dokumentation erfolgt standardmäßig im Playbook-Git-Repository des Auftraggebers. Abweichend kann der Auftraggeber eine eigene Dokumentationsplattform (zum Beispiel ein Wiki) vorgeben; dies wird gegebenenfalls in der Anlage bezeichnet. Die Dokumentation bezieht sich auf die für den Betrieb und die Wartung der in der Anlage abgebildeten Systeme erforderlichen technischen Inhalte; eine fachliche oder inhaltliche Dokumentation der Anwendungen des Auftraggebers schuldet der Auftragnehmer nicht, sofern nicht in der Anlage ausdrücklich etwas anderes vereinbart ist.

Ein bestimmter Umfang, Detaillierungsgrad oder ein bestimmtes Format der Dokumentation wird nicht geschuldet, sofern nicht in der Anlage ausdrücklich vereinbart. Dokumentationsleistungen werden zum Standardsatz vergütet.

## 4.5 Backup- und Desaster-Recovery-Testläufe

Der Auftragnehmer bietet für die in der Anlage abgebildeten Systeme optional Backup- und Desaster-Recovery-Testläufe (im Folgenden „Backup- und DR-Testläufe“) an. Diese dienen dazu, die technische Einspielbarkeit der Sicherungen nach Ziffer 2.4.2 sowie die Funktionsfähigkeit der Konfigurations- und Automatisierungsprozesse zu überprüfen. Ob und für welche Systeme oder Systemgruppen regelmäßige Backup- und DR-Testläufe vereinbart sind, ergibt sich aus der Anlage; darüber hinaus können Backup- und DR-Testläufe jederzeit auf Anforderung des Auftraggebers für einzelne Systeme oder Systemgruppen beauftragt werden.

Für jeden Backup- und DR-Testlauf richtet der Auftragnehmer im Cloud- oder Rechenzentrums-Account des Auftraggebers nach Ziffer 2.1 ein nicht produktives und temporäres Zielsystem beziehungsweise eine entsprechende Systemgruppe ein, die die produktive Umgebung technisch nachbildet (insbesondere durch automatisiertes Provisioning und Konfiguration mittels des Playbook-Git-Repositorys). Anschließend werden die nach Ziffer 2.4.2 bereitgestellten Backups auf diese Zielsysteme eingespielt, einschließlich der Wiederherstellung von Dateisystem- und Datenbanksicherungen, soweit dies für das jeweilige System relevant ist. Die konkrete technische Umsetzung der Backup- und DR-Testläufe liegt im fachlichen Ermessen des Auftragnehmers.

Backup- und DR-Testläufe prüfen ausschließlich die technische Einspielbarkeit der Backups und das technische Wiederanlaufen der Infrastruktur. Die fachliche Prüfung der wiederhergestellten Daten und Anwendungen (insbesondere inhaltliche Vollständigkeit und Richtigkeit der anwendungsspezifischen Daten sowie die fachliche Abnahme des daraus resultierenden Gesamtsystems) erfolgt nach Abschluss der technischen Umsetzung durch den Auftraggeber.

Backup- und DR-Testläufe werden – unabhängig davon, ob sie als regelmäßige Testläufe in der Anlage vereinbart oder einmalig auf Zuruf beauftragt werden – einschließlich des hierfür erforderlichen Einrichtungsaufwands für die Zielsysteme sowie der Durchführung der Wiederherstellungen, einer gegebenenfalls vom Auftraggeber gewünschten Anbindung der Zielsysteme an den Utility-Stack nach Ziffer 2.4 sowie erforderlicher Nebenarbeiten (zum Beispiel temporärer DNS- oder Routing-Konfigurationen) nach Aufwand zum Standardsatz vergütet. Die für Backup- und DR-Testläufe verwendeten Systeme werden in dem vom Auftraggeber nach Ziffer 2.1 bereitgestellten Cloud- oder Rechenzentrums-Account betrieben; der Auftraggeber trägt die hierfür anfallenden Provider- und Nutzungsentgelte und teilt dem Auftragnehmer nach Abschluss seiner fachlichen Prüfung mit, ab welchem Zeitpunkt die Zielsysteme wieder gelöscht werden können.



# 5. Service Levels und Störungsbearbeitung


## 5.1 Notfallreaktionen

Der Auftragnehmer verpflichtet sich, innerhalb der in der Anlage gebuchten Notfallreaktionszeiten für die in der Anlage als „Produktiv-System: Ja“ geführten Systeme für Notfallreaktionen zur Verfügung zu stehen. Garantierte Notfallreaktionszeiten gelten ausschließlich für Störungen, die vom Auftraggeber als Notfall gemäß den nachfolgenden Bestimmungen und über den Meldeweg nach Ziffer 5.1.1 gemeldet werden.

Ein Notfall im Sinne dieser Ziffer liegt vor, wenn eine oder mehrere der folgenden Situationen vorliegen oder unmittelbar drohen:

a) Dienste, Anwendungen oder Funktionen auf einem oder mehreren Produktiv-Systemen vollständig oder in erheblichem Umfang ausfallen oder deren Nutzung schwerwiegend beeinträchtigt ist, oder  
b) eine akute Gefährdung der Integrität, Verfügbarkeit oder Vertraulichkeit von Daten oder Systemen besteht, oder  
c) der Betrieb eines oder mehrerer Produktiv-Systeme so beeinträchtigt ist, dass hierdurch unmittelbar erhebliche wirtschaftliche oder organisatorische Nachteile zu erwarten sind, insbesondere erhebliche Umsatz-, Bestell-, Buchungs-, Zahlungs- oder Kommunikationsausfälle, der Ausfall geschäftskritischer Schnittstellen zu Drittsystemen oder eine erhebliche Rufschädigung (zum Beispiel durch kompromittierte oder manipulierte Webauftritte), oder  
d) eine der vorstehenden Situationen im Wesentlichen dadurch verursacht wird, dass ein vom Auftraggeber eingesetzter externer Dienstleister (insbesondere Cloud-, Storage-, DNS- oder vergleichbare Infrastruktur-Provider) ausfällt oder in seiner Funktion erheblich beeinträchtigt ist; hiermit ist keine Haftungsübernahme des Auftragnehmers für die Verfügbarkeit oder Qualität der Leistungen des externen Dienstleisters verbunden, die Verantwortlichkeit des Auftragnehmers richtet sich nach den Haftungsregelungen in Ziffer 8.

Ob eine Störung als Notfall im Sinne dieses SLA einzustufen ist, beurteilt der Auftragnehmer auf Grundlage der ihm vorliegenden Informationen nach pflichtgemäßem, fachlich begründetem Ermessen. Diese Einstufung ist zunächst maßgeblich. Rechte des Auftraggebers, die Einstufung gerichtlich oder durch ein unabhängiges Sachverständigengutachten überprüfen zu lassen, bleiben unberührt.

Der Auftraggeber verpflichtet sich, den Auftragnehmer im Falle eines Notfalls unverzüglich über den in Ziffer 5.1.1 beschriebenen Meldeweg zu informieren. Unterbleibt eine Notfallmeldung nach Ziffer 5.1.1, bestehen keine Ansprüche auf Einhaltung der gebuchten Notfallreaktionszeiten.

Der Auftragnehmer garantiert innerhalb der in der Anlage gebuchten Notfallreaktionszeiten ausschließlich die Aufnahme der Arbeiten und den administrativen Zugriff auf die betroffenen Systeme. Eine Entstörung innerhalb der Notfallreaktionszeit oder innerhalb eines bestimmten Zeitraums wird nicht geschuldet; ein Anspruch des Auftraggebers auf Wiederherstellung des ordnungsgemäßen Betriebs innerhalb eines bestimmten Zeitraums besteht nicht. Hiervon unberührt bleiben etwaige Ansprüche des Auftraggebers aus in der Anlage für bestimmte Systeme festgelegten Verfügbarkeitszielen, die auf Grundlage von Ziffer 5.2 vereinbart wurden.

Der Auftragnehmer treibt Entstörungen mit der gebotenen Sorgfalt und nach pflichtgemäßem, fachlich begründetem Ermessen zügig voran und arbeitet, soweit organisatorisch und personell möglich, bis zur Behebung fortlaufend daran weiter. Gleichwohl ist der Auftragnehmer nicht verpflichtet, ununterbrochen an der Entstörung zu arbeiten; er kann die im Notfall zu erbringenden Leistungen in wirtschaftlich und organisatorisch angemessenen Arbeitsphasen mit dazwischenliegenden Ruhephasen erbringen und ist insbesondere nicht verpflichtet, länger als sechs aufeinanderfolgende Stunden ohne Unterbrechung an derselben Störung zu arbeiten. Nach einer ununterbrochenen Arbeitsphase von sechs Stunden steht dem Auftragnehmer eine Ruhepause von bis zu zwei Stunden zu. Die zulässige Dauer einer ununterbrochenen Arbeitsphase beginnt mit dem Zeitpunkt, zu dem der Auftragnehmer die Arbeiten an der jeweiligen Störung tatsächlich aufnimmt, nicht mit dem Eingang der Notfallmeldung. Der Auftragnehmer ist darüber hinaus nicht verpflichtet, innerhalb eines Zeitraums von 24 Stunden ab Aufnahme der Arbeiten zur Entstörung eines Notfalls mehr als insgesamt zwölf Stunden Arbeitszeit im Rahmen der Notfallbearbeitung zu erbringen.

### 5.1.1 Meldeweg für Notfälle

Eine Notfallmeldung im Sinne von Ziffer 5.1 ist nur wirksam, wenn sie

- telefonisch über die in der Anlage bezeichnete Notfall-Rufnummer des Auftragnehmers unter Hinterlassen einer Sprachnachricht auf dem Anrufbeantworter, die zumindest den Namen des Auftraggebers (Firma) und eine kurze Beschreibung des Notfalls (insbesondere betroffene Systeme oder Dienste und die beobachteten Auswirkungen) enthält, und
- zusätzlich durch eine Nachricht im in der Anlage als „SLA-Monitoring-Chat-Raum“ bezeichneten Chat-Raum, die eine kurze Beschreibung des Notfalls (insbesondere betroffene Systeme oder Dienste und die beobachteten Auswirkungen) enthält,

erfolgt.

Die in der Anlage bezeichnete Notfall-Rufnummer ist als reine Alarmierungsnummer eingerichtet. Anrufe werden dort nicht persönlich entgegengenommen, sondern führen stets zur Möglichkeit, eine Sprachnachricht auf dem Anrufbeantworter zu hinterlassen; diese Sprachnachricht löst im internen Monitoring-System des Auftragnehmers die weitere Bearbeitung aus. Eine Notfallmeldung im Sinne dieser Ziffer liegt nur vor, wenn der Auftraggeber beide vorstehenden Schritte ausführt; ein Anruf ohne hinterlassene Sprachnachricht oder eine fehlende oder unvollständige Nachricht im SLA-Monitoring-Chat-Raum gilt nicht als Notfallmeldung.

Die Notfallmeldung gilt grundsätzlich als zugegangen, sobald sowohl die Sprachnachricht auf der Notfall-Rufnummer des Auftragnehmers als auch die Nachricht im SLA-Monitoring-Chat-Raum eingegangen sind. Steht einer der beiden Meldewege aufgrund einer technischen Störung der jeweils eingesetzten Telefonie- oder Chat-Infrastruktur (insbesondere der Systeme des jeweiligen Telekommunikations- oder Chat-Providers oder der Systeme des Auftragnehmers) objektiv nicht zur Verfügung, genügt ausnahmsweise die ausschließliche Nutzung des jeweils anderen Meldewegs; eine fehlende oder eingeschränkte Verfügbarkeit von Endgeräten oder Zugängen auf Seiten des Auftraggebers gilt nicht als solche Störung. Der Auftraggeber hat die Störung des jeweils anderen Meldewegs im Rahmen der Notfallmeldung über den nicht beeinträchtigten Meldeweg mitzuteilen (zum Beispiel durch den Hinweis, dass der Empfang von Chat-Nachrichten beim Auftragnehmer derzeit nicht möglich ist, weil der genutzte Chat-Dienst gestört ist).

Meldungen über andere Kommunikationswege (insbesondere GitLab-Issues oder E-Mails) können vom Auftragnehmer nach bestem fachlichem Ermessen bearbeitet werden, lösen jedoch in keinem Fall die Pflicht zur Einhaltung der vereinbarten Notfallreaktionszeiten aus.

### 5.1.2 Buchbare Notfallreaktionszeiten und Monatspauschalen

Für jedes der nachfolgend aufgelisteten Zeitfenster kann der Auftraggeber eine maximale Notfallreaktionszeit aus den in den dem jeweiligen Zeitfenster zugeordneten nachfolgenden Tabellen aufgeführten Optionen buchen. Die je Zeitfenster gebuchte Notfallreaktionszeit gilt einheitlich für alle Systeme, die in der Anlage als „Produktiv-System: Ja“ geführt werden. Für jedes gebuchte Zeitfenster fällt die Monatspauschale an, die in der dem jeweiligen Zeitfenster unmittelbar nachgeordneten Tabelle der gewählten Notfallreaktionszeit zugeordnet ist.

Zeitfenster:
- Werktage 10:00 Uhr bis 20:00 Uhr
- Werktage 20:00 Uhr bis 10:00 Uhr
- Wochenenden und gesetzlichen Feiertagen 10:00 Uhr bis 20:00 Uhr
- Wochenenden und gesetzlichen Feiertagen 20:00 Uhr bis 10:00 Uhr

Für die Zuordnung eines Notfalls zu einem Zeitfenster ist ausschließlich der Zeitpunkt maßgeblich, zu dem die Notfallmeldung gemäß Ziffer 5.1.1 als zugegangen gilt. Das gilt auch dann, wenn die tatsächliche Aufnahme der Arbeiten aufgrund der gebuchten Notfallreaktionszeit zeitlich in ein anderes Zeitfenster fällt.

Ungeachtet der jeweils gebuchten Notfallreaktionszeiten bemüht sich der Auftragnehmer, auf alle eingehenden Notfallmeldungen so schnell wie möglich zu reagieren.

Für nicht gebuchte Zeitfenster bemüht sich der Auftragnehmer, innerhalb eines Werktags zu reagieren; hierfür wird keine monatliche Pauschale berechnet, und es besteht kein Anspruch auf Einhaltung einer bestimmten Notfallreaktionszeit.

Die konkrete Höhe der Monatspauschalen ergibt sich aus den nachstehenden Tabellen zu den jeweiligen Zeitfenstern; die im Notfall erbrachte Arbeitszeit wird je angefangene 60 Minuten zu den dem jeweiligen Zeitfenster zugeordneten Stundensätzen abgerechnet.

**Maximale Reaktionszeit an Werktagen von 10:00 bis 20:00 Uhr**

| Maximale Reaktionszeit an Werktagen von 10:00 bis 20:00 Uhr | Monatspauschale |
| --- | --- |
| Eine Stunde | 300,00 Euro |
| Zwei Stunden | 230,00 Euro |
| Vier Stunden | 170,00 Euro |
| Sechs Stunden | 120,00 Euro |
| Acht Stunden | 80,00 Euro |
| Zwölf Stunden | 60,00 Euro |
| Keine garantierte Reaktionszeit (nur Best Effort, nächster Werktag) | 0,00 Euro |

Kosten pro begonnener 60 Minuten Arbeitszeit zur Entstörung von Notfällen an Werktagen von 10:00 bis 20:00 Uhr: 100,00 Euro

**Maximale Reaktionszeit an Werktagen von 20:00 bis 10:00 Uhr**

| Maximale Reaktionszeit an Werktagen von 20:00 bis 10:00 Uhr | Monatspauschale |
| --- | --- |
| Eine Stunde | 380,00 Euro |
| Zwei Stunden | 310,00 Euro |
| Vier Stunden | 250,00 Euro |
| Sechs Stunden | 200,00 Euro |
| Acht Stunden | 160,00 Euro |
| Zwölf Stunden | 140,00 Euro |
| Keine garantierte Reaktionszeit (nur Best Effort, nächster Werktag) | 0,00 Euro |

Kosten pro begonnener 60 Minuten Arbeitszeit zur Entstörung von Notfällen an Werktagen von 20:00 bis 10:00 Uhr: 140,00 Euro

**Maximale Reaktionszeit an Wochenenden und gesetzlichen Feiertagen von 10:00 bis 20:00 Uhr**

| Maximale Reaktionszeit an Wochenenden und gesetzlichen Feiertagen von 10:00 bis 20:00 Uhr | Monatspauschale |
| --- | --- |
| Eine Stunde | 430,00 Euro |
| Zwei Stunden | 360,00 Euro |
| Vier Stunden | 300,00 Euro |
| Sechs Stunden | 240,00 Euro |
| Acht Stunden | 190,00 Euro |
| Zwölf Stunden | 160,00 Euro |
| Keine garantierte Reaktionszeit (nur Best Effort, nächster Werktag) | 0,00 Euro |

Kosten pro begonnener 60 Minuten Arbeitszeit zur Entstörung von Notfällen an Wochenenden und gesetzlichen Feiertagen von 10:00 bis 20:00 Uhr: 125,00 Euro

**Maximale Reaktionszeit an Wochenenden und gesetzlichen Feiertagen von 20:00 bis 10:00 Uhr**

| Maximale Reaktionszeit an Wochenenden und gesetzlichen Feiertagen von 20:00 bis 10:00 Uhr | Monatspauschale |
| --- | --- |
| Eine Stunde | 520,00 Euro |
| Zwei Stunden | 450,00 Euro |
| Vier Stunden | 380,00 Euro |
| Sechs Stunden | 310,00 Euro |
| Acht Stunden | 240,00 Euro |
| Zwölf Stunden | 200,00 Euro |
| Keine garantierte Reaktionszeit (nur Best Effort, nächster Werktag) | 0,00 Euro |

Kosten pro begonnener 60 Minuten Arbeitszeit zur Entstörung von Notfällen an Wochenenden und gesetzlichen Feiertagen von 20:00 bis 10:00 Uhr: 175,00 Euro


## 5.2 Verfügbarkeitsziele

Für Systeme, für die in der Anlage kein Verfügbarkeitsziel festgelegt ist, schuldet der Auftragnehmer keine garantierte Mindestverfügbarkeit. Er erbringt seine Leistungen für diese Systeme nach bestem fachlichen Ermessen, ohne dass hierfür ein gesonderter Verfügbarkeitszuschlag berechnet wird und ohne dass ein bestimmtes Verfügbarkeitsziel einzuhalten ist.

Soweit in der Anlage für ein System ein Verfügbarkeitsziel vereinbart ist, gelten die nachfolgenden Regelungen zur Berechnung, zum Nachweis und zur Vergütung der Verfügbarkeit.

### 5.2.1 Berechnung der Verfügbarkeit

Die prozentuale Verfügbarkeit eines Systems im jeweiligen Kalendermonat wird wie folgt berechnet. Die Verfügbarkeit in Prozent ergibt sich aus der Differenz zwischen der Gesamtzeit des Kalendermonats und der Ausfallzeit, multipliziert mit einhundert und dividiert durch die Gesamtzeit des Kalendermonats:

Verfügbarkeit in Prozent = (Gesamtzeit des Kalendermonats − Ausfallzeit) × 100 / Gesamtzeit des Kalendermonats.

Die Berechnung erfolgt in der nach Ziffer 1.2 beschriebenen Zeitzone. Die Gesamtzeit des Kalendermonats ist die tatsächliche Anzahl von Minuten und Sekunden des Kalendermonats, in dem der Ausfall auftritt.

Die Anlage legt für jedes System, für das ein Verfügbarkeitsziel vereinbart ist, insbesondere den Monitoring-Messgegenstand (zum Beispiel die URL einer Website), die Erfolgskriterien (zum Beispiel das Vorhandensein eines Wortlautes im HTML-Inhalt einer Website), das Messintervall sowie die Toleranzschwellen (zum Beispiel die Anzahl aufeinanderfolgender fehlgeschlagener oder erfolgreicher Messpunkte) fest. Die Ausfallzeit ist die Summe aller Zeiträume innerhalb eines Kalendermonats, in denen der in der Anlage für das jeweilige System zur Messung des Verfügbarkeitsziels bezeichnete Monitoring-Messgegenstand nach den in der Anlage festgelegten Erfolgskriterien und Toleranzen als nicht verfügbar gilt. Ein Ausfall im Sinne dieser Ziffer liegt vor, wenn die Monitoring-Prüfungen für einen oder mehrere maßgebliche Messgegenstände nach den in der Anlage festgelegten Toleranzschwellen einen fortlaufenden Fehlerzustand anzeigen.

Die Messdaten des SLA-Monitorings werden in einem hierfür eingesetzten Messdaten-Speicher (zum Beispiel einer Datenbank) vorgehalten. Das SLA-Monitoring-Dashboard kann aus technischen Gründen rollierende Zeiträume (zum Beispiel „letzte 30 Tage“) anzeigen; diese Darstellungen dienen lediglich der operativen Orientierung. Für die vertraglich maßgebliche Berechnung und den Nachweis der Verfügbarkeitsziele sind ausschließlich die aus den im Messdaten-Speicher des SLA-Monitorings für den jeweiligen Kalendermonat gespeicherten Messdaten ermittelten Verfügbarkeitswerte maßgeblich, nicht die gegebenenfalls abweichenden Dashboard-Anzeigen.

Soweit in der Anlage für das jeweilige Verfügbarkeitsziel keine abweichenden Vorgaben zu Messintervall und Toleranzschwelle gemacht werden, gilt als Standard, dass das Monitoring alle dreißig Sekunden eine Prüfung durchführt, ein Ausfall mit dem Zeitpunkt des ersten Messpunkts einer Serie von fünf aufeinanderfolgenden fehlgeschlagenen Messpunkten beginnt und mit dem Zeitpunkt des ersten Messpunkts einer Serie von fünf aufeinanderfolgenden erfolgreichen Messpunkten endet. Die Ausfallzeit eines Ausfalls umfasst dabei den Zeitraum vom ersten Messpunkt der Serie fehlgeschlagener Messpunkte bis zum ersten Messpunkt der Serie erfolgreicher Messpunkte. Die Ausfallzeit wird anhand der Zeitpunkte der Monitoring-Messpunkte auf volle Sekunden genau ermittelt; für Zwecke der Darstellung kann sie in Minuten und Sekunden angegeben werden. In der Anlage können für einzelne Systeme abweichende Messintervalle und Toleranzschwellen definiert werden; diese gehen dem Standard vor.

Aus der vorstehenden Berechnungsformel für die Verfügbarkeit in Prozent ergeben sich für die in diesem SLA vorgesehenen Verfügbarkeitsziele und die unterschiedlichen Monatslängen die maximal zulässigen Ausfallzeiten, die in nachstehender Tabelle dargestellt sind.

| Monat(e)                                                                                      | Gesamtzeit (Minuten) | 99,75 % max. Ausfallzeit | 99,90 % max. Ausfallzeit | 99,95 % max. Ausfallzeit |
| --------------------------------------------------------------------------------------------- | -------------------- | ------------------------ | ------------------------ | ------------------------ |
| Januar, März (ohne Zeitumstellung), Mai, Juli, August, Oktober (ohne Zeitumstellung), Dezember | 44.640 Min           | 111 Min 36 Sek           | 44 Min 38 Sek            | 22 Min 19 Sek            |
| April, Juni, September, November                                                              | 43.200 Min           | 108 Min 0 Sek            | 43 Min 12 Sek            | 21 Min 36 Sek            |
| Februar (28 Tage)                                                                            | 40.320 Min           | 100 Min 48 Sek           | 40 Min 19 Sek            | 20 Min 9 Sek             |
| Februar (29 Tage, Schaltjahr)                                                                | 41.760 Min           | 104 Min 24 Sek           | 41 Min 46 Sek            | 20 Min 53 Sek            |
| März (mit Zeitumstellung, 23-Stunden-Tag)                                                    | 44.580 Min           | 111 Min 27 Sek           | 44 Min 35 Sek            | 22 Min 17 Sek            |
| Oktober (mit Zeitumstellung, 25-Stunden-Tag)                                                 | 44.700 Min           | 111 Min 45 Sek           | 44 Min 42 Sek            | 22 Min 21 Sek            |

Bei der Ermittlung der Ausfallzeit bleiben Zeiträume unberücksichtigt, in denen die Nichtverfügbarkeit auf Umstände zurückzuführen ist, die außerhalb des Verantwortungs- und Einflussbereichs des Auftragnehmers liegen. Hierzu zählen insbesondere:
- Ausfälle und Beeinträchtigungen aufgrund von Wartungsarbeiten nach Ziffer 5.3;
- Ausfälle und Beeinträchtigungen infolge von Störungen der vom Auftraggeber genutzten Rechenzentrums-, Cloud-, Netz- oder Telekommunikationsinfrastruktur oder von Störungen sonstiger vom Auftraggeber eingesetzten Drittanbieter (zum Beispiel DNS-, CDN-, Payment- oder sonstige Infrastruktur-Provider);
- Ausfälle und Beeinträchtigungen infolge eigenständig und nicht mit dem Auftragnehmer abgestimmt vorgenommener Konfigurationsänderungen, Software-Deployments oder sonstiger Eingriffe des Auftraggebers oder der Personen, denen der Auftraggeber Zugriff auf die Systeme oder die darauf betriebene Software gewährt hat, soweit diese Eingriffe nicht auf ausdrücklicher Weisung des Auftragnehmers erfolgten.
- Ausfälle und Beeinträchtigungen infolge höherer Gewalt (zum Beispiel Naturkatastrophen oder Einflussnahme durch staatliche Hoheitsträger);

### 5.2.2 Kosten für Verfügbarkeitsziele

Der Verfügbarkeitszuschlag wird als prozentualer Aufschlag auf die in der Anlage für das jeweilige System ausgewiesene Betriebs- und Wartungspauschale berechnet. Für die nachfolgende Beispielrechnung wird von einem dieser Pauschale zugrunde gelegten Wartungsaufwand von 30 Minuten pro System und Monat ausgegangen.

Beispiel: Beträgt der Betriebs- und Wartungspauschale zugrunde gelegte Wartungsaufwand pro System und Monat 50,00 Euro und ist als Verfügbarkeitsziel 99,75 % mit einem Verfügbarkeitszuschlag von 100 Prozent vereinbart, sind für dieses System 100 Euro pro Monat für die Betriebs- und Wartungspauschale zu vergüten. Der Zuschlag richtet sich nach dem vereinbarten Verfügbarkeitsziel und beträgt:

| Verfügbarkeitsziel | Verfügbarkeits-Zuschlag auf Betriebs- und Wartungspauschale |
| ------------------ | ----------------------------------------------------------- |
| 99,75 %            | 200 %                                                       |
| 99,90 %            | 300 %                                                       |
| 99,95 %            | 500 %                                                       |

Für jedes System, für das in der Anlage ein Verfügbarkeitsziel festgelegt ist, richtet der Auftragnehmer im SLA-Monitoring-System nach Ziffer 2.4.1 die für die Messung und den Nachweis der Einhaltung des Verfügbarkeitsziels erforderlichen Monitoring-Prüfungen ein. Die Vertragsparteien verpflichten sich, Git Pull-/Merge-Requests, mit denen in der Anlage ein neues oder geändertes Verfügbarkeitsziel für ein System eingeführt wird, erst dann in den Git-Branch „main“ des Git-Repositories der Anlage im Sinne von Ziffer 3.1 zusammenzuführen, wenn der Auftraggeber die eingerichteten Monitoring-Prüfungen geprüft und deren Funktionsfähigkeit und Vollständigkeit mit einem Kommentar des betreffenden Git Pull-/Merge-Requests des Git-Repositories der Anlage bestätigt hat.

Für jedes System, für das in der Anlage ein Verfügbarkeitsziel vereinbart ist, werden die hierfür maßgeblichen Monitoring-Messgegenstände im SLA-Monitoring nach Ziffer 2.4.1 eingerichtet; für die Berechnung der Verfügbarkeit und den Nachweis der Einhaltung des Verfügbarkeitsziels sind ausschließlich die Messwerte dieses SLA-Monitorings maßgeblich. Die in dieser Ziffer geregelten Verfügbarkeitsziele stellen Service Levels im Sinne von Ziffer 5.1 dar. Ansprüche des Auftraggebers bei Unterschreitung eines vereinbarten Verfügbarkeitsziels richten sich ausschließlich nach den Haftungsregelungen in Ziffer 8.


## 5.3 Wartungszeiten

Wartungsarbeiten im Sinne dieser Ziffer sind administrative Tätigkeiten des Auftragnehmers an den in der Anlage abgebildeten Systemen (insbesondere Installation von Updates, Konfigurationsänderungen, Neustarts oder vergleichbare Eingriffe). Im Rahmen solcher Wartungsarbeiten kann die Verfügbarkeit oder Leistungsfähigkeit des jeweiligen Systems oder der darauf betriebenen Dienste vorübergehend beeinträchtigt werden oder das System vorübergehend nicht zur Verfügung stehen. Wartungsarbeiten werden so geplant und durchgeführt, dass Umfang und Dauer unvermeidbarer Beeinträchtigungen der Verfügbarkeit auf das technisch notwendige Mindestmaß beschränkt werden.

Wartungsarbeiten erfolgen grundsätzlich innerhalb der folgenden Wartungszeiten:

- an den Werktagen Montag, Mittwoch und Freitag jeweils von 18:30 Uhr bis 7:00 Uhr,
- an Wochenenden und gesetzlichen Feiertagen jeweils von 17:00 Uhr bis 7:00 Uhr.

Wartungsarbeiten können, soweit dies zur Aufrechterhaltung oder Wiederherstellung des Betriebs zwingend erforderlich ist, oder auf ausdrücklichen Wunsch des Auftraggebers – ausnahmsweise auch außerhalb dieser Zeiten durchgeführt werden.

Abweichende oder ergänzende Wartungszeiten können in der Anlage pro System oder allgemein für die gesamte Infrastruktur festgelegt werden.

Wartungsarbeiten, bei denen nach fachlicher Einschätzung des Auftragnehmers eine Beeinträchtigung der Verfügbarkeit oder Leistungsfähigkeit des betroffenen Systems zu erwarten ist (insbesondere mögliche Ausfallzeiten), sind, sofern sie planbar sind, mindestens 48 Stunden im Voraus anzukündigen. Die Ankündigung erfolgt über den allgemeinen Monitoring Chat-Raum gemäß Ziffer 1.4 an die in der Anlage benannten technischen Ansprechpartner des Auftraggebers. Individuelle Absprachen für Wartungsarbeiten außerhalb der vorstehenden Wartungszeiten sind nur mit vorherigem Einverständnis eines in der Anlage benannten technischen Ansprechpartners des Auftraggebers zulässig.


## 5.4 Katastrophenvorsorge und Desaster-Recovery

Der Auftragnehmer betreibt die Infrastruktur des Auftraggebers nach dem Grundsatz „Infrastructure as Code“, um einen weitgehend automatisierten Wiederaufbau und Wiederanlauf der in der Anlage abgebildeten Systeme zu ermöglichen.

Soweit für bestimmte Systeme in der Anlage ein Verfügbarkeitsziel gemäß Ziffer 5.2.2 vereinbart ist, erstellt und pflegt der Auftragnehmer einen schriftlichen Desaster-Recovery-Plan, der die Vorgehensweisen bei Teil- und Totalausfällen beschreibt und eine Wiederherstellung durch hinreichend geschultes Personal des Auftraggebers ermöglicht. Für neu hinzukommende Systeme wird der Plan innerhalb von zwei Wochen nach deren Aufnahme in die Anlage ergänzt. Die Regelungen zu Backups nach Ziffer 2.4.2 und zu Verfügbarkeitszielen nach Ziffer 5.2 bleiben unberührt.

Meldungen und Kommunikation im Störungsfall richten sich nach Ziffer 1.4 (Kommunikation); handelt es sich um einen Notfall im Sinne von Ziffer 5.1, gelten ergänzend die dort geregelten Meldewege und Reaktionszeiten.

Bei akutem Handlungsbedarf und fehlender rechtzeitiger Erreichbarkeit des Auftraggebers ist der Auftragnehmer berechtigt, die zur Aufrechterhaltung bzw. Wiederherstellung des Betriebs erforderlichen und verhältnismäßigen Maßnahmen eigenständig einzuleiten (insbesondere Umschalt-/Failover-Verfahren, Wiederanlauf aus Sicherungen, temporäre Skalierung oder Re-Provisionierung). Der Auftragnehmer beschränkt sich dabei auf das technisch notwendige Mindestmaß, informiert den Auftraggeber unverzüglich nach Durchführung und dokumentiert die Maßnahmen.

Leistungen zur Störungsbeseitigung werden nach Aufwand vergütet; ist der Ausfall dem Auftragnehmer zuzurechnen, erfolgt die Leistung ohne gesondertes Entgelt. Ob ein Ausfall dem Auftragnehmer zuzurechnen ist, stellt der Auftragnehmer auf Grundlage der vorliegenden Monitoring- und Logdaten nach pflichtgemäßem Ermessen fest; diese Feststellung gilt zunächst als verbindlich. Rechte des Auftraggebers, die Feststellung durch ein unabhängiges Sachverständigengutachten oder eine gerichtliche Entscheidung überprüfen zu lassen, bleiben unberührt. Haftungsansprüche richten sich nach den Haftungsregelungen in Ziffer 8.

Regelmäßige Desaster-Recovery-Tests (Wiederanlauf- und Wiederherstellungsproben) werden nicht geschuldet. Optionale Backup- und Desaster-Recovery-Testläufe sind in Ziffer 4.5 geregelt.



# 6. Zugriffsberechtigungen und Sicherheit


## 6.1 Administrative Zugriffsberechtigungen

Der Auftragnehmer gewährt administrativen Zugriff auf die Systeme und Dienste des Auftraggebers ausschließlich den in der Anlage benannten technischen Ansprechpartnern des Auftragnehmers und seinen festangestellten Mitarbeitern.

Der Auftragnehmer stellt sicher, dass alle Personen mit administrativem Zugriff auf die Systeme und Dienste des Auftraggebers zur Vertraulichkeit verpflichtet sind und nur im für die Erfüllung dieses SLA erforderlichen Umfang Zugriff erhalten.

Die Weitergabe von administrativen Zugangsdaten an andere Personen oder Dritte ist unzulässig. Der Auftragnehmer ist berechtigt, einzelne administrative Zugriffsberechtigungen vorübergehend oder dauerhaft zu entziehen oder einzuschränken, soweit dies aus Sicherheitsgründen oder zur Einhaltung gesetzlicher oder vertraglicher Verpflichtungen erforderlich ist; die in der Anlage benannten technischen Ansprechpartner des Auftraggebers werden hierüber unverzüglich informiert.


## 6.2 Verlust von Passwörtern und Zugängen

Der Auftraggeber hat den Auftragnehmer in allen Fällen von Verlust, Diebstahl, Offenlegung oder missbräuchlicher Nutzung von Zugangsdaten sowie bei geplanten oder fristlosen Kündigungen zugangsberechtigter Personen unverzüglich und zu jeder Tages- und Nachtzeit als Notfall im Sinne von Ziffer 5.1 über den Meldeweg nach Ziffer 5.1.1 zu informieren. Diese Meldung ist zeitnah durch ein Issue in der Git-Hosting-Anwendung des Playbook-Git-Repositories zu dokumentieren.

Der Auftragnehmer ist berechtigt, zur Schadensminimierung unverzüglich Sperr-, Rotations- und sonstige Absicherungsmaßnahmen durchzuführen und den Auftraggeber hierüber zu informieren. Der Auftraggeber nimmt zur Kenntnis, dass hierdurch erforderliche vorübergehende Nutzungseinschränkungen und Ausfallzeiten nicht als Ausfälle im Sinne der Verfügbarkeitsziele nach Ziffer 5.2 gelten, soweit die Maßnahmen zur Abwehr oder Eindämmung eines Sicherheitsvorfalls erforderlich sind.


## 6.3 Verwaltungsinterfaces

Der Auftraggeber gewährt dem Auftragnehmer für die Laufzeit dieses Vertrages vollumfänglichen administrativen Zugang (Admin-Zugang) zu den durch Rechenzentrums- bzw. Hostinganbietern bereitgestellten Verwaltungsoberflächen, die zur Leistungserbringung für die in der Anlage abgebildeten Systeme erforderlich sind. Hierzu zählen insbesondere die Administrationsportale der Cloud-Provider (Compute/Storage/Netzwerk), Hypervisor-/VM-Verwaltungen sowie Registrar-/DNS-Zonenverwaltungen.

Soweit technisch vorgesehen, richtet der Auftraggeber eigene Admin-Benutzer beziehungsweise -Rollen für den Auftragnehmer ein. Änderungen, Einschränkungen oder Sperren solcher Zugänge sind unverzüglich mitzuteilen; der Auftraggeber ist verpflichtet, die Funktionsfähigkeit der für die Leistungserbringung erforderlichen Admin-Zugänge dauerhaft sicherzustellen.

Ist ein erforderlicher Admin-Zugang nicht oder nicht hinreichend verfügbar, fordert der Auftragnehmer den Auftraggeber unverzüglich zur Wiederherstellung auf. Soweit und solange der fehlende Zugriff nicht aus dem Verantwortungsbereich des Auftragnehmers stammt, ist der Auftragnehmer insoweit vorübergehend von der Leistungserbringung befreit; vereinbarte Reaktions- oder Verfügbarkeitsziele nach Ziffer 5 gelten während dieser Zeit nicht, und aus der Nichterbringung von Leistungen in diesem Zeitraum werden keine Ansprüche hergeleitet.

Ob die Ursache der Zugangsbeeinträchtigung dem Auftragnehmer zuzurechnen ist, stellt der Auftragnehmer nach pflichtgemäßem Ermessen auf Grundlage der vorliegenden Nachweise (insbesondere Logs und Monitoring-Daten) fest; diese Feststellung gilt zunächst als verbindlich. Rechte des Auftraggebers, die Feststellung durch ein unabhängiges Sachverständigengutachten oder eine gerichtliche Entscheidung überprüfen zu lassen, bleiben unberührt.

Der Auftragnehmer gewährt dem Auftraggeber jederzeit eigene administrative Zugänge (insbesondere root- oder vergleichbare Admin-Zugänge) zu den in der Anlage abgebildeten Systemen. Der Auftragnehmer ist nicht berechtigt, diese Zugänge ohne Zustimmung des Auftraggebers dauerhaft zu entziehen oder einzuschränken; hiervon unberührt bleiben vorübergehende, zur Abwehr oder Eindämmung von Sicherheitsvorfällen erforderliche Maßnahmen nach Ziffer 6.2.

Verweigert der Auftraggeber einen erforderlichen Admin-Zugang dauerhaft oder wiederholt oder stellt er ihn trotz Aufforderung nicht innerhalb einer angemessenen Frist, in der Regel nicht länger als 72 Stunden, wieder her, ist der Auftragnehmer berechtigt, die betroffenen Leistungen einzustellen und diesen Vertrag aus wichtigem Grund fristlos zu kündigen.



# 7. Vertragslaufzeit und Kündigung


## 7.1 Inkraftsetzung und Dauer

Das SLA tritt mit Unterzeichnung in Kraft und läuft auf unbestimmte Zeit.

Der Auftraggeber kann dieses SLA einschließlich der Anlage jederzeit ohne Angabe von Gründen mit sofortiger Wirkung kündigen; die Kündigung erfolgt in Textform per E-Mail gemäß Ziffer 1.4.

Der Auftragnehmer kann dieses SLA einschließlich der Anlage ohne Angabe von Gründen mit einer Frist von 60 Tagen kündigen; die Kündigung erfolgt in Textform per E-Mail gemäß Ziffer 1.4. Das Recht des Auftragnehmers zur fristlosen Kündigung aus wichtigem Grund bleibt unberührt.


## 7.2 Außerordentliche Kündigung aus wichtigem Grund

Der Auftragnehmer ist berechtigt, dieses SLA aus wichtigem Grund ohne Einhaltung einer Kündigungsfrist zu kündigen. Die gesetzlichen Rechte des Auftraggebers zur außerordentlichen Kündigung aus wichtigem Grund bleiben unberührt.

Ein wichtiger Grund liegt vor, wenn dem Auftragnehmer unter Berücksichtigung aller Umstände des Einzelfalls und unter Abwägung der beiderseitigen Interessen die Fortsetzung dieses SLA bis zum Ablauf der ordentlichen Kündigungsfrist oder bis zur sonstigen Beendigung nicht zugemutet werden kann.

Für den Auftragnehmer liegen wichtige Gründe insbesondere vor, wenn

- wiederholte Vertragsverletzungen des Auftraggebers trotz Abmahnung und angemessener Fristsetzung fortbestehen,
- die Systeme vom Auftraggeber oder von Personen, denen der Auftraggeber Zugriff gewährt hat, für rechtswidrige Zwecke genutzt werden (insbesondere zum Bereithalten, Verbreiten oder Abrufen strafbarer Inhalte, etwa volksverhetzender, gewaltverherrlichender oder in vergleichbarer Weise strafbarer Inhalte),
- der Auftraggeber, seine gesetzlichen Vertreter, Organe oder Mitarbeiter Straftaten begehen, die nach Ansicht des Auftragnehmers die weitere Zusammenarbeit unzumutbar machen, insbesondere Straftaten gegen die sexuelle Selbstbestimmung, gegen die körperliche Unversehrtheit, gegen die persönliche Freiheit oder im Zusammenhang mit der Herstellung, Verbreitung oder dem Abruf von Darstellungen sexualisierter Gewalt,
- die Systeme zur Vorbereitung oder Durchführung von Angriffen auf fremde IT-Systeme (insbesondere Hacking, Denial-of-Service-Angriffe, unbefugtes Eindringen in fremde Netze) oder zum Betrieb von Botnetzen genutzt werden oder der Auftraggeber vom Auftragnehmer als kritisch eingestufte Sicherheitsupdates oder sonstige Maßnahmen zur Abwehr konkret bezeichneter, erheblicher Sicherheitsrisiken (zum Beispiel durch Sicherheitswarnungen oder Sicherheitsbulletins dokumentierte Schwachstellen) trotz mindestens dreier schriftlicher Hinweise innerhalb eines Zeitraums von zwei Monaten und angemessen gesetzter Umsetzungsfristen ausdrücklich oder durch Untätigkeit dauerhaft verweigert und hierdurch ein erhebliches Risiko für die Integrität, Vertraulichkeit oder Verfügbarkeit einer oder mehrerer Systeme entsteht,
- der Auftraggeber oder Personen, denen der Auftraggeber Zugriff gewährt hat, durch fahrlässige oder vorsätzliche Handlungen die Sicherheit der Systeme erheblich gefährden (insbesondere durch Missachtung von Sicherheitsvorgaben, Offenlegung von Zugangsdaten oder den Betrieb offensichtlich unsicherer Software),
- der Auftraggeber erforderliche Admin-Zugänge im Sinne von Ziffer 6.3 dauerhaft oder wiederholt verweigert oder diese trotz Aufforderung nicht innerhalb einer angemessenen Frist, in der Regel nicht länger als 72 Stunden, wiederherstellt, soweit dem Auftraggeber dies nicht aus Gründen höherer Gewalt oder vergleichbarer, von ihm nicht zu vertretender Umstände unmöglich ist,
- der Auftraggeber sich mit zwei aufeinanderfolgenden Monatsbeträgen oder einem wesentlichen Teil hiervon in Verzug befindet oder eine nach außen erkennbare ernsthafte Gefährdung seiner Zahlungsfähigkeit eintritt (insbesondere Antrag auf Eröffnung eines Insolvenzverfahrens, Ablehnung eines Insolvenzantrags mangels Masse oder Einstellung von Zahlungen),
- der Auftraggeber oder von ihm veranlasste Personen vorsätzlich oder grob fahrlässig unrichtige Tatsachenbehauptungen über den Auftragnehmer verbreiten, die nach objektiver Betrachtung geeignet sind, dessen Ruf erheblich zu schädigen, oder
- die Systeme in einer Weise genutzt werden, die den Auftragnehmer einem konkret absehbaren erheblichen Risiko der Inanspruchnahme durch Dritte oder aufsichtsrechtlichen Maßnahmen aussetzt, insbesondere bei wiederholten oder trotz Abmahnung fortgesetzten Verstößen gegen datenschutzrechtliche Vorgaben oder gegen Exportkontroll- und Sanktionsrecht.

Die Kündigung aus wichtigem Grund ist in Textform per E-Mail gemäß Ziffer 1.4 unter Angabe der maßgeblichen Gründe zu erklären. Vor Ausspruch der Kündigung ist der andere Vertragsteil grundsätzlich abzumahnen und ihm eine angemessene Frist zur Abhilfe zu setzen, soweit nicht aufgrund der Besonderheiten des Einzelfalls eine Abmahnung entbehrlich ist, insbesondere in Fällen schwerwiegender Straftaten, rechtswidriger Nutzung der Systeme oder erheblicher Gefährdung der Sicherheit der Systeme, bei denen eine Abhilfe objektiv nicht möglich oder dem Auftragnehmer nicht zumutbar ist.



# 8. Haftung und Versicherung


## 8.1 Haftungsausschluss und Haftungsbegrenzung

Die Haftung des Auftragnehmers richtet sich nach den nachfolgenden Regelungen. Eine Haftung wegen Überschreitung beziehungsweise Nichteinhaltung eines Service Levels besteht nur, soweit der Auftragnehmer die Überschreitung beziehungsweise Nichteinhaltung zu vertreten hat; § 254 BGB bleibt unberührt.

Der Auftragnehmer haftet insbesondere nicht für:

1. Ausfälle, die durch den Auftragnehmer nicht direkt verursacht wurden, insbesondere externe DNS- oder Routingprobleme, virtuelle oder sonstige Angriffe auf die Netzinfrastruktur der durch den Auftraggeber beauftragten Server-Provider (DoS/Viren/Schadsoftware) und Ausfälle von Teilen des Internets außerhalb der Kontrolle des Auftragnehmers.
2. Ausfälle, Beeinträchtigungen und Leistungsstörungen im Verantwortungsbereich der vom Auftraggeber ausgewählten Infrastruktur- und Hosting-Anbieter (insbesondere Verfügbarkeitsprobleme von Rechenzentren sowie Compute-, Storage- oder Netzwerkressourcen der Cloud- oder Server-Provider), soweit diese nicht auf vom Auftragnehmer zu vertretende Fehlkonfigurationen der von ihm verwalteten Komponenten zurückzuführen sind.
3. Ausfälle, welche durch Wartungsarbeiten zu den vereinbarten Wartungszeiten verursacht wurden, sofern diese Arbeiten zur Erfüllung dieses SLA notwendig sind und in anderer Form nicht oder nur durch unzumutbaren zusätzlichen Aufwand durchführbar wären.
4. Ausfälle, Schäden und sonstige Verluste, die durch unbefugte oder manipulative Einflüsse Dritter (insbesondere Hackerangriffe, Malware, Ransomware) verursacht werden, soweit der Auftragnehmer die ihm obliegenden Pflichten zur Absicherung der Systeme nicht verletzt hat; im Übrigen richtet sich die Haftung nach den vorstehenden Regelungen, insbesondere Ziffer 8.1 Absätze 3 bis 5.
5. Ausfälle, welche durch höhere Gewalt verursacht wurden, zum Beispiel Naturkatastrophen oder Einflussnahme durch staatliche Hoheitsträger.
6. Ausfälle, welche durch Fehler der auf den Systemen eingesetzten Software (zum Beispiel Bugs in Betriebssystemen, Datenbanken oder Anwendungen) verursacht werden, soweit der Auftragnehmer die ihm obliegenden Pflichten bei Auswahl, Installation, Konfiguration und Pflege dieser Software nicht verletzt hat.
7. Ausfälle, welche auf fahrlässiges Handeln der Mitarbeiter des Auftraggebers zurückzuführen sind.

Weitergehende Ansprüche gegen den Auftragnehmer, insbesondere auf Ersatz mittelbarer oder atypischer Folgeschäden (zum Beispiel Reputations- oder Vertrauensschäden), sind ausgeschlossen, soweit es sich nicht um Schäden handelt, die als direkte oder mittelbare, vertragstypische und vorhersehbare Folge einer Verletzung wesentlicher Vertragspflichten nach den vorstehenden Regelungen zu ersetzen sind.

Für Schäden aus der Verletzung des Lebens, des Körpers oder der Gesundheit haftet der Auftragnehmer nach den gesetzlichen Vorschriften; eine vertragliche Begrenzung der Haftung findet insoweit nicht statt.

1. Im Übrigen haftet der Auftragnehmer nur bei Nichtvorhandensein einer garantierten Beschaffenheit sowie für Vorsatz und grobe Fahrlässigkeit. Dies schließt auch seine gesetzlichen Vertreter, seine in diesem SLA angegebenen technischen Ansprechpartner sowie seine festangestellten Mitarbeiter ein.
2. Für Fehler der vertragsgegenständlichen Leistungen, die bereits bei Vertragsabschluss vorlagen, ist die verschuldensunabhängige Haftung ausgeschlossen; eine Haftung des Auftragnehmers wegen Verschuldens bei der Einrichtung, Konfiguration oder Übergabe der Systeme richtet sich nach den vorstehenden Regelungen.
3. Für leichte Fahrlässigkeit haftet der Auftragnehmer nur, sofern eine wesentliche Vertragspflicht verletzt wird, deren Erfüllung die ordnungsgemäße Durchführung dieses SLA überhaupt erst ermöglicht und auf deren Einhaltung der Auftraggeber regelmäßig vertrauen darf (Kardinalspflicht). Wesentliche Vertragspflichten in diesem Sinne sind insbesondere die Pflichten, die in diesem SLA geregelten Betriebs-, Wartungs- und Sicherungsleistungen (einschließlich der Sicherungen nach Ziffer 2.4.2 sowie der vereinbarten Service Levels nach Ziffer 5) im vereinbarten Umfang zu erbringen.
4. Bei fahrlässiger Verletzung einer Kardinalspflicht ist die Haftung auf solche Schäden beschränkt, mit deren Entstehung im Rahmen der Bereitstellung der vertragsgegenständlichen Leistungen typischerweise gerechnet werden muss (vertragstypischer, vorhersehbarer Schaden).
5. Bei einfach fahrlässig verursachtem Verlust von Daten haftet der Auftragnehmer – sofern er seine Pflichten zur Einrichtung und Durchführung der Sicherungen nach Ziffer 2.4.2 ordnungsgemäß erfüllt hat – abweichend von Ziffer 4 nur für die Kosten, die für die Wiederherstellung der Daten aus den nach Ziffer 2.4.2 vorgesehenen Backups erforderlich gewesen wären. Soweit der Datenverlust darauf beruht, dass der Auftragnehmer diese Pflichten verletzt hat, richtet sich die Haftung nach den vorstehenden Regelungen.
6. Die Haftung nach zwingenden gesetzlichen Bestimmungen wie das Produkthaftungsgesetz sowie der Einwand des Mitverschuldens bleiben unberührt.

Für alle Ansprüche gegen den Auftragnehmer auf Schadensersatz gilt eine Verjährungsfrist von einem Jahr, beginnend mit dem Zeitpunkt zu dem der Schaden festgestellt wurde und der Auftraggeber von den Anspruch begründenden Umständen und der Haftung des Auftragnehmers Kenntnis erlangte oder ohne grobe Fahrlässigkeit hätte erlangen müssen. Die Verjährungsfrist gilt nicht für eine Haftung bei Vorsatz, grober Fahrlässigkeit, für Personenschäden, eine garantierte Beschaffenheit oder nach dem Produkthaftungsgesetz.


## 8.2 Haftpflichtversicherung

Der Auftragnehmer hält für die Laufzeit dieses Service‑Level‑Agreements eine IT‑Haftpflichtversicherung mit Deckungssummen von 3.000.000,00 (drei Millionen) Euro für Vermögensschäden sowie 3.000.000,00 (drei Millionen) Euro für Personen‑ und Sachschäden vor.

Für Vertragsstrafen wegen der Verletzung von Geheimhaltungs‑, Vertraulichkeits‑ oder Datenschutzvereinbarungen bzw. ‑erklärungen gilt eine Entschädigungsgrenze von 300.000,00 (dreihunderdtausend) Euro; diese Entschädigungsgrenze ist Teil der Versicherungssumme.

Der Auftragnehmer informiert den Auftraggeber unverzüglich, wenn die IT-Haftpflichtversicherung gekündigt, ausgesetzt oder in für den Auftraggeber sonstig relevanter Weise eingeschränkt oder geändert wird.

Auf Verlangen weist der Auftragnehmer dem Auftraggeber das Bestehen der IT-Haftpflichtversicherung und deren Deckungssummen nach. Die Haftpflichtversicherung begründet keine über Ziffer 8.1 hinausgehenden Ansprüche gegen den Auftragnehmer; maßgeblich bleiben die dort geregelten Haftungsbeschränkungen.



# 9. Änderungen und Schlussbestimmungen


## 9.1 Änderungen des Service Level Agreements

Das SLA einschließlich der Anlage bildet die abschließende Regelung über den Leistungsumfang des Auftragnehmers nach diesem Vertrag. Weitere Vereinbarungen über Leistungen des Auftragnehmers gelten nur, soweit sie in der Anlage ausdrücklich bezeichnet sind.

Änderungen und Ergänzungen dieses SLA einschließlich der Anlage bedürfen der Zustimmung beider Vertragsparteien und der Textform per E-Mail gemäß Ziffer 1.4. Dies gilt auch für eine Änderung dieser Ziffer. Für inhaltliche Änderungen der Anlage tritt an die Stelle der Textform die in Ziffer 3.1 beschriebene Git-Mechanik.


## 9.2 Rechtswahl und Gerichtsstand

Für dieses SLA einschließlich Anlage gilt das Recht der Bundesrepublik Deutschland unter Ausschluss des UN-Kaufrechts (CISG).

Ausschließlicher Gerichtsstand für alle Streitigkeiten aus oder im Zusammenhang mit diesem SLA einschließlich Anlage ist – soweit gesetzlich zulässig – der Sitz des Auftragnehmers in Berlin, Deutschland.


## 9.3 Sonderregelungen

Keine. EDITME


## 9.4 Salvatorische Klausel

Sofern einzelne Bestimmungen dieses SLA oder der Anlage ganz oder teilweise nicht rechtswirksam oder nicht durchführbar sind oder werden, bleibt die Wirksamkeit der übrigen Bestimmungen dieses SLA und der Anlage unberührt.

Die Parteien werden in diesem Fall eine wirksame und durchführbare Bestimmung vereinbaren, die dem wirtschaftlichen Zweck der unwirksamen oder undurchführbaren Bestimmung möglichst nahekommt; solange eine solche Vereinbarung nicht getroffen ist, gelten die gesetzlichen Regelungen. Dasselbe gilt im Fall einer unbeabsichtigten Regelungslücke.

Der Auftraggeber bestätigt, dass ihm die technischen und vertraglichen Regelungen dieses SLA einschließlich der Anlage erläutert wurden und er deren Inhalt verstanden hat.





_________________________  
Ort, Datum



_________________________  
Unterschrift Max Mustermann EDITME  
Geschäftsführer Example GmbH EDITME  
E-Mail: m.mustermann@example.com EDITME



_________________________  
Ort, Datum


_________________________  
Unterschrift Peter Thurner  
Geschäftsführer Blunix GmbH  
E-Mail: p.thurner@blunix.com  
