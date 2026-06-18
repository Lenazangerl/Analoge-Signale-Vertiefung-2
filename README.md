# Analoge-Signale-Vertiefung-2
---

Der **Effektivwert** ist der Wert einer Wechselspannung oder eines Wechselstroms, der die gleiche Leistung erzeugt wie eine gleich große Gleichspannung bzw. ein gleich großer Gleichstrom.

Wechselspannung ändert sich ständig von + zu - der durchschnitt wäre null (Sinus), um diesen mit einer gleichspannung (konstant), zu vergleichen braucht man einen durschnittswert. Daher bildet man den Effektivwert.

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

**Erstelle vier Funktionsdiagramme und nehme dabei an, dass der Spitzenwert 5V beträgt. Berechne daneben immer den Effektivwert und erläutere in kurzen Worten oder mit grafischen Hilfsmitteln, wie das Ergebnis zustande kommt.**

## 1. Sinussignal

$$
U_\mathrm{eff}=\frac{\hat U}{\sqrt{2}}
$$

Einsetzen:

$$
U_\mathrm{eff}=\frac{5}{\sqrt{2}}
$$

$$
U_\mathrm{eff}=\frac{5}{1{,}414}
$$

$$
U_\mathrm{eff}\approx 3{,}54\ \text{V}
$$

**Warum?**  
Der Sinus erreicht den Spitzenwert nur kurz → der Mittelwert der Leistung ist kleiner.

---

## 2. Rechtecksignal

$$
U_\mathrm{eff}=\hat U
$$

Einsetzen:

$$
U_\mathrm{eff}=5\ \text{V}
$$

**Ergebnis:**

$$
U_\mathrm{eff}=5{,}00\ \text{V}
$$

**Warum?**  
Die Spannung ist konstant → keine Schwankung → volle Leistung die ganze Zeit.

---

## 3. Dreiecksignal

$$
U_\mathrm{eff}=\frac{\hat U}{\sqrt{3}}
$$

Einsetzen:

$$
U_\mathrm{eff}=\frac{5}{\sqrt{3}}
$$

$$
U_\mathrm{eff}=\frac{5}{1{,}732}
$$

$$
U_\mathrm{eff}\approx 2{,}89\ \text{V}
$$

**Warum?**  
Linearer Anstieg und Abfall → viele kleine Werte, daher geringerer Effektivwert.

---

## 4. Sägezahnsignal

$$
U_\mathrm{eff}=\frac{\hat U}{\sqrt{3}}
$$

Einsetzen:

$$
U_\mathrm{eff}=\frac{5}{\sqrt{3}}
$$

$$
U_\mathrm{eff}=\frac{5}{1{,}732}
$$

$$
U_\mathrm{eff}\approx 2{,}89\ \text{V}
$$

**Warum?**  
Auch hier wird der Spitzenwert nur kurz erreicht → gleicher Effektivwert wie Dreieck.

---

**Kondensatoren und Spulen werden in der Wechselstromtechnik als Widerstände eingesetzt. Beschreibe die drei verschiedenen Widerstandsarten bei einer sinusförmigen Wechselspannung. Warum ist zum Beispiel der Widerstand einer Spule an Sinusspannungen größer als bei Gleichspannung? Wie berechnet man diese Widerstände und wieso spielt die Kreisfrequenz hier eine Rolle?**




## Induktiver Widerstand (Spule)

$$
X_L = \omega L
$$

mit:
- \(X_L\) = induktiver Widerstand  
- \(L\) = Induktivität  
- \(\omega = 2\pi f\)

---

### Gleichstrom (f = 0)

$$
X_L = 0
$$

→ Die Spule wirkt wie ein normaler Leiter (fast kein Widerstand)

---

### Erklärung

Bei Gleichstrom ändert sich der Strom nicht.  
Ohne Stromänderung entsteht keine Induktionsspannung:

- keine Änderung des Magnetfelds  
- keine Gegenspannung  
- daher kein „induktiver Widerstand“

---

### Wechselstrom

Bei Wechselspannung ändert sich der Strom ständig:

- Spule erzeugt eine Gegenspannung
- sie „wehrt sich“ gegen Stromänderung

---

### Warum steigt der Widerstand bei AC?

$$
X_L \propto f
$$

Je höher die Frequenz:
- desto schneller die Stromänderung
- desto stärker die Gegeninduktion
- desto größer der Widerstand

---

### Kreisfrequenz

$$
\omega = 2\pi f
$$

$$
X_L = \omega L
$$
