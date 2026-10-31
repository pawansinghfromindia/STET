## Computer Organization

Q 1. What is the **primary difference between ROM and RAM**?
- [ ] A. ROM is faster than RAM
- [ ] B. ROM is volatile, while RAM is non-volatile
- [ ] C. ROM is used for data storage, while RAM is used ofr program execution
- [x] D. **ROM stores permanent data that can't be changed, while RAM stores temporary data that can be read and written**.

<details>
  <summary> <b> RAM vs ROM </b> </summary>

<br/>

The primary difference between ROM and RAM is that RAM is volatile memory, whereas ROM is non-volatile memory.

> **RAM = Volatile = Data lost when power is off.**

> **ROM = Non-volatile = Data retained when power is off.**

| Feature	              | RAM	                  | ROM                                        |
|-----------------------|-----------------------|--------------------------------------------|
| Full form	            | Random Access Memory	| Read Only Memory                           |
| Nature	              | Volatile	            | Non-volatile                               |
| Data after power off	| Lost	                | Retained                                   |
| Main purpose	        | Temporarily stores data and running programs	| Stores firmware and startup instructions|
| Access	              | Read and write	      | Primarily read; some types can be rewritten |
| Examples	            | DRAM, SRAM            | PROM, EPROM, EEPROM, Flash ROM             |

- When we open a browser, its running data is loaded into RAM.
- BIOS/UEFI firmware is stored in non-volatile memory (traditionally ROM or flash memory).

<img width="986" height="387" alt="image" src="https://github.com/user-attachments/assets/3c6072cb-0bb7-4e3c-b63e-2820cf23fef5" />


ROM stores permanent data, while RAM stores temporary data that can be read and written	Best answer among the options.
However, ROM is not necessarily unchangeable; flash ROM and EEPROM can be rewritten.
  
</details>
<!------------------------------>

Option C is partially correct! <br/>
ROM is used for data storage, while RAM is used for program execution	Partially correct, but it does not clearly explain 
volatility and data retention.

---

Q 2. Which components of an ideal microcomputer is responsible for temporarily holding data and instrcutions during processing?
- [ ] A. CPU
- [ ] B. ALU
- [x] C. **Memory**
- [ ] D. Output devices

<details>
  <summary> <b> Memory Unit (main memory/RAM) like buffer, register etc </b> </summary>

<br/>

The Memory Unit (main memory/RAM) temporarily holds data and instructions that the CPU needs while processing.

For example, when we open a program:
1. The program is loaded from secondary storage into RAM.
2. The CPU fetches instructions from memory.
3. The CPU processes those instructions.
4. Results may be stored back in memory.

| Component	 | Main function                                              |
|------------|------------------------------------------------------------|
| A. CPU	   | Executes instructions and controls computer operations.    |
| B. ALU	   | Performs arithmetic and logical operations.                |
| C. Memory	 | Temporarily holds data and instructions during processing. |
| D. Output devices	| Present processed information to the user.          |

  
</details>
<!------------------------------>

> - Memory: Stores data and instructions.
> - CPU: Processes instructions.
> - ALU: Performs calculations and logical comparisons.
> - Control Unit: Directs and coordinates operations.
> - Output Unit: Displays results.

---

Q 3. Which of the following application is a typical use of **micro-controllers** in the fields of home automation?
- [ ] A. Satellite communication
- [ ] B. Air Traffic control
- [x] C. Temperature and lighting control
- [ ] D. Space exploration

<details>
  <summary> <b> Micro-controllers </b> </summary>

<br/>

> A microcontroller (MCU) is a small, programmable computer built onto a single integrated circuit (IC).

- It is designed to control specific tasks in electronic devices and automated systems.

- Unlike a general-purpose computer, a microcontroller is usually designed for a dedicated function.

### 1. What does a microcontroller contain?

A microcontroller typically integrates three essential components: `CPU + Memory + peripherals`

<img width="320" height="317" alt="image" src="https://github.com/user-attachments/assets/202be427-e6ab-4b39-8fcf-f3d844ccfbc4" />


