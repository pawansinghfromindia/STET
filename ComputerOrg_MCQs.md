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
> - Immediate = Value directly given in the instructions.
> - Direct = Address of data directly given as memory(data).
> - Indirect = Address obtained indirectly like one memory(add) contains effective memory(data).
> - Indexed = Address calculated using an index. Add(instruction)+index register value

---

Q 14. In an ideal micro-computer, where is the **Arithmetic Logic Unit(ALU) located**?
- [x] A. CPU
- [ ] B. Memory
- [ ] C. Input devices
- [ ] D. Output devices

<details>
  <summary> <b> CPU = ALU + CU + Registers </b> </summary>

### Arithmetic Logic Unit (ALU)

The ALU is a major component of the CPU responsible for performing arithmetic and logical operations.

Arithmetic operations:
- Addition (+)
- Subtraction (−)
- Multiplication (×)
- Division (÷)

Logical operations:
- AND
- OR
- NOT
- XOR
- Comparisons (greater than, less than, equal to)

<img width="352" height="317" alt="image" src="https://github.com/user-attachments/assets/91b8336f-bebe-4f1a-b10c-21288f94ae01" />

### 2. CPU components

| Component	            | Main function                              |
|-----------------------|--------------------------------------------|
| **ALU**	              | Performs arithmetic and logical operations |
| **Control Unit (CU)** | Controls and coordinates CPU operations    |
| **Registers**	        | Temporarily store data and instructions    |

<br/>
  
</details>
<!------------------------------>

> CPU components = ALU + CU + Registers
> - ALU = Calculations and Logic; CU = Control; Registers = Temporary storage.

---

Q 15. In which year did the intel release the first x86 micro-processor, the x86 (8086), which laid the foundation for the x86 
architecture widely used in personal computers?
- [ ] A. 1971
- [x] B. 1981
- [ ] C. 1986
- [ ] D. 1991

<details>
  <summary> <b> The Intel 8086 was released by Intel in 1978 , So ~1981 </b> </summary>

<br/>

### 1. Concept: Intel 8086 microprocessor

The Intel 8086 was released by Intel in 1978. <br/>
It was a 16-bit microprocessor and established the foundation of the x86 instruction-set architecture.

<img width="387" height="316" alt="image" src="https://github.com/user-attachments/assets/efcf09d6-5441-4e42-80c6-3c7d10d535ce" />

### 2. Intel processor timeline

| Year	| Processor	  | Significance                                |
|-------|-------------|---------------------------------------------|
| 1971	| Intel 4004	| First commercial single-chip microprocessor | 
| 1972	| Intel 8008	| Early 8-bit microprocessor                  |
| 1974	| Intel 8080	| Popular 8-bit microprocessor                |
| 1978	| Intel 8086	| Beginning of the x86 architecture           |
| 1979	| Intel 8088	| Used in the original IBM PC (1981)          |
  
</details>
<!------------------------------>

> - 1971 -> Intel 4004 (First commercial single-chip microprocessor)
> - 1978 -> Intel 8086 (Beginning of the x86 architecture)

---

Q 16. What is the relationship between the distance between parity bits and their error detectation and correction capability
in Hamming code?
- [ ] A. Closer parity bits provide higher error correction capability
- [x] B. Closer parity bits provide lower error correction capability
- [ ] C. Distance between parity bits has no impact on error correction capability
- [ ] D. The position of parity bits is irrelevant in Hamming code 

<details>
  <summary> <b> Closer parity bits provide lower error correction capability in Hamming Code </b> </summary>

<br/>

In Hamming Code, parity-bit positions and coverage patterns matter, not simply the physical distance between parity bits.

### 1. Concept: Parity-bit placement in Hamming Code

In Hamming Code, parity bits are placed at positions that are powers of 2: `1, 2, 4, 8, 16`

Each parity bit checks a specific group of bit positions.

For example, in a 7-bit Hamming Code:

| Position	| Bit type |
| 1	        | P1       |
| 2	        | P2       |
| 3	        | Data     |
| 4         | P4       |
| 5	        | Data     |
| 6	        | Data     |
| 7	        | Data     |

Each parity bit covers a different combination of positions. <br/>
Together, their results produce a syndrome that identifies a single-bit error.
  
</details>
<!------------------------------>

---

Q 17. **EBCDIC** is mainly used in which type of computer system?
- [x] A. Mainframe computers
- [ ] B. Personal computers
- [ ] C. Super computers
- [ ] D. Mobile devices

<details>
  <summary> <b> EBCDIC, ASCII, Unicode (UTF-8, UTF-16) </b> </summary>

<br/>

### 1. Concept: EBCDIC

EBCDIC stands for Extended Binary Coded Decimal Interchange Code.

It is an 8-bit character encoding system developed by IBM and is mainly associated with IBM mainframe and midrange computer systems.

It represents characters such as:
- `A–Z (uppercase letters)`
- `0–9 (digits)`
- `Special symbols and punctuation`

Option and Explanation
- A. Mainframe computers,	Correct! `EBCDIC` is traditionally used in IBM mainframe environments.
- B. Personal computers,	`ASCII` and `Unicode` are more commonly used.
- C. Supercomputers, Generally use modern character encoding standards such as `ASCII` and `Unicode`.
- D. Mobile devices,	Primarily use `Unicode`, especially `UTF-8` and `UTF-16`.


### 3. EBCDIC vs ASCII

| Feature	        | EBCDIC	        | ASCII                     |
|-----------------|-----------------|---------------------------|
| Full form	      | Extended Binary Coded Decimal Interchange Code	| American Standard Code for Information Interchange |
| Original design	| IBM	            | ANSI                      |
| Common use	    | IBM mainframes	| General-purpose computing | 
| Standard size	  | 8 bits 	        | Originally 7 bits         |

  
</details>
<!------------------------------>

> - `EBCDIC` **Extended Binary Coded Decimal Interchange Code**, used in IBM mainframe environments
> - `ASCII` -> Traditional character encoding in computers, 
> - `Unicode` (`UTF-8`, `UTF-16`) -> Modern multilingual text representation


---

Q 18. Which method is used to transfer small amount of data between the CPU and I/O device using programmed I/O?
- [ ] A. Polling
- [ ] B. DMA
- [ ] C. Interrupt-Driven I/O
- [c] D. Parallel I/O

<details>
  <summary> <b> </b> </summary>

<br/>

Options, Method and Explanation

- A	Polling, Correct! CPU repeatedly checks device status and performs the transfer.
- B	DMA, Transfers data directly between memory and I/O devices with minimal CPU involvement.
- C	Interrupt-driven I/O,	The device interrupts the CPU when it needs attention.
- D	Parallel I/O,	Refers to transferring multiple bits simultaneously, not the programmed I/O control method.

