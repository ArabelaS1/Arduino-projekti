<div align="center">

# Arduino Projects Lab

### Embedded sistemi, senzori, automatika i praktična elektronika

<p>
Kolekcija Arduino projekata razvijenih kroz eksperimentisanje sa senzorima, aktuatorima, LCD ekranima, logičkim sklopovima i automatizacijom.
</p>

<img src="https://readme-typing-svg.demolab.com?font=Roboto+Mono&size=20&pause=1000&color=00BFA6&center=true&vCenter=true&width=700&lines=Arduino+Uno+%7C+Sensors+%7C+Automation;Embedded+Logic+%7C+LCD+Interfaces;Practical+Electronics+Projects" />

</div>

---

## Pregled repozitorija

Ovaj repozitorij sadrži praktične Arduino projekte fokusirane na:

<table>
<tr>
<td width="25%" align="center"><b>Senzori</b><br>temperatura, svjetlost, udaljenost</td>
<td width="25%" align="center"><b>Automatika</b><br>releji, motori, alarmi</td>
<td width="25%" align="center"><b>Displeji</b><br>LCD, OLED, serijska komunikacija</td>
<td width="25%" align="center"><b>Logika</b><br>uslovi, stanja, upravljanje</td>
</tr>
</table>

---

## Korištene komponente

<div align="center">

<img src="https://img.shields.io/badge/Arduino_UNO-0A0A0A?style=for-the-badge&logo=arduino&logoColor=00BFA6">
<img src="https://img.shields.io/badge/C%2FC++-0A0A0A?style=for-the-badge&logo=cplusplus&logoColor=00599C">
<img src="https://img.shields.io/badge/LCD_16x2-0A0A0A?style=for-the-badge">
<img src="https://img.shields.io/badge/Sensors-0A0A0A?style=for-the-badge">
<img src="https://img.shields.io/badge/Relay_Module-0A0A0A?style=for-the-badge">

</div>

---

# Projekti

## 01. Smart Room Monitor

<table>
<tr>
<td width="55%" valign="top">

### Opis

Sistem za praćenje osnovnih uslova u prostoriji. Projekat koristi senzor temperature i vlage, fotootpornik i LCD ekran za prikaz podataka u realnom vremenu.

### Funkcionalnosti

- mjerenje temperature i vlage
- detekcija jačine svjetlosti
- prikaz podataka na LCD ekranu
- upozorenje pomoću LED diode kada je prostorija previše tamna ili topla

### Komponente

- Arduino Uno
- DHT11 senzor
- LDR senzor
- LCD 16x2
- LED dioda
- otpornici 220Ω i 10kΩ

</td>
<td width="45%" valign="top">

### Šema povezivanja

```mermaid
flowchart TD
    A[Arduino Uno] --> B[DHT11 senzor]
    A --> C[LDR + 10kΩ otpornik]
    A --> D[LCD 16x2 displej]
    A --> E[LED indikator]
    B --> F[Temperatura i vlaga]
    C --> G[Jačina svjetlosti]
    F --> D
    G --> D