| Component	                    | Function
|-------------------------------|--------------------------------------------------------|
| **`CPU`**	                    | Executes instructions and controls operations.         |
| **`RAM`**	                    | Temporarily stores data during processing.             |
| **`ROM / Flash`**	            | Stores the program or firmware.                        |
| **`Input/Output (I/O) Ports`**|	Connect sensors, switches, displays and other devices. |
| **`Timers/Counters`**	        | Measure time and count events.                         |
| **`ADC`**	                    | Converts analog signals into digital values.           |
| **`Communication Interfaces`**|	Enable communication using UART, SPI, I2C, etc.        |

> Important: **A microcontroller integrates CPU, memory and peripherals into one chip**.

### 2. How does a microcontroller work in automation?

A microcontroller generally follows this cycle:

**1. Input**: Receives information from sensors.  <br/>
**2. Processing**: Executes its programmed instructions. <br/>
**3. Decision**: Determines what action should be performed. <br/>
**4. Output**: Controls motors, lights, alarms or other devices. <br/>


<img width="1075" height="737" alt="image" src="https://github.com/user-attachments/assets/cc314e75-c91f-429b-9cd6-97c7415da71f" />


Example: **Automatic street light**
- A light sensor detects darkness.
- The microcontroller processes the sensor reading.
- It switches ON the street light.
- When daylight returns, it switches OFF the light.

### 3. Applications of microcontrollers

**1. Home appliances**  <br/>
Washing machines, microwave ovens, refrigerators and air conditioners.


**2. Automobiles** <br/>
Engine control, airbags, parking sensors, ABS and automatic climate control.

**3. Industrial automation** <br/>
Robotic arms, conveyor belts, temperature control and machine monitoring.

**4. Agriculture** <br/>
Automatic irrigation, soil moisture monitoring and greenhouse control.

**5. Medical equipment** <br/>
Digital thermometers, blood pressure monitors and patient monitoring devices.

**6. Security systems** <br/>
Burglar alarms, access control, smart locks and motion detectors.

### 4. Popular microcontrollers

| Microcontroller|	Important features / Uses                                        |
|----------------|-------------------------------------------------------------------|
| 8051	         | Classic 8-bit microcontroller used in embedded systems education. |
| PIC	           | Microcontrollers developed by Microchip Technology.               |
| AVR	           | Used in Arduino boards such as Arduino Uno.                       |
| ARM Cortex-M	 | Common in modern embedded and real-time control systems.          |
| ESP32	         | Supports Wi-Fi and Bluetooth; used in IoT applications.           |
| ATmega328P	   | 8-bit AVR microcontroller used in Arduino Uno R3.                 |

### 5. Microcontroller vs Microprocessor

| Feature 	        | Microcontroller	                        | Microprocessor               |
|-------------------|-----------------------------------------|------------------------------|
| Integration    	  | CPU, memory and peripherals on one chip	| Primarily CPU on the chip    |
| Memory	          | Usually built-in RAM and program memory	| Usually uses external memory |
| Cost	            | Generally lower	                        | Generally higher system cost |
| Power consumption	| Generally low	                          | Generally higher             |
| Application	      | Dedicated control tasks	                | General-purpose computing    |
| Examples	        | `8051`, `PIC`, `ATmega328P`, `ESP32`    | `Intel Core`, `AMD Ryzen`    |

Q1. Which component is integrated into a microcontroller?
- [x] A. CPU, memory and I/O
- [ ] B. Only CPU
- [ ] C. Only RAM
- [ ] D. Only ALU

A microcontroller integrates a CPU, memory and peripherals on one chip.

Q2. Which microcontroller is used in Arduino Uno R3?
- [ ] A. 8051
- [x] B. ATmega328P
- [ ] C. Intel Core i5
- [ ] D. AMD Ryzen

Arduino Uno R3 uses the ATmega328P AVR microcontroller.

Q3. Which component detects physical conditions in automation?
- [ ] A. Actuator
- [x] B. Sensor
- [ ] C. Display
- [ ] D. Printer

A sensor detects conditions such as temperature, light or pressure.

Q4. Which is a common IoT microcontroller with Wi-Fi and Bluetooth?
- [ ] A. 8086
- [ ] B. 8051
- [x] C. ESP32
- [ ] D. Pentium

ESP32 includes wireless connectivity, including Wi-Fi and Bluetooth.

Q5. What is the primary purpose of a microcontroller?
- [ ] A. General-purpose computing
- [x] B. Dedicated control tasks
- [ ] C. Printing documents
- [ ] D. Storing large files

Microcontrollers are designed to control specific functions in embedded systems.
  