### Transfer Mode

| I/O method	              | Who controls the transfer?	| Key feature                                        |
|---------------------------|-----------------------------|----------------------------------------------------|
| Programmed I/O (Polling)	| CPU	                        | CPU repeatedly checks device status.               |
| Interrupt-driven I/O	    | CPU, notified by device	    | Device generates an interrupt.                     |
| DMA	                      | DMA controller	            | Data transfers directly between memory and device. |
  
</details>
<!------------------------------>

> Transfer Mode:
> 1. Programmed I/O (Polling), CPU repeatedly checks device status.
> 2. Interrupt-driven I/O, Device generates an interrupt.
> 3. DMA, Data transfers directly between memory and device

> - Polling -> CPU keeps checking.
> - Interrupt -> Device informs CPU.
> - DMA -> Direct memory transfer.

---

Q 19. What does the term **Harvard architecture** refers to in the context of micro-controller?
- [ ] A. A type of micro-controller with high processing speed.
- [x] B. A micro-controller architecture that uses a separate memory space for instructions and data
- [ ] C. A micro-controller with advanced addressing modes
- [ ] D. A micro-controller with a large number of I/O ports

<details>
  <summary> <b> </b> </summary>

<br/>

### Harvard vs Von Neumann Architecture

| Feature	                                 | Harvard Architecture	       | Von Neumann Architecture  |
|------------------------------------------|-----------------------------|---------------------------|
| Instruction memory	                     | Separate	Instruction memory | Shared Instruction memory |
| Data memory	                             | Separate	Data memory	       | Shared Data memory        |	
| Buses	                                   | Separate	Buses              | Shared Buses              |
| Simultaneous instruction and data access | Possible	                   | Typically limited by shared bus |
| Common application	                     | Many microcontrollers	     | General-purpose computer systems |
  
</details>
<!------------------------------>

> - Harvard Architecture = Separate instruction and data memory.
> - Von Neumann Architecture = Shared instruction and data memory.

---

Q 20. Which **error-detection technique** generally provide stronger detection of burst errors?
- [ ] A. Simple parity checking
- [ ] B. Decimal number conversion
- [x] C. Cyclic Redundance check
- [ ] D. Gray code conversion

<details>
  <summary> <b> Cyclic Redundancy Check (CRC) </b> </summary>

<br/>

###  Cyclic Redundancy Check (CRC)

CRC is an error-detection technique widely used in computer networks, data communication and storage devices.

It is particularly effective at detecting burst errors, where multiple consecutive bits are corrupted during transmission.

How does CRC work?
1. Sender treats the data as a binary polynomial.
2. It divides the data by a predefined generator polynomial using modulo-2 division (XOR).
3. The remainder is appended to the original data.
4. Receiver performs the same division.
5. A non-zero remainder indicates an error.

<img width="502" height="337" alt="image" src="https://github.com/user-attachments/assets/f35d48f9-bab4-43a5-9987-d2f242273ff9" />


Options, Techniques and Explanation
- A.	Simple parity, checking	Detects odd numbers of bit errors but can miss even numbers of errors.
- B.	Decimal number conversion,	Not an error-detection technique.
- C.	CRC,	Correct! Provides strong detection of burst errors.
- D.	Gray code conversion,	Reduces bit changes between consecutive values; not primarily an error-detection method.

Which operation is primarily used in CRC modulo-2 division?
- [ ] A. Decimal addition
- [x] B. Binary XOR
- [ ] C. Binary multiplication with carries
- [ ] D. Decimal subtraction

> **CRC uses XOR (Exclusive OR) for modulo-2 division.**

Remember the XOR rules:
| A	| B	| A XOR B|
|---|---|--------|
| 0	| 0	| 0      |
| 0	| 1	| 1      |
| 1	| 0	| 1      |
| 1	| 1	| 0      |
  
</details>
<!------------------------------>

> - **Parity Check**: Simple error detection.
> - **Checksum**: Error detection in data communication.
> - **CRC(Cyclic Redundancy Check)**: Strong burst-error detection.
> - **Hamming Code**: Error detection and correction.

> CRC uses **XOR (Exclusive OR) for modulo-2 division**.


---

Q 21. A cache has 64 lines and uses direct mapping. Which cache line is selected for memory block 150?
- [ ] A. Line 20
- [x] B. Line 22
- [ ] C. Line 24
- [ ] D. Line 26

<details>
  <summary> <b> Direct-Mapped Cache </b> </summary>

<br/>

### Direct-Mapped Cache

In a direct-mapped cache, each main-memory block can be stored in exactly one specific cache line.

The formula is: **`Cache line = Memory block number mod Number of cache lines`**
```
Given:
- Number of cache lines = 64
- Memory block number = 150
Calculation by formula:
      Cache line = Memory block number mod Number of cache lines
                 = 150 % 64
                 = 22          [ 64 x 2 + 22 = 150]

```
  
</details>
<!------------------------------>

> For direct mapping: `cache line = Block mod cache size`

---

Q 22. Which component stores the micro-instructions of a micro-programmed control unit?
- [ ] A. cache memory
- [ ] B. main memory
- [x] C. control memory
- [ ] D. register memory

<details>
  <summary> <b> Micro-programmed Control Unit </b> </summary>

<br/>

### Micro-programmed Control Unit

A micro-programmed control unit generates control signals using small instructions called micro-instructions.

These micro-instructions are stored in a special memory called Control Memory (also known as Control Store).

1. The control unit selects the required micro-instruction.
2. It fetches that micro-instruction from control memory.
3. The micro-instruction generates control signals.
4. These signals coordinate CPU operations.

<img width="1037" height="542" alt="image" src="https://github.com/user-attachments/assets/23453e9f-b18d-4f3d-8441-fa377e787d98" />


**Component	and Function**
- Cache memory,	Stores frequently accessed instructions and data.
- Main memory,	Stores programs and data currently in use.
- Control memory,	Stores micro-instructions.
- Register memory, Not the standard name for the memory storing microcode.

| Control unit type	            | How control signals are generated           |
|-------------------------------|---------------------------------------------|
| Hardwired control unit	      | Fixed logic circuits                        |
| Micro-programmed control unit	| Micro-instructions stored in control memory |

> **Micro-programmed Control Unit -> Micro-instructions -> Control Memory.**
  
</details>
<!------------------------------>

> - Micro-programmed Control Unit -> Micro-instructions -> Control Memory.

---

