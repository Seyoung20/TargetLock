<div align="center">

# **TARGET LOCK**

<p>
    <img src="https://img.shields.io/badge/version-v1.0-green" alt="Version">
    <img src="https://img.shields.io/badge/project-OOP-blue" alt="License">
    <img src="https://img.shields.io/badge/SDG-3_Good_Health-blueviolet" alt="SDG 3">
  </p>

</div>

<br />

# TargetLock
**TargetLock** is designed to support a healthier lifestyle by empowering users to make more mindful and goal-aligned food decisions. Inspired by the principles of **`Sustainable Development Goal 3`**, the system promotes long-term wellness, disease prevention, and healthier daily habits through informed nutrition awareness. Whether your focus is overall fitness, improved mood, better sleep, glowing skin, stress reduction, or simply building a sustainable healthy routine, TargetLock encourages consistency and positive choices that contribute to your personal well-being.

---

## **DESCRIPTION/OVERVIEW**

TargetLock is designed to transform the process of healthy eating into a guided, data-driven experience. The system's core function is to connect a user's **target goal** directly with the nutritional impact of their food choices.

### **How it Works:**
1.  **Goal Selection:** The user first selects a specific health objective (**Muscle Gain, Weight Loss**, etc.).
2.  **Food Logging:** After choosing a food item (either from a pre-defined list or using the **Custom Food** option), TargetLock analyzes its **nutritional value, safety level**, and overall health impact.
3.  **Personalized Feedback:** The system then provides clear, personalized recommendations, informing the user whether the food **supports or goes against** their selected goal.
4.  **Motivation:** TargetLock includes a **streak tracker** that records each logged food, providing **encouraging messages** to motivate consistency and support long-term healthy habits, aligning with **SDG 3 – Good Health and Well-Being**.

---

## **OOP CONCEPTS APPLIED**

The application of **Object-Oriented Programming (OOP)** principles ensures a robust, maintainable, and scalable system structure.

| OOP Concept    | Description & Application in TargetLock                                                                                                                                                                                                                                                          |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Encapsulation** | Achieved by bundling data (food name, nutritional values, health goal) and the methods that operate on that data within classes like `FoodItem` and `UserProfile`. **Private** attributes protect internal data, ensuring it is only modified via controlled, **public** methods (getters/setters). |
| **Inheritance**  | Used to model specialized behaviors from a general type. A base class, **`HealthGoal`**, is extended by subclasses like **`WeightLossGoal`** or **`MuscleGainGoal`**. These subclasses share common properties but implement specific, distinct goal-checking logic. |
| **Abstraction**  | Focuses on showing essential features while hiding complex implementation details. The **`Analyzer`** class exposes a simple **`getRecommendation()`** method, abstracting away the complex nutritional calculations and safety checks performed internally. |
| **Polymorphism** | Allows a single interface to be used for different implementations. The core **`Analyzer`** interacts with all goal types through a single **`HealthGoal`** reference. When the **`analyze(food)`** method is called, the correct, goal-specific logic is executed. |

---

## **PROGRAM STRUCTURE** 

The system is designed with several key classes to manage functionality and data flow.

* **`TargetLockApp` (Main Class):** **Orchestrates** the main menu, user interaction, and overall program execution.
* **`UserProfile`:** **Stores** the user's chosen goal and manages the **streak tracker**.
* **`HealthGoal` (Abstract Base Class):** **Defines** the common interface for all health objectives.
    * *Subclasses:* `MuscleGainGoal`, `WeightLossGoal`, etc.
* **`FoodItem`:** **Represents** a piece of food with all nutritional attributes. Includes the **Custom Food** option.
* **`Analyzer`:** **Contains** the core logic for processing a food item against the user's goal, calculating the health impact, and generating **personalized recommendations**.
* **`StreakTracker`:** **Manages** the streak count and provides motivational messages for consistency.

---

## **HOW TO RUN THE PROGRAM**

This is a console-based application requiring a Java environment.

1.  **`Select Goal:`** First, the user selects their **desired health goal**.
2.  **`Select Food:`** After choosing a goal, the system displays food categories, and the user selects a specific item.
3.  **`Custom Food Option:`** If the food is not listed, they can use the **Custom Food** option, manually entering the food name and its nutritional values.
4.  **`Analysis and Recommendations:`** Once submitted, the system **analyzes** the input and informs the user about the food’s overall healthiness, its safety level, and personalized recommendations on whether it **supports or goes against** their selected goal. It also suggests **healthier options**.
5.  **`Motivation:`** The **streak tracker** is included to motivate consistency, encouraging users to regularly check their food choices and maintain a long-term healthy lifestyle.

