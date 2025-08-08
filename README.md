# Arduino-Buttons-LEDs-Project

Arduino-based interactive project where multiple push buttons control corresponding LEDs. 🛠 Components Arduino Uno board ×1

Breadboard ×1

Red LEDs ×4

Push buttons ×4

Resistors: 220Ω (for LEDs) ×4, 10kΩ (for buttons) ×4

Jumper wires (as needed)

USB cable ×1

🔗 Overview 4 push buttons wired to digital pins with internal pull-up.

4 LEDs wired to digital pins with resistors.

When you press a button, its corresponding LED lights up.

📐 Circuit Diagram Add your diagram here:

🧾 Code Example cpp نسخ تحرير const int leds[] = {2, 3, 4, 5}; const int buttons[] = {6, 7, 8, 9};

void setup() { for (int i = 0; i < 4; i++) { pinMode(leds[i], OUTPUT); pinMode(buttons[i], INPUT_PULLUP); } }

void loop() { for (int i = 0; i < 4; i++) { digitalWrite(leds[i], digitalRead(buttons[i]) == LOW ? HIGH : LOW); } } 📋 Steps to Run 1️⃣ Build the circuit as shown in the diagram. 2️⃣ Connect the Arduino to your PC. 3️⃣ Upload the sketch to the board using the Arduino IDE. 4️⃣ Press buttons and watch the LEDs light up!