Q 23. In Cyclic Redundancy Check(CRC), error detection is based on:
- [x] A. Binary division using a generator polynomial.
- [ ] B. Decimal Addition using a caary bit
- [ ] C. Parity checking using a single bit
- [ ] D. Data comparison using memory address

<details>
  <summary> <b> Binary division using a generator polynomial </b> </summary>

<br/>

CRC (Cyclic Redundancy Check) detects errors using modulo-2 binary division with a predefined generator polynomial.

Suppose a sender wants to transmit data:
1. The sender selects a generator polynomial, represented as a binary bit pattern.
2. It appends zeros to the data, according to the degree of the generator polynomial.
3. It performs modulo-2 division (binary division using XOR, without carries or borrows).
4. The remainder is appended to the original data. This remainder is called the CRC bits.
5. The receiver divides the received data by the same generator polynomial.
6. If the remainder is zero, no error is detected. A non-zero remainder indicates an error.
  
</details>
<!------------------------------>

> CRC (Cyclic Redundancy Check) detects errors using modulo-2 binary division with a predefined generator polynomial.

> - Parity: Checks whether the number of 1s is even or odd.
> - Checksum: Uses arithmetic sums to detect errors.
> - CRC: Uses modulo-2 binary division with a generator polynomial.

---

Q 24. In which addressing mode is the operand stored in a CPU register specified in the instruction?
- [ ] A. Direct addressing
- [x] B. Register addressing
- [ ] C. Immediate addressing
- [ ] D. Indexed addressing

<details>
  <summary> <b> Register addressing </b> </summary>

<br/>

In register addressing mode, the operand is stored in a CPU register, and the instruction specifies which register contains the operand.

**Understand the concept with an example** <br/>
Consider this 8086-style instruction:
```asm
MOV AX, BX
```
- `AX` is the destination register.
- `BX` is the source register.
- The CPU copies the value stored in `BX` into `AX`.
Here, the operand is obtained from a CPU register, so this is register addressing.

| Addressing mode |	Where is the operand?                                    |
|-----------------|----------------------------------------------------------|
| Direct	        | At the memory address specified in the instruction.      |
| Register	      | In the CPU register specified in the instruction.        |
| Immediate	      | The actual data value is part of the instruction itself. |
| Indexed	        | At a memory location calculated using an index register and usually a displacement. |

Remember these four distinctions:
- Immediate: Value is inside the instruction.
- Register: Value is inside a CPU register.
- Direct: Memory address is given directly.
- Indexed: Index register helps calculate the memory address.
  
</details>
<!------------------------------>

> Four distinctions:
> - Immediate: Value is inside the instruction.
> - Register: Value is inside a CPU register.
> - Direct: Memory address is given directly.
> - Indexed: Index register helps calculate the memory address.

---

Q 25. Which **cache mapping technique** allows a main memory block to be placed in **any cache line**?
- [ ] A. Direct mapping
- [x] B. Associative mapping
- [ ] C. Set-associateive mapping
- [ ] D. Sequential mapping

<details>
  <summary> <b> Associative mapping </b> </summary>

<br/>

In associative mapping, a main memory block can be placed in any available cache line.

The cache controller searches the cache tags to determine whether the required block is present.

### 3 cache mapping techniques

**A. Direct mapping**
> Each main memory block maps to exactly one specific cache line.

Example: Block 10 may be assigned only to cache line 2.

**B. Associative mapping**
> A memory block can be placed in any cache line, provided space is available.

Example: Block 10 can be placed in line 0, 1, 2, or any other line.

**C. Set-associative mapping**
> A memory block maps to one specific set, but can occupy any line within that set.

Example: Block 10 maps to set 2, and can occupy any line within set 2.
  
</details>
<!------------------------------>

The the placement rule:
> - Direct: One specific line.
> - Associative: Any line.
> - Set-associative: Any line within one specific set.

---

Q 26. Which statement correctly distinguish intrupt-driven I/O from programmed I/O?
- [ ] A. Interrupt-driven I/O requires continuous status checking
- [ ] B. Programmed I/O always transfer data directly to memory
- [x] C. Interrupt driven I/O can notify the CPU when service is needed
- [ ] D. Program I/O never involve the CPU

<details>
  <summary> <b> I/O techniques </b> </summary>

<br/>

### I/O techniques

**Programmed I/O (Polling)**
- The CPU repeatedly checks the device's status.
- If the device is ready, the CPU performs the data transfer.
- The CPU remains involved in checking and managing the operation.

<img width="770" height="346" alt="image" src="https://github.com/user-attachments/assets/3b01bae5-daf9-424e-94a0-db24c5343521" />


**Interrupt-driven I/O**
- The CPU starts an I/O operation and continues doing other work.
- When the device needs attention or is ready, it sends an interrupt signal.
- The CPU temporarily pauses its current work, executes the **Interrupt Service Routine (ISR)**, and then resumes.

<img width="757" height="332" alt="image" src="https://github.com/user-attachments/assets/1c5c5a82-9187-4d54-95ec-6ab8091ae3f1" />


| Technique	                  | Main responsibility                               |
|-----------------------------|---------------------------------------------------|
| Programmed I/O(Polling)     | CPU repeatedly checks and manages transfer        |
| Interrupt-driven I/O	      | Device interrupts CPU when service is needed      |
| DMA(Data Memory Allocation) |	Transfers data directly between device and memory |

Which I/O technique transfers data directly between an I/O device and main memory with minimal CPU involvement?
- [ ] A. Programmed I/O
- [ ] B. Interrupt-driven I/O
- [x] C. DMA (Direct Memory Access)
- [ ] D. Polling

DMA allows data to move directly between an I/O device and main memory without the CPU managing every byte or word transferred.
  
</details>
<!------------------------------>

> - Polling(Programmed I/O): CPU keeps checking.
> - Interrupt(Interrupt-driven I/O): Device alerts the CPU.
> - DMA (Direct Memory Access): Data transfers directly between device and memory with minimal CPU involvement.

---

Q 27. In relative addressing, the effective address is generally calculated using:
- [x] A. Program counter and displacement 
- [ ] B. Accumulator and operand
- [ ] C. Stack pointer and opcode
- [ ] D. Instruction register and data

<details>
  <summary> <b> </b> </summary>

<br/>

### 1. Relative addressing

In relative addressing mode, the effective address is calculated by adding the displacement (offset) to the contents of the Program Counter (PC).

**`Effective Address = PC + Displacement`**

For example:
```
- Program Counter = 1000
- Displacement = 50
- Effective Address = 1050
```
The CPU calculates the target address relative to the current instruction position.

</details>
<!------------------------------>

