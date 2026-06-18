# Analoge-Signale-Vertiefung-2
---

Der **Effektivwert** ist der Wert einer Wechselspannung oder eines Wechselstroms, der die gleiche Leistung erzeugt wie eine gleich große Gleichspannung bzw. ein gleich großer Gleichstrom.

## Allgemeine Formel

$$
X_{\mathrm{eff}} = \sqrt{\frac{1}{T}\int_0^T x^2(t)\,dt}
$$

**Erklärung:**
- **X_eff** = Effektivwert
- **T** = Periodendauer
- **x(t)** = Momentanwert des Signals

Zur Berechnung wird:
1. Jeder Momentanwert quadriert.
2. Der Mittelwert über eine Periode berechnet.
3. Die Quadratwurzel gezogen.

---

## Sinussignal

**Formel:**

$$
U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{2}}
$$

oder

$$
I_{\mathrm{eff}} = \frac{\hat{I}}{\sqrt{2}}
$$

**Erklärung:**
- **Û** = Scheitelwert (Spitzenwert)
- **Î** = Scheitelwert des Stroms
- √2 ≈ 1,414

---

## Rechtecksignal

**Formel:**

$$
U_{\mathrm{eff}} = \hat{U}
$$

**Erklärung:**

Das Signal besitzt während der gesamten Periode den gleichen Betrag. Daher ist der Effektivwert gleich dem Scheitelwert.

---

## Dreiecksignal

**Formel:**

$$
U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{3}}
$$

**Erklärung:**

Da das Signal gleichmäßig ansteigt und wieder abfällt, ist der Effektivwert kleiner als beim Sinussignal.

---

## Sägezahnsignal

**Formel:**

$$
U_{\mathrm{eff}} = \frac{\hat{U}}{\sqrt{3}}
$$

**Erklärung:**

Der Effektivwert eines Sägezahnsignals entspricht dem eines Dreiecksignals.

---

## Übersicht

| Signaltyp | Formel |
|-----------|--------|
| Sinus | $$U_{\mathrm{eff}}=\frac{\hat{U}}{\sqrt{2}}$$ |
| Rechteck | $$U_{\mathrm{eff}}=\hat{U}$$ |
| Dreieck | $$U_{\mathrm{eff}}=\frac{\hat{U}}{\sqrt{3}}$$ |
| Sägezahn | $$U_{\mathrm{eff}}=\frac{\hat{U}}{\sqrt{3}}$$ |

## Merksatz

- **Sinus:** durch **√2** teilen.
- **Rechteck:** Effektivwert = Scheitelwert.
- **Dreieck und Sägezahn:** durch **√3** teilen.
- **Allgemein:** **Quadrieren → Mittelwert bilden → Quadratwurzel ziehen.**
