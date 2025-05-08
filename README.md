# 🎮 My Game Dev Portfolio 

---

## **Project Showcase**

# 🏎️ Dom's Racer  
*A Unity-based racing game developed for a university dissertation on controller design impact*  

<img src="https://github.com/DominicTalbot/game-dev-portfolio/blob/e231680b6f9c851be1526f812c12feaa8fe1fb62/Images/DomsRacer.png?raw=true" alt="Gameplay Screenshot" width="900"/>

*Figure: Screenshot of Dom's Racer in action (from dissertation)*  

---

## 📖 **Project Overview**  
**Developed for**: BSc (Hons) Computer Game Technologies Dissertation (University of Suffolk, 2019)  
**Research Focus**: Investigating the impact of controller design (Xbox One, Adaptive Controller, Keyboard) on player experience, heart rate, and performance.  
**Key Features**:  
- Custom terrain and AI-driven opponent cars  
- Lap-tracking system with triggers and timers  
- Camera stabilization for dynamic racing  
- Built with Unity (C#)

<img src="https://github.com/DominicTalbot/game-dev-portfolio/blob/b4fdb7c344cce08b5ec6e05daae66fe5e4d4f073/Images/DomsRacer3.png?raw=true" alt="Terrain Tools" width="500"/>



---

## 🛠️ **Technical Implementation**  
### **1. Terrain & Environment**  
- Created using Unity’s Terrain Tool with custom textures/normal maps.  
- Trees and assets from Unity’s Standard Assets.  
- Skybox: *Classic Skybox* from Unity Asset Store.  

<img src="https://github.com/DominicTalbot/game-dev-portfolio/blob/79491e1777e638c863dd87cb55522f17848944df/Images/DomsRacer4.png?raw=true" alt="Terrain Tools" width="800"/>

*Figure: Terrain design process (from dissertation)*  

### **2. Car Controls & Camera**  
- **Camera Stabilization**: Hidden GameObject tracks car rotation to prevent shaky footage.  
  ```csharp
  transform.eulerAngles = new Vector3(carX - carX, carY, carZ - carZ);
AI Opponents: Waypoint system for pathfinding.

### 3. **Lap System & Timer** 
Triggers at halfway/finish lines to track laps.

- **C# timer converts milliseconds to minutes:seconds.

```csharp
if (SecondCount >= 60) {
    SecondCount = 0;
    MinuteCount += 1;
}
```

---

## 📊 **Research Findings**
**Hypothesis:**  
*"Using an unfamiliar controller affects player performance and heart rate."*

### **Results**
- The **Adaptive Controller** showed the highest mean max heart rate (**88.6 bpm** vs. **Keyboard’s 87.7 bpm**).
- Participants reported higher excitement when using the Adaptive Controller due to its **large buttons**.

### **Controls**
- **Xbox/Adaptive Controller:** Triggers for acceleration/brake.
- **Keyboard:** WASD (default Unity input).

---

## 🔍 **Dissertation Context**
This game was part of a research study comparing **Xbox One, Adaptive, and Keyboard controllers**.

### **Key Insights**
- **Controller design impacts** player comfort and heart rate.
- **Future work:** Expanding participant demographics (see dissertation **Chapter 6**).

📄 **Full Dissertation:** [View Dissertation](https://github.com/DominicTalbot/game-dev-portfolio/blob/45d62db4e5110260660ecb519a0fd4f13f8dc7c3/Documents/FinalDissertation.docx4.pdf)

