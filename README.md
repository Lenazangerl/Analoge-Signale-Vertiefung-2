# Analoge Signale & Wechselstromtechnik: Vertiefung

Der **Effektivwert** ($U_{\mathrm{eff}}$ bzw. $I_{\mathrm{eff}}$) beschreibt den Wert einer Wechselspannung oder eines Wechselstroms, der an einem ohmschen Widerstand im zeitlichen Mittel die gleiche elektrische Leistung (Wärmeenergie) erzeugt wie eine gleich große Gleichspannung oder ein gleich großer Gleichstrom.

> **Hintergrund:** Da sich periodische Wechselspannungen kontinuierlich zwischen positiven und negativen Werten bewegen, beträgt ihr linearer Mittelwert über eine vollständige Periode exakt null. Um die energetische Wirkung dennoch vergleichen zu können, nutzt man das mathematische RMS-Verfahren (*Root Mean Square*):
> 1. Quadrieren der Momentanwerte des Signals $x(t)$ (negative Werte werden positiv).
> 2. Mittelwertbildung über die Periodendauer $T$.
> 3. Ziehen der Quadratwurzel aus diesem Mittelwert.

---

## 1. Signalformen und Effektivwertberechnung ($\hat{U} = 5\,\text{V}$)

Nachfolgend sind die Berechnungen für vier grundlegende Signalformen bei einem Spitzenwert von $\hat{U} = 5\,\text{V}$ aufgeführt.

### A. Sinussignal
**Formel:**
$$U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{2}}$$

**Berechnung:**
$$U_{\mathrm{eff}} = \frac{5\,\text{V}}{\sqrt{2}} \approx \frac{5}{1{,}414} \approx 3{,}54\,\text{V}$$

**Erklärung:**
Die Sinuswelle erreicht ihren Spitzenwert von $5\,\text{V}$ innerhalb einer Periode nur sehr kurzzeitig im Scheitelpunkt. Da die Spannung kontinuierlich ab- und aufbaut, liegt der Leistungseffekt im zeitlichen Mittel deutlich unter dem Spitzenwert.

*[Platzhalter: Labor-Oszilloskop-Diagramm des Sinussignals]*

---

### B. Rechtecksignal (symmetrisch)
**Formel:**
$$U_{\mathrm{eff}} = \hat{U}$$

**Berechnung:**
$$U_{\mathrm{eff}} = 5{,}00\,\text{V}$$

**Erklärung:**
Das ideale Rechtecksignal schaltet instantan zwischen $+5\,\text{V}$ und $-5\,\text{V}$ um. Da der Betrag der Spannung zu jedem Zeitpunkt konstant $5\,\text{V}$ ist ($5^2 = (-5)^2 = 25$), ist die Leistungsabgabe durchgehend maximal. Der Effektivwert entspricht genau dem Scheitelwert.

*[Platzhalter: Labor-Oszilloskop-Diagramm des Rechtecksignals]*

---

### C. Dreiecksignal
**Formel:**
$$U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{3}}$$

**Berechnung:**
$$U_{\mathrm{eff}} = \frac{5\,\text{V}}{\sqrt{3}} \approx \frac{5}{1{,}732} \approx 2{,}89\,\text{V}$$

**Erklärung:**
Durch den rein linearen, gleichmäßigen Anstieg und Abfall verweilt das Signal mathematisch gesehen viel Zeit in der Nähe des Nullpunkts. Da kleine Werte im Quadrat noch kleiner gewichtet werden, fällt der Effektivwert geringer aus als beim harmonischen Sinussignal.

*[Platzhalter: Labor-Oszilloskop-Diagramm des Dreiecksignals]*

---

### D. Sägezahnsignal
**Formel:**
$$U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{3}}$$

**Berechnung:**
$$U_{\mathrm{eff}} = \frac{5\,\text{V}}{\sqrt{3}} \approx \frac{5}{1{,}732} \approx 2{,}89\,\text{V}$$

**Erklärung:**
Obwohl die Kurvenform optisch asymmetrisch ist (linearer Anstieg gefolgt von einem steilen Abfall), ist die mathematische Verteilung aller Amplitudenwerte innerhalb einer Periode identisch mit der des Dreiecksignals. Daher ergibt sich exakt derselbe Effektivwert.

*[Platzhalter: Labor-Oszilloskop-Diagramm des Sägezahnsignals]*

---

## 2. Widerstandsarten in der Wechselstromtechnik

In der Wechselstromtechnik wird der klassische Widerstandsbegriff erweitert, da Energiespeicher (Kondensatoren und Spulen) den Stromfluss frequenzabhängig beeinflussen.

| Widerstandsart | Formelzeichen / Berechnung | Verhalten bei Gleichstrom (DC, $f = 0\,\text{Hz}$) | Verhalten bei Wechselstrom (AC) |
| :--- | :--- | :--- | :--- |
| **Ohmscher Widerstand** | $R = \frac{U}{I}$ | Konstanter Widerstand. Wandelt elektrische Energie unumkehrbar in Wärme um. | Frequenzunabhängig. Strom und Spannung verlaufen absolut phasengleich. |
| **Induktiver Blindwiderstand** (Spule) | $X_L = \omega \cdot L = 2\pi f \cdot L$ | $X_L = 0\,\Omega$<br>Wirkt nach dem Einschalten wie ein idealer Kurzschluss/Leiter. | Proportional zur Frequenz. Erzeugt eine Phasenverschiebung (Strom eilt der Spannung nach). |
| **Kapazitiver Blindwiderstand** (Kondensator) | $X_C = \frac{1}{\omega \cdot C} = \frac{1}{2\pi f \cdot C}$ | $X_C \rightarrow \infty\,\Omega$<br>Wirkt im geladenen Zustand wie eine dauerhafte Leitungsunterbrechung. | Antiproportional zur Frequenz. Führt zu einer Phasenvoreilung des Stroms. |