Remember these addressing modes:
- Immediate addressing: Operand value is inside the instruction.
- Direct addressing: Address is specified in the instruction.
- Indirect addressing: Address field points to a location containing the effective address.
- Register addressing: Operand is in a CPU register.
- Relative addressing: PC + displacement.
- Indexed addressing: Index register + displacement/base address.

---

Q 28. Which addressing mode is commonly used for **Branching and jumb to subroutine execution**?
- [ ] A. Immediate addressing
- [x] B. Relative addressing
- [ ] C. Direct addressing
- [ ] D. Indexed addressing

<details>
  <summary> <b> Relative addressing </b> </summary>

<br/>

Relative addressing is commonly used in branch instructions and subroutine calls, particularly when the target address is calculated relative to the Program Counter (PC).

The target address is calculated as: `Target Address = PC + Displacement`

For example:
```
- PC = 1000
- Displacement = 200
- Target address = 1200
```
The CPU can branch to the target location without storing its complete absolute address in the instruction.

Note: Branches and subroutine calls can also use absolute or indirect addressing, depending on the processor architecture. Relative addressing is a common technique, not the only one.

Options and Explanation
- A. Immediate addressing,	The operand value is included directly in the instruction.
- B. Relative addressing,	Correct! Commonly used for PC-relative branches and calls.
- C. Direct addressing,	Specifies an address directly rather than calculating it relative to PC.
- D. Indexed addressing,	Uses an index register to calculate an effective address, commonly for arrays and tables.

Which register generally contains the address of the next instruction to be fetched?
- [ ] A. Accumulator
- [x] B. Program Counter
- [ ] C. Instruction Register
- [ ] D. Stack Pointer

|      Register	                |             Main function                                  |
|-------------------------------|------------------------------------------------------------|
| **Program Counter (PC)**	    | Holds the address of the next instruction to be fetched.   |
| **Instruction Register (IR)**	| Holds the instruction currently being decoded or executed. |
| **Accumulator**	              | Stores intermediate arithmetic and logical results.        |
| **Stack Pointer (SP)**	      | Points to the top of the stack.                            |

> PC(Program Counter) = Where to fetch the next instruction
> IR(Instruction Register) = Which instruction is currently being processed

</details>
<!------------------------------>

> - Branching -> Relative addressing
> - Array access -> Indexed addressing
> - Constant value -> Immediate addressing
> - Operand in register -> Register addressing

---

Q 29. In an instruction using immediate addressing, the operand is:
- [ ] A. stored in CPU register
- [ ] B. located through a pointer
- [x] C. included within the instruction
- [ ] D. retrieve from a stack

<details>
  <summary> <b> Immediate addressing - operand is included within the instruction  </b> </summary>

<br/>

In immediate addressing mode, the actual operand value is provided directly as part of the instruction.

Example
```asm
MOV AX, 25
```
- `MOV` -> Instruction
- `AX` -> Destination register
- `25` -> Immediate operand (actual value)

The CPU does not need to fetch the operand from another memory location.


Options and	Explanation
- A. Stored in CPU register, 	Register addressing mode.
- B. Located through a pointer,	Indirect addressing mode.
- C. Included within instruction,	Correct! immediate addressing.
- D. Retrieved from a stack,	Stack addressing mode.


| Mode	    | Operand location                   |
|-----------|------------------------------------|
| Immediate	| Inside instruction                 |
| Register	| CPU register                       |
| Direct	  | Memory address specified           |
| Indirect	| Address obtained through a pointer |
| Relative	| PC + displacement                  |
| Indexed	  | Index register + displacement      |

Consider the instruction: `MOV BX, 50`, Which addressing mode is used for the source operand 50?
- [ ] A. Direct addressing
- [ ] B. Register addressing
- [x] C. Immediate addressing
- [ ] D. Indirect addressing
  
</details>
<!------------------------------>

> Immediate = actual value is included in the instruction.

---

Q 30. Which error detection methods adds an extra bit to a data unit to make the number of 1s even or odd?
- [ ] A. Checksum
- [ ] B. Hamming code
- [x] C. Parity bit method
- [ ] D. CRC Method

<details>
  <summary> <b> Parity bit method </b> </summary>

<br/>

The parity bit method adds one extra bit to a data unit so that the total number of 1s becomes either even or odd.

There are two types:
- Even parity: Total number of 1s must be even.
- Odd parity: Total number of 1s must be odd.

<img width="1072" height="601" alt="image" src="https://github.com/user-attachments/assets/860fc9bf-2e3a-466d-95d6-4d9f4748fb74" />

| Method	              | Purpose                                                         |
|-----------------------|-----------------------------------------------------------------|
| A. Checksum	          | Uses arithmetic operations to detect data errors.               |
| B. Hamming code	      | Uses multiple parity bits to locate and correct certain errors. |
| C. Parity bit method	| Adds an extra bit to achieve even or odd parity.                |
| D. CRC	              | Uses modulo-2 binary division with a generator polynomial.      |
  
</details>
<!------------------------------>

> - Parity bit: Adds one bit.
> - Hamming code: Multiple parity bits; standard Hamming code can correct single-bit errors.
> - Checksum: Arithmetic-based error detection.
> - CRC: Generator polynomial and binary division.

---

Q 31. In an **even-parity system**, the data bits are `1011001`. What should be the parity bit?
- [x] A. 0
- [ ] B. 1
- [ ] C. 10
- [ ] D. 11

<details>
  <summary> <b> Even-parity system, Odd-parity system </b> </summary>

<br/>

In an even-parity system, the total number of 1s in the data bits plus the parity bit must be even.

Given data: `1011001`
```
Count the number of 1s:
- Total number of 1s = 4
- 4 is already an even number.
- Therefore, the parity bit must be 0.
```
Final transmitted data: `10110010` <br/>
Total number of 1s remains 4 (even).

> - Even number of 1s -> Parity bit 0 for even parity.
> - Odd number of 1s -> Parity bit 1 for even parity.

Trick: **Count the 1s first. If their count is already even, add 0; otherwise, add 1.**
  
</details>
<!------------------------------>

> - Even number of 1s -> Parity bit 0 for even parity.
> - Odd number of 1s -> Parity bit 1 for even parity.

Trick: **Count the 1s first. If their count is already even, add 0; otherwise, add 1.**

---

Q 32. Which statement about a **single parity bit** is correct?
- [ ] A. It corrects all single-bit errors
- [ ] B. It detects every possible burst error
- [ ] C. It detects any even number of bit errors
- [x] D. It detects any odd number of bit errors

<details>
  <summary> <b> Single parity bit </b> </summary>

<br/>

A single parity bit is used to detect errors by checking whether the total number of 1s is even or odd.

The important principle is:
- An odd number of bit flips changes the parity, so an error is detected.
- An even number of bit flips preserves the parity, so the error may go undetected.

