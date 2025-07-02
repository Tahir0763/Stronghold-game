# 🏰 Stronghold: The Ultimate C++ OOP Challenge

**Stronghold** is an ultra-challenging, console-based multiplayer strategy game designed to push C++ OOP students to their absolute limits. Set in a brutal medieval world, players must manage every facet of a kingdom—economy, warfare, politics, corruption, diplomacy, and survival—all in real-time using advanced C++ concepts.

> ⚠️ This project is intentionally difficult and demands mastery of object-oriented programming, memory management, and system design. Beginners, beware.

---

## 🚀 Features

### 🔥 Extreme Game Mechanics

- **Dynamic Population & Social Structure**
  - Peasants, merchants, nobility, military—all with different roles, needs, and consequences.
  - Plagues, famine, and revolts based on player actions.

- **Realistic Army System**
  - Time-based training (`sleep()`), morale, pay, and corruption.
  - Generals can turn against the kingdom if mismanaged.

- **King Election & Political Chaos**
  - Elections, coups, assassinations, blackmail.
  - Leadership styles dynamically alter gameplay.

- **Deep Economy & Taxation System**
  - Inflation, progressive taxation, corruption, public services, and market crashes.

- **Banking & Corruption Simulation**
  - Loans, audits, fraud, bank heists, treasury mismanagement.

- **Resource & Supply Chain Management**
  - Every resource must be tracked: food, weapons, stone, iron, wood, gold.

- **Dynamic Trade, Market & Diplomacy**
  - Trade deals, sanctions, smugglers, boycotts.

- **Multiplayer & Text-Based Deception**
  - Form alliances or betray others through console chat.
  - Manipulation and broken treaties welcome.

---

## 🛠 Implementation Constraints (C++ OOP)

- 🔄 **Three-File Structure**:  
  - `.h` → Class definitions  
  - `.cpp` → Implementations  
  - `main.cpp` → Game execution  

- 💡 **OOP Design**:  
  - Inheritance, polymorphism (e.g., `Leader` → `King`, `Commander`, `GuildLeader`)  
  - Virtual functions for decision-making systems  

- 📦 **Dynamic Memory**:  
  - All game objects allocated via `new` and deallocated using `delete` or smart pointers  

- ⚠️ **Exception Handling**:  
  - All errors handled via `try-catch` (invalid inputs, file errors, illegal actions)

- 📁 **File Handling**:  
  - Save/load game states  
  - Log resource stats to `score.txt`

- 📦 **Template Classes**:  
  ```cpp
  template <typename T>
  class Resource {
      T quantity;
  public:
      void setQuantity(T q) { quantity = q; }
  };
  