### Warum ist der Widerstand einer Spule an Sinusspannungen größer als bei Gleichspannung?
Ein sinusförmiger Wechselstrom ändert kontinuierlich seine Stärke und Richtung. Nach dem **Lenzschen Gesetz** induziert jede Stromänderung in einer Spule eine Gegenspannung (Selbstinduktion), welche ihrer Ursache – der Stromänderung – entgegenwirkt. Je schneller sich der Strom ändert (also je höher die Frequenz $f$ bzw. Kreisfrequenz $\omega$ ist), desto intensiver ist diese induzierte Gegenspannung. Bei Gleichstrom findet nach dem Einschwingvorgang keine Stromänderung mehr statt, weshalb die Gegenwirkung verschwindet und nur der minimale ohmsche Drahtwiderstand wirksam bleibt.

### Die Rolle der Kreisfrequenz ($\omega$)
Die Kreisfrequenz $\omega = 2\pi f$ beschreibt die Winkelgeschwindigkeit der Zeigerrotation und repräsentiert die zeitliche Änderungsrate des Signals in Radiant pro Sekunde. Sie fließt direkt in die Berechnung ein, weil die Blindwiderstände dynamische Reaktionen auf die *Änderungsgeschwindigkeit* des Stroms (Spule) bzw. der Spannung (Kondensator) darstellen.

---

## 3. Modulation in der Nachrichtentechnik

Unter **Modulation** versteht man den Vorgang, bei dem ein niederfrequentes Nutzsignal (Information wie Audio oder Daten) einen Parameter eines hochfrequenten Trägersignals gezielt verändert. Dies ist notwendig, da niederfrequente Signale aufgrund physikalischer Gesetze (z. B. erforderliche Antennenlänge) nicht direkt über weite Strecken effizient übertragen werden können.

Ein sinusförmiger Träger besitzt drei primäre Parameter, die moduliert werden können:
1. **Amplitudenmodulation (AM):** Das Nutzsignal verändert die Höhe (Amplitude) des Trägersignals. Anfällig für atmosphärische Störungen (Rauschen).
2. **Frequenzmodulation (FM):** Das Nutzsignal verändert die zeitliche Frequenz des Trägers. Sehr robust gegenüber Störungen (z. B. UKW-Radio).
3. **Phasenmodulation (PM):** Das Nutzsignal verändert den aktuellen Phasenwinkel des Trägers. Bildet das Fundament moderner, digitaler Übertragungsverfahren (WLAN, LTE, 5G).

---

## 4. Tiefpassfilter und Grenzfrequenz

Ein RC-Tiefpass lässt Signale mit Frequenzen unterhalb seiner Grenzfrequenz $f_g$ nahezu ungeschwächt passieren, während höhere Frequenzen gedämpft werden. Die Berechnung der Grenzfrequenz erfolgt über die Formel:

$$f_g = \frac{1}{2\pi \cdot R \cdot C}$$

### Dimensionierung einer Schaltung für $f_g = 1\,\text{kHz}$
Um eine Grenzfrequenz von genau $1\,\text{kHz}$ ($1000\,\text{Hz}$) zu realisieren, wählen wir einen Standardwert für den Kondensator und berechnen den dazu passenden Widerstand:
* **Gewählt:** Kapazität $C = 100\,\text{nF} = 100 \cdot 10^{-9}\,\text{F}$
* **Berechnung des Widerstands $R$:**

$$R = \frac{1}{2\pi \cdot f_g \cdot C} = \frac{1}{2\pi \cdot 1000\,\text{Hz} \cdot 100 \cdot 10^{-9}\,\text{F}} \approx 1591{,}55\,\Omega$$
* **Bauteilauswahl:** Es wird ein Widerstand von **$1{,}59\,\text{k}\Omega$** (bzw. ein $1{,}5\,\text{k}\Omega$ in Reihe mit einem $91\,\Omega$ Widerstand) verwendet.

### Tinkercad-Versuchsaufbau und Überprüfung
Zur Überprüfung der Schaltung wird in Tinkercad folgende Schaltung simuliert:
1. Ein **Funktionsgenerator** wird an den Eingang der Schaltung angeschlossen (Sinuswelle, Amplitude: $5\,\text{V}$).
2. Ein **Widerstand mit $R = 1{,}59\,\text{k}\Omega$** wird in Reihe zum Signalweg geschaltet.
3. Ein **Kondensator mit $C = 100\,\text{nF}$** wird nach dem Widerstand gegen Masse (GND) geschaltet.
4. Ein **Oszilloskop** greift die Ausgangsspannung parallel am Kondensator ab.

**Verhalten bei der Überprüfung:** * Speist man eine niedrige Frequenz von $100\,\text{Hz}$ ein, bleibt die Ausgangsamplitude nahezu unverändert bei knapp $5\,\text{V}$.
* Erhöht man die Frequenz exakt auf die berechnete Grenzfrequenz von $1\,\text{kHz}$, sinkt die Ausgangsspannung auf genau **$70{,}7\,\%$** des Eingangswertes (Dämpfung um $-3\,\text{dB}$, was exakt $U_{\mathrm{eff}} = \frac{U_{\mathrm{in}}}{\sqrt{2}}$ entspricht) und zeigt eine Phasenverschiebung von $-45^\circ$.
* Bei Frequenzen weit über $1\,\text{kHz}$ (z. B. $10\,\text{kHz}$) bricht die Ausgangsspannung am Oszilloskop fast vollständig ein.

*[Platzhalter: Screenshot der aufgebauten Tiefpass-Schaltung aus Tinkercad bei 1 kHz]*
