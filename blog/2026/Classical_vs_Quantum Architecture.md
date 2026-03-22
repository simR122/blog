---
date: 2026-03-21
---

# From Transistors to Tunnels: My Journey Through Computer Architecture

I recently went down a rabbit hole exploring how computers actually "think." It’s easy to get lost in the jargon, so I broke it down into three stages: the Classic, the Modern, and the Quantum. Here’s my map of the landscape.

---

## 1. The Foundation: CISC vs. RISC

Everything starts with how a processor understands instructions. I learned that there are two main philosophies:

**CISC (Complex Instruction Set Computing):** Think of this as a "Swiss Army Knife." One instruction can do multiple things. This is the backbone of x64 (Intel/AMD) processors. It’s powerful but can be power-hungry.

**RISC (Reduced Instruction Set Computing):** This is the "Scalpel." It uses simple, uniform instructions that execute lightning-fast. This is the foundation of ARM (Advanced RISC Machine).

---

## 2. The Modern Era: ARM64 and x64

In my own tech, I checked my "System Type" and found out where I stand.

**x64** is the 64-bit evolution of the traditional CISC architecture. It’s what runs most high-end gaming rigs and servers.

**ARM64** is the modern 64-bit RISC architecture. It’s why the new Apple M-series chips and Snapdragon laptops have incredible battery life—they do more with less energy.

---

## 3. The "Reset": Quantum Computing

Then, I looked into the future. Quantum chips don't just use bits (0 or 1); they use Qubits. Unlike my laptop, which follows a linear path, a Quantum Processing Unit (QPU) uses "Quantum Gates" to manipulate probability.

### Key Technical Concepts I Uncovered:

- **Superposition:** A qubit can exist in a state of 0 and 1 simultaneously.  
- **Hadamard Gate (H-Gate):** This is the fundamental "randomizer." It puts a qubit into that 50/50 superposition state. Learn more about the Hadamard Gate.  
- **CNOT Gate (Controlled-NOT):** This is the "logic" of quantum. It flips a second qubit only if the first one is 1, creating entanglement. See CNOT Gate details.

---

## Final Thought

We aren't replacing x64 or ARM64 with Quantum. Instead, we are building a hybrid future. My ARM-based laptop might one day act as the "controller" for a QPU, offloading massive math problems to the quantum realm while keeping my UI smooth and efficient.

---

## Bonus: My Quantum "Hello World" (Using Qiskit)

To see a quantum chip in action, I looked at Qiskit, an open-source SDK from IBM. Instead of typing `print("Hello World")`, a quantum "Hello World" involves a tiny circuit that entangles two qubits so they stay perfectly in sync.

Here is what that looks like in code:

```python
from qiskit import QuantumCircuit

# 1. Create a circuit with 2 qubits
qc = QuantumCircuit(2)

# 2. Apply a Hadamard Gate to the first qubit
# This puts it into "Superposition" (50% 0, 50% 1)
qc.h(0)

# 3. Apply a CNOT Gate using qubit 0 to control qubit 1
# This "Entangles" them. If qubit 0 is 1, qubit 1 flips!
qc.cx(0, 1)

# 4. Result: A "Bell State" where both qubits are now linked.
print(qc)

###What’s actually happening here?
By using the H-Gate and CNOT Gate together, I created a Bell State. In this state, if you measure the first qubit and find it's a 1, the second qubit will instantly be a 1 too, even if they were on opposite sides of the universe.

---

It’s a far cry from the simple "Add 1+1" instructions in x64 or ARM64, but that’s the beauty of the "Tunnels" (Quantum Tunneling) era!
[IBM QuickStart](https://quantum.cloud.ibm.com/docs/en/guides/quick-start)


Initiated to reach the zenith