<img width="1092" height="615" alt="image" src="https://github.com/user-attachments/assets/2a6c8f8e-3aed-4fe9-925b-2ed61567efc0" />

  
</details>
<!------------------------------>

> Single parity bit = Error detection, not error correction.

---

Q 33. The **checksum method** generally detects transmission errors by:
- [ ] A. Adding a parity bit to every bit
- [x] B. computing a sum of data segments
- [ ] C. reversing the transmitted data
- [ ] D. inserting redundant address bits

<details>
  <summary> <b> Checksum method </b> </summary>

<br/>

The checksum method detects transmission errors by dividing data into segments (commonly fixed-size words) and calculating their sum.

The sender and receiver independently calculate or verify the checksum to identify possible corruption.

**Understand with an example**

Suppose the sender divides data into three 8-bit segments:
```
Segment 1: 00000101  (5)
Segment 2: 00000011  (3)
Segment 3: 00000010  (2)
                  ----
Sum:              10
```
The sender calculates a checksum from the sum and transmits it along with the data.

At the receiver's end:
1. The received data segments are added.
2. The checksum is included in the verification.
3. If the result satisfies the checksum rule, the data passes the check; otherwise, an error is indicated.

Note: Internet checksums commonly use one's-complement addition and transmit the one's-complement of the sum.

| Technique	    | Main principle                                      |
|---------------|-----------------------------------------------------|
| Parity	      | Even/odd number of 1s                               |
| Checksum	    | Addition of data segments                           |
| CRC	          | Modulo-2 binary division                            |
| Hamming code	| Multiple parity bits; can correct single-bit errors |

Which error-detection method uses a generator polynomial and modulo-2 division?
- [ ] A. Checksum
- [ ] B. Parity bit
- [x] C. CRC(Cyclic Redundancy Check)
- [ ] D. Hamming code

CRC uses modulo-2 binary division with a generator polynomial to detect transmission errors.
  
</details>
<!------------------------------>

> Remember the four methods:
> - Parity -> Counts 1s.
> - Checksum -> Adds data segments.
> - CRC -> Binary division using XOR.
> - Hamming code -> Uses parity bits to locate and correct single-bit errors.

---

Q 34. Which technique is commonly used to locate and correct a single-bit errors in a data word?
- [ ] A. Checksum method
- [ ] B. Simple parity method
- [x] C. Hamming code
- [ ] D. Data compression

<details>
  <summary> <b> Hamming code </b> </summary>

<br/>

Hamming code is an error-correcting code commonly used to detect and correct single-bit errors in transmitted or stored data.

It adds redundant parity bits at specific positions in a data word. <br/>
These parity bits help identify the position of an erroneous bit.

**How Hamming code works?** <br/>
Consider a 7-bit Hamming code (Hamming 7,4):
- 4 bits are data bits.
- 3 bits are parity bits.
- Parity bits occupy positions 1, 2 and 4 (powers of 2).
- Data bits occupy positions 3, 5, 6 and 7.

<img width="1037" height="210" alt="image" src="https://github.com/user-attachments/assets/56809692-b9ae-4063-b826-2194c8885d5e" />

When the receiver checks the parity bits, it generates a syndrome (an error-position indicator).

For a standard Hamming (7,4) code:
- Syndrome 000 -> No error detected.
- A non-zero syndrome -> Identifies the position of a single-bit error.
The receiver can then flip that bit to correct the error.
 
</details>
<!------------------------------>

> - Standard Hamming code corrects single-bit errors.
> - Extended Hamming code can provide SECDED: Single Error Correction, Double Error Detection.

---

Q 35. In a standard Hamming code, parity bits are placed at positions whose indices are:
- [x] A. power of 2
- [ ] B. prime numbers
- [ ] C. odd numbers
- [ ] D. multiple of 3

<details>
  <summary> <b> Hamming code : power of 2 </b> </summary>

<br/>

In standard Hamming code, parity bits are placed at positions whose indices are powers of 2.

These positions are: `1, 2, 4, 8, 16, 32,...`

For example, in Hamming (7,4):

<img width="1065" height="182" alt="image" src="https://github.com/user-attachments/assets/37ee0804-92b3-4e27-bea4-9258009ced6d" />

**Why are parity bits placed at powers of 2?** <br/>
Each parity bit checks selected bit positions based on the binary representation of their position numbers.

For example:
- P1 checks positions whose binary representation has the least significant bit set.
- P2 checks positions whose second bit is set.
- P4 checks positions whose third bit is set.
This arrangement allows the receiver to calculate a syndrome and identify a single erroneous bit.
  
</details>
<!------------------------------>

> - Hamming parity positions = 2⁰, 2¹, 2², 2³...
> - 1, 2, 4, 8, 16, 32.
---

Q 36. Which characteristics is associated with a hardwired control unit?
- [ ] A. Control signals are generated by micro-instructions
- [x] B. Control signals are generated by fixed logic circuits
- [ ] C. Control operations require program interpretation
- [ ] D. Control sequence are stored in control memomry

<details>
  <summary> <b> Hardwired control unit </b> </summary>

<br/>

A hardwired control unit generates CPU control signals using fixed hardware logic circuits, such as:
- Logic gates
- Decoders
- Flip-flops
- Counters
- Control logic circuits
The control signals coordinate CPU operations such as fetching, decoding and executing instructions.

<img width="675" height="382" alt="image" src="https://github.com/user-attachments/assets/b91effec-fb05-4366-84ea-ef9b97bb872e" />

<img width="762" height="367" alt="image" src="https://github.com/user-attachments/assets/c79cdf39-3e21-4a12-806d-f50cbf368a5b" />


|      Hardwired	                    |   Micro-programmed  |
|-------------------------------------|---------------------|
| Fixed logic circuits	              | Micro-instructions  |
| Generally faster	                  | Generally slower    |
| Difficult to modify	                | Easier to modify    |
| No control memory for microprograms | Uses control memory |

Which type of control unit stores its control instructions in control memory?
- [ ] A. Hardwired control unit
- [x] B. Micro-programmed control unit
- [ ] C. Arithmetic control unit
- [ ] D. Register-based control unit

A micro-programmed control unit stores its micro-instructions in control memory (control store). These instructions generate the control signals required to execute CPU operations.
  
</details>
<!------------------------------>

> - Hardwired = Hardware logic; Fixed logic circuits.
> - Micro-programmed = Micro-instructions; Control memory containing micro-instructions.

---

Q 37. Which logic fate is equivalent to an OR gate followed by an inverter?
- [ ] A. NAND Gate
- [ ] B. XOR Gate
- [ ] C. AND Gate
- [x] D. NOR Gate