</details>
<!------------------------------>

> **Micro-controller is a mini-version of micro-processor.**

---

Q 4. For an ideal micro-computer, what is the **purpose of the clock or oscillator circuit**?
- [ ] A. Providing power to the micro-controller
- [ ] B. Displaying time and date information
- [x] C. Generating timing signals to synchronize operations
- [ ] D. cooling the micro-computer components

<details>
  <summary> <b> A clock or oscillator circuit </b> </summary>

<br/>

**A clock or oscillator circuit** generates regular electrical pulses called clock signals. <br/>
These signals synchronize the operations of different components of a microcomputer.

Think of it like a conductor directing an orchestra: every component performs its operation at the appropriate time.

How it works:
1. The oscillator generates a continuous sequence of pulses.
2. These pulses provide timing references to the CPU and other components.
3. The CPU uses clock cycles to coordinate instruction execution and internal operations.
4. The clock frequency determines how many clock cycles occur per second.

<img width="526" height="287" alt="image" src="https://github.com/user-attachments/assets/f6f9bba3-ccbd-4502-b639-5ae126c2c283" />

| Term	          | Meaning                                  |
| Clock signal	  | Periodic timing pulses                   |
| Oscillator	    | Circuit that generates a periodic signal |
| Clock frequency	| Number of clock cycles per second        |
| Hertz (Hz) 	    | Unit of frequency                        |
| 1 MHz	          | 1 million cycles per second              |
| 1 GHz	          | 1 billion cycles per second              |


Options and	Explanation
- A. Providing power,	The power supply provides electrical energy.
- B. Displaying time and date, 	A real-time clock (RTC) performs this function.
- C. Generating timing signals,	Correct. It synchronizes microcomputer operations.
- D. Cooling components	Cooling is handled by heat sinks, fans or other thermal solutions.
  
</details>
<!------------------------------>

> **Clock = Timing + Synchronization.**

---

Q 5. Which micro-controller family is known for its widespread use in embedded systems, ranging consumer electronic to
industrial automation?
- [ ] A. Intel 4004
- [x] B. ARM Cortex-M
- [ ] C. Intel 8086
- [ ] D. Motorola 68000

<details>
  <summary> <b> ARM Cortex-M family </b> </summary>

<br/>

The **ARM Cortex-M family** consists of processor cores designed specifically for microcontrollers and embedded applications.

They are widely used because they offer:
- Low power consumption.
- Good performance for control applications.
- Compact, cost-effective designs.
- Support for real-time embedded operations.

Examples of applications:
- Consumer electronics and smart appliances.
- Automotive control systems.
- Industrial automation and robotics.
- Medical devices and IoT products.

Options, Processor and Why it is incorrect?
- A	Intel 4004, An early 4-bit microprocessor, not a microcontroller family.
- B	ARM Cortex-M,	Designed for microcontroller and embedded applications.
- C	Intel 8086,	A 16-bit general-purpose microprocessor.
- D	Motorola 68000,	A general-purpose microprocessor family.
  
</details>
<!------------------------------>

---

Q 6. The micro-controller used in many **Arduino boards** is based on which architecture?
- [ ] A. ARM Cortext-A
- [ ] B. Intel x86
- [x] C. AVR
- [ ] D. Motorola 68000

<details>
  <summary> <b> Architecture used in Arduino boards - AVR </b> </summary>

<br/>

### AVR architecture

Many classic Arduino boards use microcontrollers based on the AVR architecture, developed by Atmel 
(now part of Microchip Technology).

For example:
- Arduino Uno R3 -> ATmega328P (8-bit AVR)
- Arduino Mega 2560 -> ATmega2560 (8-bit AVR)
- Arduino Nano (classic) -> ATmega328P (8-bit AVR)

The microcontroller executes the program (sketch) uploaded to the Arduino and controls connected sensors, LEDs, motors
and other devices.

<img width="1081" height="291" alt="image" src="https://github.com/user-attachments/assets/6614566c-bcf9-43c8-8838-1e679dc4a1f5" />


Optios, Architecture and Explanation

- A	ARM Cortex-A,	Designed mainly for application processors, such as those in smartphones and other advanced systems.
- B	Intel x86,	Common in PCs and general-purpose computing.
- C	AVR,	Used in classic Arduino boards such as Uno R3.
- D	Motorola 68000,	A general-purpose microprocessor architecture.
  
