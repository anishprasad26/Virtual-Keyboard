# Virtual-Keyboard
Project focusing python, image processing, open cv, user interface



# **Virtual Keyboard using Hand Tracking**

### **Overview**

This project implements a **Virtual Keyboard** using **Computer Vision** and **Hand Tracking**.
By tracking hand landmarks through your webcam, you can simulate keyboard typing using just your fingers—no physical keyboard needed.

---

### **Features**

* **Hand Detection** using `cvzone`'s HandDetector
* **Finger Position Tracking**
* On-screen **Virtual Keyboard Layout (QWERTY)**
* Press keys by using specific finger gestures:

  * **Pointing with index finger** highlights the key
  * **Pinch gesture (thumb + index)** triggers the key press
* Uses `pynput` to send actual keyboard inputs to the system.

---

### **Technologies Used**

* Python
* OpenCV
* `cvzone` (Hand Tracking Module)
* `pynput` (Simulate keyboard input)

---

### **Requirements**

Install the required libraries:

```bash
pip install opencv-python cvzone pynput
```

---

### **How It Works**

1. **Hand Tracking**:
   The webcam captures your hand using `cvzone.HandTrackingModule`.

2. **Virtual Keyboard Drawing**:
   The keys are drawn on the screen as colored rectangles.

3. **Gesture Control**:

   * **Hover over a key** with your index finger → Highlighted key
   * **Pinch (Thumb + Index finger up)** → Key press is registered
   * Actual key press is simulated using `pynput`.

---

### **Usage**

Run the Python file:

```bash
python virtual\ keyboard.py
```

Make sure your webcam is connected and properly working.

---


### **Project Structure**

```
virtual keyboard.py   # Main project file
```

---

### **Future Improvements**

* Add support for Shift / Caps Lock
* Add number keys and special characters
* Integrate sound feedback
* Create a GUI for customization

---

### **Credits**

* **cvzone** by Murtaza Hassan
* **pynput** for keyboard control

---

