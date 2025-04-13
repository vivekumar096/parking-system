# 🚗 Smart Parking System using Min Heap (C++)

This project simulates an efficient parking lot system using a **Priority Queue** implemented via **Min Heap**. The goal is to always allocate the **nearest available parking slot to the lift**, enhancing user convenience.

---

## 📌 Features

- **Custom Parking Layout**: Users input the dimensions of the parking lot and specify the lift location.
- **Smart Slot Allocation**: The system calculates the distance of each slot from the lift and stores them in a Min Heap.
- **Dynamic Updates**: As cars enter or exit the parking lot, the Min Heap is updated to always offer the nearest vacant slot.
- **User-Friendly Simulation**: Mimics real-world parking logic commonly used in malls, offices, and high-traffic buildings.

---

## 🛠️ Technologies Used

- **C++**
- **Priority Queue (Min Heap)** for efficient slot selection
- **OOP Concepts** for modular and clean code structure

---

## 🚀 How It Works

1. **Initialization**  
   - User enters the parking lot's number of rows and columns.  
   - User specifies the coordinates of the lift.

2. **Distance Calculation**  
   - The system calculates the Manhattan distance of all slots from the lift.

3. **Priority Queue Construction**  
   - Vacant slots are inserted into a Min Heap based on their distance from the lift.

4. **Car Entry/Exit Simulation**  
   - When a car enters, the nearest slot is allocated and removed from the heap.  
   - When a car exits, the slot is re-added to the heap and marked vacant.

---

## 📸 Sample Output (CLI)

```plaintext
Enter parking lot size (rows cols): 3 3
Enter lift location (row col): 1 1

Car Entered. Slot Allocated: (1,1)
Car Entered. Slot Allocated: (0,1)
Car Exited from (1,1)
Car Entered. Slot Allocated: (1,1)
