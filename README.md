# Pipelined Processor

This repository contains a Verilog implementation of a **pipelined processor** with **2-stage, 3-stage, and 4-stage pipeline variants**.  
The processor executes instructions in a pipeline, allowing overlapping of different phases of multiple instructions — thereby improving throughput.

---

## 🔹Features

- **2-Stage pipeline:**  
  - **Fetch/Execute**
  
- **3-Stage pipeline:**  
  - **Fetch → Decode → Execute**
  
- **4-Stage pipeline:**  
  - **Fetch → Decode → Execute → Memory**
  
- Support for **hazard handling**, **stall**, and **forwarding** mechanisms.
- Separate modules for **control**, **datapath components**, and **hazard detection**.

---

## 🔹Directory Structure
├── 2 Stage/
│ ├─ ALU.v
│ ├─ ControlUnit.v
│ ├─ ExecuteUnit.v
│ ├─ FetchUnit.v
│ ├─ Hazard.v
│ ├─ InstructionMemory.v
│ ├─ Latch_FetchExecute.v
│ ├─ MemoryUnit.v
│ ├─ OperandFetchUnit.v
│ ├─ processorCore.v
│ ├─ RegisterFile.v
│ └─ out.vvp
├── 3 Stage/
│ ├─ ALU.v
│ ├─ ControlUnit.v
│ ├─ ExecuteUnit.v
│ ├─ FetchUnit.v
│ ├─ Hazard.v
│ ├─ InstructionMemory.v
│ ├─ Latch_FetchDecode.v
│ ├─ Latch_DecodeExecute.v
│ ├─ MemoryUnit.v
│ ├─ OperandFetchUnit.v
│ ├─ processorCore.v
│ ├─ RegisterFile.v
│ └─ out.vvp
├── 4 Stage/
│ ├─ ALU.v
│ ├─ ControlUnit.v
│ ├─ ExecuteUnit.v
│ ├─ FetchUnit.v
│ ├─ Hazard.v
│ ├─ InstructionMemory.v
│ ├─ Latch_FetchDecode.v
│ ├─ Latch_DecodeExecute.v
│ ├─ Latch_ExecuteMemory.v
│ ├─ MemoryUnit.v
│ ├─ OperandFetchUnit.v
│ ├─ processorCore.v
│ ├─ RegisterFile.v
│ └─ out.vvp
└─ README.md