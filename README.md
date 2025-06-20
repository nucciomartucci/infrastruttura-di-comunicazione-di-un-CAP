
# Progetto: Infrastruttura di Comunicazioni per un Centro di Assistenza Primaria (CAP)

**Studente**: Martucci Nuccio (Erasmus)  
**Materia**: Sistemi di informazione e comunicazione nel settore sanitario  
**Data**: dicembre 2023


## Contesto
Progettazione di un'infrastruttura di rete per un Centro di Assistenza Primaria (CAP) di 25m x 30m con:
- 6 ambulatori medici
- 6 ambulatori infermieristici
- 2 sale di cura
- 1 sala prelievi
- 1 sala riunioni
- Area amministrativa con 4 postazioni pubbliche e 2 telefoniche

## Requisiti del Progetto
1. **Analisi delle opzioni tecniche**:
   - Scelta tra architettura centralizzata vs distribuita
   - Selezione tra dispositivi low-cost vs fascia alta
2. **Schema di interconnessione** dei dispositivi
3. **Piano di cablaggio** con posizionamento di:
   - Punti rete (rosette)
   - Dispositivi di comunicazione (router, switch)
4. **Giustificazione delle scelte**:
   - Tipologia di cavo
   - Numero e porte degli switch
   - Robustezza e scalabilità
5. **Specifiche tecniche** di tutti i componenti
6. **Budget dettagliato**
7. **Piano di implementazione temporale**

## Soluzione Implementata
### Architettura di Rete
- **Approccio ibrido**: Elementi centralizzati (server, firewall) e distribuiti (switch periferici)
- **Topologia a stella gerarchica** per ridurre i single point of failure
- **Scelta dispositivi fascia alta** (Cisco) per affidabilità e sicurezza

### Componenti Principali
| Dispositivo | Modello | Caratteristiche | Quantità |
|-------------|---------|----------------|----------|
| **Switch Core** | Cisco SG350-10SFP | 10 porte (1/10 Gbps) | 1 |
| **Switch Periferici** | Cisco CBS250-24T-4X | 24 porte + 4 SFP+ | 4 |
| **Router** | Cisco C1101-4P | Porte Gigabit Ethernet | 1 |
| **Firewall** | Cisco Firepower 4110 | Next-Generation Firewall | 1 |
| **Server** | Dell PowerEdge R740 | Intel Xeon, 3TB RAM | 1 |
| **Cablaggio** | Belden 74011NH (Cat 6a) | 10 Gbps @ 100m | 1200m |
| **Cablaggio Core** | UTP Cat 7 | 10 Gbps, doppia schermatura | 20m |

### Punti Chiave
- **Cablaggio**: CAT 6a per la maggioranza dei punti, CAT 7 per le connessioni core
- **Scalabilità**: 30% di porte libere per future espansioni
- **Sicurezza**: Firewall enterprise per protezione dati sanitari
- **Assenza WiFi**: Soluzione cablata per evitare interferenze con pazienti elettrosensibili
- **Budget Totale**: €40,740.50

### Diagrammi
- Schema di interconnessione dispositivi
- Piano distribuzione cablaggio
- Cronogramma implementazione (3 mesi)

[Scarica la documentazione completa](Proyecto_SICSB.pdf)
## Note dell'autore
> Progetto sviluppato individualmente. 
> Include giustificazioni tecniche dettagliate e analisi dei costi