</details>
<!------------------------------>

---

Q 7. How does **Hamming Code** handle the correction of multiple errors?
- [x] A. It can't correct multiple errors
- [ ] B. It uses checksums to detect multiple errors
- [ ] C. It requires additional redundancy bits for each error
- [ ] D. It uses the parity bits to narrow down possible error possible error positions

<details>
  <summary> <b> Standard Hamming Code corrects only one-bit errors, not multiple-bit errors in general. </b> </summary>

<br/>

### 1. Concept: How Hamming Code works

Hamming Code is an error-detection and error-correction technique used in digital communication and computer memory.

It adds extra bits called parity bits to the original data bits.

The parity bits are placed at positions that are powers of 2:

`1, 2, 4, 8, 16, ...`

When data is received, the parity checks are performed again. 
Their combined results form a syndrome, which identifies the position of a single-bit error.


| Code	                         | Capability                 |
|--------------------------------|----------------------------|
| Standard Hamming Code	         | Corrects single-bit errors |
| Extended Hamming Code (SECDED) | Corrects single-bit errors and detects double-bit errors |
| Multiple-bit error correction	 | Requires stronger error-correcting codes, depending on the number of errors |
  
</details>
<!------------------------------>

> - Hamming Code -> Single-bit correction.
> - Extended Hamming Code -> Single-bit correction + double-bit detection.
> - Syndrome -> Identifies the erroneous bit position.

---

Q 8. In a micro-computer system, what does the **address bus facilitates**?
- [x] A. Communication between CPU and memory
- [ ] B. Communication between CPU and input device
- [ ] C. Communication between CPU and output device
- [ ] D. Communication between memory and input device 

<details>
  <summary> <b> Function of the address bus: Communication between CPU and memory </b> </summary>

<br/>

### 1. Address bus

The address bus carries the address of the memory location or I/O port that the CPU wants to access.

For example, when the CPU wants to read data from memory location 2000, it places address 2000 on the address bus.

The **address bus tells the system where to access data, not what the data is**.

<img width="796" height="397" alt="image" src="https://github.com/user-attachments/assets/7a5d8d1d-97c6-4c3a-918c-0e8450f25999" />


### 2. Understand the three buses

| Bus	                | Main function	                                 | Direction                    |
|---------------------|------------------------------------------------|------------------------------|
| **1. Address bus**	| Carries the address/location	                 | Usually CPU -> memory or I/O |
| **2. Data bus**	    | Carries actual data	                           | Usually bidirectional        |
| **3. Control bus**	| Carries control signals such as Read and Write | Depends on signal            |

Example: Reading data from memory
1. CPU places the memory address on the address bus.
2. CPU sends a Read signal through the control bus.
3. Memory sends the requested data through the data bus.
  
</details>
<!------------------------------>

> - Address bus = WHERE (Carries the address/location)
> - Data bus = WHAT (Carries actual data)
> - Control bus = HOW (Carries control signals such as Read and Write)

---

Q 9. Which company introduced the first commercially avaiable micro-processor, the Intel 4004, in 1971?
- [ ] A. IBM
- [ ] B. Motorola
- [x] C. Intel
- [ ] D. Texas Instruments

<details>
  <summary> <b> Intel </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 10. How is **the width of the data bus typically measured in a micro-computer system**?
- [ ] A. in Kilobytes(KB)
- [ ] B. in MegaHertz(MHz)
- [x] C. in Bits
- [ ] D. in Address lines

<details>
  <summary> <b> Data bus = WHAT (Carries actual data) in bits </b> </summary>

<br/>

The data bus width refers to the number of bits that can be transferred simultaneously between the CPU, memory and 
other components.

For example:
- 8-bit data bus  -> transfers 8 bits at a time.
- 16-bit data bus -> transfers 16 bits at a time.
- 32-bit data bus -> transfers 32 bits at a time.
- 64-bit data bus -> transfers 64 bits at a time.

Options and	Explanation
- A. Kilobytes (KB),	Measures data storage or size, not bus width.
- B. MegaHertz (MHz),	Measures frequency, such as clock frequency.
- C. Bits,	Correct! Measures how many bits can be transferred simultaneously.
- D. Address lines,	Determine the address space, not the data bus width.
  
