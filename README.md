# Arduino Telegraph

**Tagline:** Communicate with Morse code using light and Arduino!

---

## **About the Project**

Hey! I built **Arduino Telegraph**, a two-way Morse code communication system using an Arduino R4, an LED, a light sensor, buttons, and a backend. The idea is simple but fun: I can type a message using buttons, it gets converted into Morse code, sent to a backend, and I can get a reply back. The Arduino then blinks the reply with an LED, and a light sensor reads it back — basically, I created a **modern telegraph**!

It’s like chatting via flashes of light. I wanted to make a project that’s interactive, hands-on, and shows how hardware, software, and networks can work together.

---

## **How It Works**

1. **Input:**

   * I use 4 buttons to select numbers that correspond to letters.

     * **Btn1:** Increase number
     * **Btn2:** Accept the current number as a letter
     * **Btn3:** Send the full message
     * **Btn4:** Remove last entry

2. **Sending Message:**

   * Arduino converts the letters to Morse code.
   * The message is sent to a backend via Wi-Fi (HTTP, WebSocket, or MQTT).

3. **Backend Reply:**

   * The backend decodes the Morse code, shows the message, and lets the user type a reply.
   * Reply is converted to Morse code and sent back to Arduino.

4. **Receiving Reply:**

   * Arduino receives the Morse code reply and blinks an LED accordingly.
   * A light sensor detects the blinking LED.
   * Arduino decodes the pulses (dot = 0–600 ms, dash = 600–1000 ms) and displays the message on a screen.

5. **Back-and-Forth Conversation:**

   * I can then type another message using buttons, and the whole cycle repeats.

---

## **Components**

* Arduino R4 (with Wi-Fi)
* 4 Buttons
* OLED/LCD Screen
* LED
* Light Sensor (LDR or Photodiode)
* Resistors, wires, breadboard
* Optional: backend server for message relay

---

## **Why I Made This**

I wanted a project that:

* Combines **hardware and software** in an interactive way
* Uses **Morse code** for learning and fun
* Explores **physical communication via light**
* Lets me experiment with **IoT and networking**

---

## **Challenges**

* Making the light sensor reliably distinguish between dots and dashes.
* Timing calibration for LED pulses (I increased the pulse lengths for reliability).
* Minimizing ambient light interference.

---

## **Conclusion**

**Arduino Telegraph** is a fun, hands-on project that combines electronics, coding, and networking into one interactive system. It’s like a modern telegraph that you can hold in your hands!

---

If you want, I can also **make a “Quick Start” section with wiring instructions and sample Arduino code snippets** to put directly in this README so anyone can build it.

Do you want me to add that next?