<details>
  <summary> <b> NOR Gate </b> </summary>

<br/>

A NOR gate is equivalent to an OR gate followed by an inverter (NOT gate).
- First, the OR gate produces an output. 
- Then the NOT gate reverses that output.

| A	| B	| OR (A+B) | NOR Output|
|---|---|----------|----|
| 0	| 0	| 0	       | 1  |
| 0	| 1	| 1	       | 0  |
| 1	| 0	| 1	       | 0  |
| 1 | 1	| 1	       | 0  |

<img width="1050" height="165" alt="image" src="https://github.com/user-attachments/assets/a456b556-8b5e-4684-b920-e3cd517fb2aa" />

  
</details>
<!------------------------------>

> - NAND = NOT + AND
> - NOR = NOT + OR

---

Q 38. Which addressing mode uses the operand value directky in the instruction?
- [x] A. Immediate addressing
- [ ] B. Direct Addressing
- [ ] C. Indirect Addressing
- [ ] D. Register Addressing

<details>
  <summary> <b> Immediate addressing </b> </summary>

<br/>

> **Immediate addressing means the operand value is immediately available within the instruction.**

- Immediate: Actual value is included in the instruction.
- Direct: Memory address is specified in the instruction.
- Indirect: A pointer or register provides the effective address.
- Register: Operand is stored in a CPU register.
  
</details>
<!------------------------------>

> - Immediate: Actual value is included in the instruction.
> - Direct: Memory address is specified in the instruction.
> - Indirect: A pointer or register provides the effective address.
> - Register: Operand is stored in a CPU register.

---

Q 39. In direct mapping, the cache line for a memory block is determined by:
- [x] A. The block number modulo cache line
- [ ] B. The current CPU instruction
- [ ] C. The size of the main memory
- [ ] D. The cache replacement policy

<details>
  <summary> <b> The block number modulo cache line </b> </summary>

<br/>

**Cache Line = Memory Block Number mod Number of Cache Lines**

Direct mapping assigns each memory block to exactly one specific cache line.

```
Suppose:
- Main memory block number = 150
- Number of cache lines = 64

Calculation:

Cache line = 150 mod 64 = 22

```

Remember the three cache mapping techniques:
- **Direct mapping**: One block -> One fixed line.
- **Associative mapping**: One block -> Any cache line.
- **Set-associative mapping**: One block -> Any line within its assigned set.
  
</details>
<!------------------------------>

---

Q 40. In programmed I/O, the CPU typically checks the status of an I/O device repeatedly. This technique is known as:
- [ ] A. Interrupt masking
- [ ] B. Memory mapping
- [x] C. Polling
- [ ] D. Cycle Stealing

<details>
  <summary> <b> Polling </b> </summary>

<br/>

### 1. What is Polling?

Polling is a technique in which the CPU repeatedly checks the status of an I/O device to determine whether it is ready for data transfer.

It is commonly associated with **Programmed I/O**.

**Example** <br/>
Imagine the CPU is waiting for keyboard input:
1. CPU checks whether a key has been pressed.
2. If no key is pressed, it checks again.
3. If a key is pressed, the CPU reads the input.
This repeated checking is called polling.

### 2. Difference between I/O techniques

| Technique	                    | How it works                             |
|-------------------------------|------------------------------------------|
| **Programmed I/O (Polling)**	| CPU repeatedly checks device status.     |
| **Interrupt-driven I/O**	    | Device sends an interrupt to notify CPU. |
| **DMA**	                      | Data transfers directly between device and memory with minimal CPU involvement. |


- A. Interrupt masking: Disables or prevents selected interrupts.
- B. Memory mapping: Assigns memory addresses to hardware or I/O registers.
- C. Polling: Correct; repeatedly checks device status.
- D. Cycle stealing: DMA technique in which a DMA controller temporarily takes control of the system bus.

Which technique allows an I/O device to notify the CPU when it requires attention?
- [ ] A. Polling
- [x] B. Interrupt-driven I/O
- [ ] C. Cycle stealing
- [ ] D. Programmed I/O

- Polling: The CPU repeatedly checks the device's status.
- Interrupt-driven I/O: The device sends an interrupt signal to notify the CPU when it needs attention.
- Cycle stealing: A DMA controller temporarily takes control of the system bus.
- Programmed I/O: The CPU directly manages the I/O operation.
  
</details>
<!------------------------------>

> Remember:
- Polling - CPU checks repeatedly.
- Interrupt - Device alerts CPU.
- DMA - Direct memory transfer.
- Cycle stealing - DMA temporarily uses bus cycles.

> - Polling = CPU asks;
> - Interrupt = device alerts.

---

Q 41. Which I/O techniques area allows a device to notify the CPU when it requires attention?
- [x] A. Programmed I/O
- [ ] B. Memory polling
- [ ] C. Bus waiting
- [ ] D. Interrupt-driven I/O

<details>
  <summary> <b> Interrupt-driven I/O </b> </summary>

<br/>

In interrupt-driven I/O, the device sends an interrupt signal to the CPU when it requires attention. <br/>
The CPU can perform other tasks instead of continuously checking the device.

| Technique	               | How it works                               |
|--------------------------|--------------------------------------------|
| **Programmed I/O**	     | CPU directly manages the I/O operation.    |
| **Memory polling**	     | CPU repeatedly checks device status.       |
| Bus waiting	             | Not a standard I/O notification technique. |
| **Interrupt-driven I/O** | Device notifies CPU through an interrupt.  |


Which I/O technique transfers data between memory and a device with minimal CPU involvement?
- [ ] A. Polling
- [ ] B. Interrupt-driven I/O
- [x] C. DMA
- [ ] D. Programmed I/O

**DMA (Direct Memory Access)** <br/>
DMA allows data to transfer directly between an I/O device and main memory without requiring the CPU to manage every byte or word.

The CPU typically initiates the transfer, and the DMA controller manages it.
  
</details>
<!------------------------------>

- Polling -> CPU repeatedly checks.
- Interrupt-driven I/O -> Device alerts CPU.
- DMA(Direct Memory Access) -> Direct transfer between device and memory.

---

Q 42. What is the **primary function of DMA(Direct Memory Access)**?
- [ ] A. Execute arithmetic and logical operations
- [ ] B. Schedule processes for CPU execution
- [ ] C. Translate logical addresses into physical addresses
- [x] D. Transfer data between I/O devices and memory

<details>
  <summary> <b> DMA (Direct Memory Access) </b> </summary>

<br/>

### 1. Direct Memory Access (DMA)

DMA allows an I/O device to transfer data directly to or from main memory without requiring the CPU to handle every individual data transfer.