</details>
<!------------------------------>

> - Data bus width -> `Bits`
> - Address bus width -> `Number of address lines`
> - Clock speed -> `Hz, MHz or GHz`
> - Memory capacity -> `Bytes, KB, MB or GB`

---

Q 11. Micro-controllers find application in various fields. What is a typical application of **micro-controllers in the 
automative industry**?
- [ ] A. Operating System for computers
- [ ] B. Entertainment system in airplanes
- [x] C. Engine control cars
- [ ] D. Weather forecasting system

<details>
  <summary> <b> Microcontrollers in the automotive industry </b> </summary>

<br/>

Microcontrollers are widely used in cars to monitor and control different operations.

A major application is the **Engine Control Unit (ECU)**.

The ECU uses a microcontroller to:
- Monitor engine temperature.
- Control fuel injection.
- Manage ignition timing.
- Monitor engine speed.
- Improve engine performance and fuel efficiency.

Automotive applications:
- ECU -> Engine control.
- ABS -> Anti-lock braking system.
- Airbag controller -> Safety system.
- Cruise control -> Maintains vehicle speed.

Options and	Explanation
- A. Operating System for computers,	General-purpose computer software, not a typical automotive microcontroller application.
- B. Entertainment system in airplanes,	An aviation application, not an automotive one.
- C. Engine control in cars,	Correct! Microcontrollers manage engine operations through the ECU.
- D. Weather forecasting system,	Primarily uses larger computing systems and weather models.
  
</details>
<!------------------------------>

> Automotive applications:
> - ECU -> Engine control.
> - ABS -> Anti-lock braking system.
> - Airbag controller -> Safety system.
> - Cruise control -> Maintains vehicle speed.

---

Q 12. What is the **primary role of the memory-mapped I/O techniques in a micro-controller**?
- [ ] A. It increases the speed of program execution.
- [ ] B. It provides additional memory space for data storage.
- [x] C. It allows external devices to access the micro-controller's memory
- [ ] D. It eliminates the need of I/O Operations

<details>
  <summary> <b> It allows external devices to access the microcontroller's memory. </b> </summary>

<br/>

More precisely, memory-mapped I/O assigns specific memory addresses to I/O device registers, allowing the CPU to 
communicate with peripherals using ordinary memory read/write instructions.

### 1. Concept: Memory-mapped I/O

Normally, a microcontroller has memory (RAM/Flash) and peripherals such as GPIO ports, timers and UART.

In memory-mapped I/O, peripheral registers are assigned addresses within the processor's memory address space.

For example:
- Address 0x2000 -> RAM location.
- Address 0x4000 -> GPIO control register (illustrative address).

</details>
<!------------------------------>

> - Memory-mapped I/O -> I/O registers share the memory address space.
> - Isolated I/O -> Separate I/O address space and special I/O instructions (in architectures that support it).

---

Q 13. Which addressing mode involves specifying a value within the instruction itself, rather than referencing a memory 
location?
- [ ] A. Direct Addressing
- [x] B. Immediate addressing
- [ ] C. Indirect addressing
- [ ] D. Index addressing

<details>
  <summary> <b> addressing mode  </b> </summary>

<br/>

| Addressing mode	|  How the operand is obtained	                        | Example            |
|-----------------|-------------------------------------------------------|--------------------|
| Immediate	      | Value is inside the instruction	                      | `MOV R1, #25`      |
| Direct	        | Instruction specifies the memory address	            | `LOAD R1, 2000`    |
| Indirect        | Address is obtained through another location/register	| `LOAD R1, [R2]`    |
| Indexed	        | Effective address is calculated using an index	      | `LOAD R1, [R2 + 4]`|

Remember:
- Immediate = Value directly given.
- Direct = Address directly given.
- Indirect = Address obtained indirectly.
- Indexed = Address calculated using an index.
  
</details>
<!------------------------------>

Remember:
> - Immediate = Value directly given.
> - Direct = Address directly given.
> - Indirect = Address obtained indirectly.
> - Indexed = Address calculated using an index.

---

Q 14. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>


---

Q 15. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 16. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 17. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 18. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 19. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 20. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 21. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 22. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 23. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 24. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 25. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 26. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 27. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 28. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 29. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 30. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>

---

Q 31. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> <b> </b> </summary>

<br/>
  
</details>
<!------------------------------>
