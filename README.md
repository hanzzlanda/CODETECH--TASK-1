### 🔍 **Project Overview: Arduino-Based Temperature Monitoring System**

This project is a **real-time temperature monitoring system** using an **LM35 analog temperature sensor** and an **Arduino Uno**. It displays the current temperature on a **16x2 LCD** (either I2C or parallel interface) and optionally prints it on the **serial monitor**.


### 📦 **Key Components**

* **Arduino Uno** – Main microcontroller
* **LM35 Temperature Sensor** – Outputs analog voltage proportional to temperature (10 mV/°C)
* **16x2 LCD Display** – Shows live temperature readings
* **(Optional)**: Buzzer, Relay, I2C Module, SD Card (for advanced versions)



### ⚙️ **Working Principle**

1. **LM35** senses ambient temperature and outputs an analog voltage.
2. **Arduino** reads the voltage via its **A0 analog pin**, converts it to Celsius.
3. The **LCD** displays the temperature (e.g., "Temp: 32.6 C").
4. The **serial monitor** also logs the temperature for debugging or analysis.



### 🧠 **Formula Used**

Voltage = analogRead(A0) * (5.0 / 1023.0);
Temperature (°C) = Voltage * 100.0;


### 🧪 **Applications**

* Room/environment monitoring
* Server room protection
* Weather stations
* IoT projects (when paired with Wi-Fi or cloud)