**How it works**:
1. CPU configures the DMA controller with the source, destination and transfer size.
2. DMA controller manages the data transfer.
3. After the transfer is complete, the DMA controller can notify the CPU through an interrupt.

| Functions	and Component                             |
|-----------------------------------------------------|
| **Arithmetic and logical operations - ALU**         |
| **Process scheduling - Operating System scheduler** |
| **Logical-to-physical address translation - MMU**   |
| **Data transfer between I/O and memory	- DMA**     |

Which component is responsible for translating logical addresses into physical addresses?
- [ ] A. ALU
- [ ] B. DMA Controller
- [x] C. MMU
- [ ] D. Control Unit

**MMU (Memory Management Unit)** translates logical or virtual addresses into physical memory addresses.
  
</details>
<!------------------------------>

> - Control Unit -> Coordinates CPU operations
> - ALU -> Arithmetic and logic Calculations
> - Scheduler -> Process scheduling
> - MMU -> Address translation
> - DMA -> Data transfer

---

Q 43. Which DMA transfer mode allows the DMA controller to use the system bus by taking individual bus cycles from CPU?
- [ ] A. Burst mode
- [ ] B. Transparent mode
- [x] C. Cycle Stealing
- [ ] D. Interrupt mode

<details>
  <summary> <b> Cycle stealing: A DMA controller temporarily takes control of the system bus.  </b> </summary>

<br/>

### Cycle Stealing Mode

In Cycle Stealing, the DMA controller takes control of the system bus for one or a few individual bus cycles at a time to transfer data.

During those cycles, the CPU temporarily pauses its bus access. The CPU can resume once the DMA controller releases the bus.


| DMA Mode	           | How it works                                                                 |
|----------------------|------------------------------------------------------------------------------|
| **Burst mode**	     | DMA transfers a block of data continuously, holding the bus for the transfer.| 
| **Transparent mode** | DMA transfers data when the CPU is not using the system bus.                 |
| **Cycle stealing**	 | DMA takes individual bus cycles from the CPU.                                |

Which DMA mode transfers an entire block of data continuously by taking control of the system bus?
- [ ] A. Cycle stealing
- [x] B. Burst mode
- [ ] C. Transparent mode
- [ ] D. Interrupt mode

**Burst mode** allows the DMA controller to take control of the system bus and transfer an entire block of data continuously before releasing the bus.
  
</details>
<!------------------------------>

> DMA 3 modes:
- 1. Burst Mode - Entire block at once, Continuous block transfer..
- 2. Cycle stealing - Individual bus cycles.
- 3. Transparent - Uses bus when CPU is idle, basically transfers when the CPU is not using the bus.

---

Q 44. Which addressing mode is commonly used to access array elements using a base address and an index?
- [ ] A. Immediate addressing
- [ ] B. Implied addressing
- [ ] C. Register addressing
- [x] D. Indexed addressing

<details>
  <summary> <b> Indexed Addressing Mode </b> </summary>

<br/>

### 1. Indexed Addressing Mode

Indexed addressing is commonly used to access array elements.

The effective address is calculated using a base address and an index (often scaled by the element size).

Example:
```
Suppose:
- Base address = 1000
- Index = 3
- Each array element occupies 4 bytes

Then Effective Address(EA) = 1000 + (3x4) = 1012
So, the fourth array element is accessed at address 1012 (assuming zero-based indexing).
```
**EA = Base add + (Index * size of elememt)**

Options and	Meaning
- A. Immediate,	Operand value is included in the instruction.
- B. Implied,	Operand is understood from the instruction itself.
- C. Register,	Operand is stored in a CPU register.
- D. Indexed,	Uses an index with a base address to calculate the effective address.

Which addressing mode uses the operand value directly within the instruction?
- [ ] A. Direct addressing
- [ ] B. Immediate addressing
- [ ] C. Indexed addressing
- [ ] D. Indirect addressing

**In immediate addressing, the actual operand value is included directly in the instruction.**
 
</details>
<!------------------------------>

> - Array + Base address + Index = Indexed addressing.

> - Immediate: Value is given directly.
> - Direct:  Memory address is given.
> - Indirect: Address is obtained through a pointer.
> - Indexed: Base address + index.

---

Q 45. Compared with a micro-programmed control unit, a hardwired control unit generally offers:
- [x] A. Higher Operating speed
- [ ] B. Easier modification of control logic
- [ ] C. Greater dependence on control memory
- [ ] D. Simpler changes to instruction sequence

<details>
  <summary> <b> Control Unit - Hardwired vs Micro-programmed Control Unit </b> </summary>


### Control Unit(CU)

A Control Unit (CU) coordinates and controls the operations of the CPU.

There are two common ways to implement it:

1. **Hardwired Control Unit**
- Uses fixed logic circuits, gates, flip-flops and decoders.
- Generates control signals directly through hardware.
- Generally faster.
- Difficult to modify because its logic is physically implemented.

2. **Micro-programmed Control Unit**
- Uses microinstructions stored in control memory.
- Generates control signals by executing microinstructions.
- Generally slower than hardwired control.
- Easier to modify by changing microcode.

|           Hardwired CU	                  | Micro-programmed CU        |
|-------------------------------------------|----------------------------|
| Faster	                                  | Generally slower           |
| Fixed logic	                              | Microinstructions          |
| Difficult to modify	                      | Easier to modify           |
| No control memory required for microcode	| Requires control memory    |

Which control unit stores microinstructions in a special memory called control memory?
- [ ] A. Hardwired control unit
- [x] B. Micro-programmed control unit
- [ ] C. Arithmetic Logic Unit
- [ ] D. Register Unit
  
</details>
<!------------------------------>

> Hardwired CU = Speed, Fixed logic circuits;
> Micro-programmed CU = Flexibility, Microinstructions stored in control memory.

---

Q 46. A cache has a hit ratio of 90%. If 1000 memory accesses occurs how many caches misses are expected?
- [ ] A. 10
- [ ] B. 50
- [ ] C. 900
- [x] D. 100

<details>
  <summary> <b> Hit Ratio and Miss Ratio </b> </summary>


### Cache Hit Ratio and Miss Ratio

- **Hit ratio**: Percentage of memory accesses where the required data is found in cache.

- **Miss ratio**: Percentage of memory accesses where the required data is not found in cache.

**Miss ration = 100% - Hit ratio**

Example:
```
Given:
- Total memory accesses = 1000
- Cache hit ratio = 90%
Miss ratio: 100% - 90% = 10%

cache misses = 10% of 1000 = 100
```