---

## **SAMPLE OUTPUT**
<details>
  <summary>Lose Weight</summary>
<img src="img/1-1.png" alt="Char Creation" width="50%">
<img src="img/1-2.png" alt="Char Creation" width="50%">
<img src="img/1-3.png" alt="Char Creation" width="50%">
</details>

<details>
  <summary>Gain Muscle</summary>
<img src="img/2-1.png" alt="Stats Up" width="50%">
<img src="img/2-2.png" alt="Stats Up" width="50%">
<img src="img/2-3.png" alt="Stats Up" width="50%">
</details>

<details>
  <summary>Maintain Energy</summary>
<img src="img/3-1.png" alt="Ending" width="50%">
<img src="img/3-2.png" alt="Ending" width="50%">
<img src="img/3-3.png" alt="Ending" width="50%">
</details>

---

## **AUTHOR AND ACKNOWLEDGEMENT** 

**Gratitude to Our Instructor**

<p align="center">
  <img src="img/grace.png" width="200px" alt="Grace" style="border-radius: 100px;" />
</p>

We would like to express our sincere gratitude to our CS 211 instructor, **`Ms. Christiana Grace Alib`**, for her invaluable mentorship and guidance. Her expertise in Object-Oriented Programming principles was crucial to our effective application of these concepts, leading to the successful development of our system, **TargetLock**.

---

### Project Made By: Looter's Members

<table>
  <tr>
    <td align="center">
      <a href="https://www.facebook.com/atarahjrzi">
        <img src="/img/mayan.png" width="100px;" alt="Alea, Mariane GitHub Profile Image"/>
      </a>
      <br />
      <sub><b>Alea, Mariane M.</b></sub>
      <br />
      <a href="https://www.facebook.com/atarahjrzi">
        <img src="https://img.shields.io/badge/Facebook-1877F2?style=flat&logo=facebook&logoColor=white" alt="Facebook"/>
      </a>
      <br />
      <a href="https://www.instagram.com/atarahjrzi/">
        <img src="https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white" alt="Instagram"/>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://www.facebook.com/justinjake.baliwag">
        <img src="/img/justin.png" width="100px;" alt="Baliwag, Justin Jake Profile Image"/>
      </a>
      <br />
      <sub><b>Baliwag, Justin Jake R.</b></sub>
      <br />
      <a href="https://www.facebook.com/justinjake.baliwag">
        <img src="https://img.shields.io/badge/Facebook-1877F2?style=flat&logo=facebook&logoColor=white" alt="GitHub"/>
      </a>
      <br />
      <a href="https://www.instagram.com/4sdfgh.jj/">
        <img src="https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white" alt="Instagram"/>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://www.facebook.com/danielibea.ilagan">
        <img src="/img/daniel.png" width="100px;" alt="Ibea, Daniel Profile Image"/>
      </a>
      <br />
      <sub><b>Ibea, Daniel I.</b></sub>
      <br />
      <a href="https://www.facebook.com/danielibea.ilagan">
        <img src="https://img.shields.io/badge/Facebook-1877F2?style=flat&logo=facebook&logoColor=white" alt="GitHub"/>
      </a>
      <br />
      <a href="https://www.instagram.com/danyll_p/">
        <img src="https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white" alt="Instagram"/>
      </a>
      <br />
    </td>
    <td align="center">
      <a href="https://www.facebook.com/sam.pabito.1">
        <img src="/img/sam.png" width="100px;" alt="Pabito, Sam Angelo Profile Image"/>
      </a>
      <br />
      <sub><b>Pabito, Sam Angelo A.</b></sub>
      <br />
      <a href="https://www.facebook.com/sam.pabito.1">
        <img src="https://img.shields.io/badge/Facebook-1877F2?style=flat&logo=facebook&logoColor=white" alt="GitHub"/>
      </a>
      <br />
      <a href="https://www.instagram.com/sampabitoo/">
        <img src="https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white" alt="Instagram"/>
      </a>
      <br />
    </td>
  </tr>
</table>
