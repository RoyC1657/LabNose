# LabNose

An IoT air quality monitoring system built with Arduino that continuously measures VOC (Volatile Organic Compound) levels and streams real-time data to a live cloud dashboard. Triggers an SMS alert when gas levels exceed a defined threshold.

---

## What It Does

- Continuously collects VOC sensor data and streams it to Arduino Cloud
- Displays live charts and gauges on an Arduino Cloud dashboard accessible from any browser or the Arduino Cloud mobile app
- Sends an automated SMS alert via IFTTT webhook when VOC levels exceed 1000 ppb
- Stores up to 15 days of historical chart data in Arduino Cloud

---

## Hardware

- Arduino board with WiFi capability
- VOC / gas sensor
- Micro USB for power and serial monitoring

---

## Tech Stack

- **Arduino Cloud** — device management, data streaming, live dashboard
- **IFTTT (If This Then That)** — webhook integration for SMS alerts
- **Arduino IDE** — firmware development (`.ino`)

---

## How It Works

```
LabNose powers on
    ↓
Connects to WiFi and Arduino Cloud
    ↓
Continuously reads VOC sensor data
    ↓
Streams data to Arduino Cloud dashboard (charts update in real time)
    ↓
If VOC > 1000 ppb → sends webhook to IFTTT → triggers SMS alert
```

---

## Dashboard

The live dashboard is accessible through the Arduino Cloud web app or the Arduino Cloud mobile app on iPhone. It displays:

- Real time VOC gauge
- VOC over time chart
- 15 days of historical data

---

## Setup Instructions

**First time setup:**

1. Create an account at [app.arduino.cc](https://app.arduino.cc)
2. Create a new Thing and add your WiFi credentials under the Things tab
3. Upload the `.ino` sketch to your LabNose device via micro USB
4. Open the dashboard to view live data

**If LabNose is already configured:**

1. Plug in LabNose to power
2. Log in to Arduino Cloud
3. Open the LabNose dashboard to view charts and gauges
4. To modify code or view the serial monitor, connect via micro USB and open the Sketch tab

**SMS Alerts:**

SMS alerts are handled through IFTTT. Each LabNose device requires a separate IFTTT account with a webhook applet configured to trigger on the incoming signal and send an SMS to the associated phone number.

---

## Author

Roy Corella
