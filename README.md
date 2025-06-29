# Hot Standby Simulation in Java

This is a simple Java simulation that demonstrates the **Hot Standby** redundancy pattern used in **mission-critical systems** to ensure high availability.

## 🧠 What Is Hot Standby?

Hot standby is a fault-tolerant design where a **standby system** runs in parallel with the **primary system**, maintaining a **live replicated state**. If the primary system fails, the standby can take over **immediately**, minimizing downtime and preventing data loss.

## 🚀 What Does This Project Do?

- Simulates a **primary system** processing data.
- Simulates a **standby system** that continuously receives replicated data from the primary.
- Introduces a simulated failure in the primary system.
- Automatically triggers the **standby system to take over**, continuing operations seamlessly with the replicated state.

## 💡 Key Concepts Demonstrated

- Real-time data replication
- Failover using `CountDownLatch`
- Thread coordination
- Redundancy modeling using simple Java classes

## 📦 Technologies Used

- Java (no external libraries)
- Multithreading (`Thread`, `synchronized`, `CountDownLatch`)

## 📍 Why It Matters

Mission-critical systems (like air traffic control, emergency communication platforms, and financial transaction engines) cannot afford downtime. This simulation shows the **basic principles** behind how such systems maintain availability even when failures occur.