A cache has a hit ratio of 80%. If there are 500 memory accesses, how many cache hits are expected?
- [ ] A. 100
- [ ] B. 200
- [x] C. 400
- [ ] D. 450

```
Given:
- Total memory accesses = 1000
- Cache hit ratio = 80%
Miss ratio: 100% - 80% = 20%

cache misses = 20% of 500 = 100
cache hits   = 80% of 500 = 400
```
  
</details>
<!------------------------------>

> - **Hit ratio**: Percentage of memory accesses where the required data is found in cache.
> - **Miss ratio**: Percentage of memory accesses where the required data is not found in cache.
> - **Miss ration = 100% - Hit ratio**

---

Q 47. In register indirect addressing, the specified register contains:
- [ ] A. The operand value of the instruction
- [ ] B. The instruction code
- [x] C. The memory address of the operand
- [ ] D. The next instruction

<details>
  <summary> <b> Register Indirect Addressing </b> </summary>

<br/>

In register indirect addressing, the specified CPU register contains the memory address where the actual operand is stored.

Example

Suppose:
- Register `BX` contains `2000H`.
- Memory location `2000H` contains the value `50`.
The CPU uses `BX` to find the operand in memory. The operand is `50`, not `2000H`.


In **register addressing**, where is the actual operand stored?
- [ ] A. Main memory
- [x] B. CPU register
- [ ] C. Program Counter
- [ ] D. Instruction Register

In **register addressing**, the actual operand is stored directly in a CPU register.

Example: `MOV AX, BX` - the value in register `BX` is used as the operand.
  
</details>
<!------------------------------>

> Addressing
- Register addressing -> **Register contains the operand(value)**.
- Register indirect -> Register contains the **operand's memory address**.
- Immediate addressing -> Instruction contains the operand **value**.
- Direct addressing -> Instruction contains the **memory address**.

---

Q 48. Which type of memory is generally used to store frequently accessed instructions and data for faster CPU access?
- [x] A. Cache memory
- [ ] B. Optical memory
- [ ] C. Magnetic memory
- [ ] D. Virtual memory

<details>
  <summary> <b> Cache memory </b> </summary>

<br/>

**Cache memory** is a small, high-speed memory located inside or close to the CPU.

It stores frequently accessed instructions and data so that the CPU can retrieve them faster than accessing main memory (RAM).

Example: If the CPU repeatedly needs the same instruction or data, cache can provide it without fetching it from RAM every time.

**Cache memory is commonly organized into three levels:**
| Cache	 | Speed	        | Size            |
|--------|----------------|-----------------|
| **L1** | Fastest	      | Smallest        |
| **L2** | Slower than L1	| Larger          |
| **L3** | Slower than L2	| Usually largest |

- **L1 Cache**: Closest to the CPU core; generally the smallest and fastest.
- **L2 Cache**: Larger but slower than L1.
- **L3 Cache**: Usually larger and often shared among CPU cores.

**options and explaination**
- A. Cache memory,	Correct! Stores frequently accessed data and instructions.
- B. Optical memory,	Uses laser technology, e.g. CDs and DVDs.
- C. Magnetic memory,	Uses magnetic storage, e.g. hard disks and tapes.
- D. Virtual memory,	Uses secondary storage to extend the available memory space.

Which cache level is generally the smallest and fastest?
- [x] A. L1 Cache
- [ ] B. L2 Cache
- [ ] C. L3 Cache
- [ ] D. Main Memory
  
</details>
<!------------------------------>

> Cache = Speed | RAM = Working memory | Virtual memory = Memory extension | Optical = Laser storage

---

Q 49. Which mapping technique divides the cache into sets, with each set containing multiple lines?
- [ ] A. Direct mapping
- [ ] B. Associate mapping
- [x] C. Set-associate mapping
- [ ] D. Sequential mapping

<details>
  <summary> <b> Set-Associative Mapping </b> </summary>

<br/>

**Set-associative mapping** is a cache mapping technique that combines features of direct mapping and fully associative mapping.
- Cache is divided into multiple sets.
- Each set contains multiple cache lines (ways).
- A memory block maps to one specific set.
- Within that set, the block can be placed in any available line.

Example:

Suppose a cache has 8 lines and uses 2-way set-associative mapping.
- Number of sets = 8 ÷ 2 = 4
- Each set contains 2 cache lines.
- A memory block maps to one of the 4 sets and can occupy either line within that set.

<img width="442" height="312" alt="image" src="https://github.com/user-attachments/assets/ac9adf63-9524-47c7-9d23-a24882bc9fa2" />


### 2. Comparison of mapping techniques

| Technique	                    | Mapping rule                                                            |
|-------------------------------|-------------------------------------------------------------------------|
| **Direct mapping**	          | Each memory block maps to exactly one cache line.                       |
| **Fully associative mapping**	| A memory block can go into any cache line.                              |
| **Set-associative mapping**	  | A memory block maps to one set but can occupy any line within that set. |

A cache has 16 lines and uses 4-way set-associative mapping. How many sets does it contain?
- [ ] A. 2
- [x] B. 4
- [ ] C. 8
- [ ] D. 16

```
Given:
- Total cache lines = 16
- Associativity = 4-way
Number of sets = 16 / 4 = 4
So, Each set contains 4 cache lines.
```

> **Number of sets = (Total cache line)/ways per set**
  
</details>
<!------------------------------>

> Set-associative = One set, multiple possible lines.
> - **Number of sets = (Total cache line)/ways per set**

---

Q 50. Which write policy **updates both cache and main memory simultaneously**?
- [ ] A. Write-back
- [x] B. Write-through
- [ ] C. Write-allocate
- [ ] D. No-write-allocate

<details>
  <summary> <b> Cache Write Policies </b> </summary>

### Cache Write Policies

A cache write policy determines how data is updated in cache and main memory when the CPU performs a write operation.

**Write-through**
- Updates the cache and main memory both simultaneously.
- Keeps cache and main memory consistent.
- Generally causes more memory traffic.

**Write-back**
- Updates only the cache initially.
- Marks the cache block as dirty.
- Updates main memory when that block is replaced.

Options and	Function
- A. **Write-back**,	Updates cache first; main memory later.
- B. **Write-through**,	Updates both cache and main memory immediately.
- C. **Write-allocate**,	Loads a block into cache on a write miss.
- D. **No-write-allocate,	Does not load the block into cache on a write miss.

In which write policy is main memory updated only when a modified cache block is replaced?
- [ ] A. Write-through
- [ ] B. Write-back
- [ ] C. Write-allocate
- [ ] D. No-write-allocate
  
</details>
<!------------------------------>

> - Write-through: Write to both cache and main memory immediately.
> - Write-back: Write to cache now, memory later.

---
