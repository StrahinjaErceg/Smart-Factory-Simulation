PLC Automation Project – Smart Factory Simulation
Feb 2025 - Mar 2025

Video:
https://www.youtube.com/watch?v=f3U1ZGWMOZw

Overview:
This project simulates a smart factory using Siemens S7-1500 PLC (CPU 1518F-4 PN/DP) programmed in TIA Portal V15.1. It controls conveyors, stacker cranes, and 2/3-axis robotic arms in Factory I/O, automating material sorting, processing, assembly, and palletizing.

Components:

* Siemens S7-1500 PLC (CPU 1518F-4 PN/DP)
* Factory I/O simulation software
* TIA Portal V15.1
* PLCSIM Advanced V4.0
* Sensors, conveyors, stacker cranes, robotic arms

Project Flow:

1. Raw material enters the line.
2. Photoelectric sensors detect and sort materials by color.
3. Sorted materials move to processing stations.
4. Each item is processed into two parts.
5. A robotic arm picks and combines the two processed parts.
6. The assembled item is placed onto a pallet.
7. Once four items are on a pallet, the stacker crane stores it.

Setup & Prerequisites:

1. Install Factory I/O (supported version).
2. Install Siemens TIA Portal V15.1.
3. Install PLCSIM Advanced V4.0.
4. Ensure network settings allow PLC and simulation to communicate.

Running the Project:

1. Open TIA Portal V15.1 and load the project file (Factory.ap_15).
2. Open PLCSIM Advanced and launch CPU 1518F-4 PN/DP simulation.
3. In TIA Portal, select 'Online' > 'Compile and Download to device'.
4. Start the PLC in PLCSIM Advanced.
5. Open Factory I/O scene file (Factory.factoryio).
6. Configure the I/O address mapping in Factory I/O to match your PLC tags
  * Use the provided Default tag table.pdf.
8. Press 'Play' in Factory I/O to begin the simulation.

Key PLC Logic Modules:

* `ColorSorter` – reads sensor inputs, writes sorting outputs.
* `Processor` – controls processing stations.
* `Assembler` – sequences robot arm motions to combine parts.
* `Palletizer` – counts items, signals stacker crane when pallet is full.
* `ErrorHandler` – monitors faults and stops conveyors/robots if errors occur.

Tips & Troubleshooting:

* Verify all I/O addresses match between TIA Portal and Factory I/O.
* Use PLCSIM Advanced diagnostics to monitor tag values in real time.
* Pause simulation to adjust conveyor speeds or sensor thresholds.
* Check `SystemLog.txt` for error messages if the line stops unexpectedly.

Project Files:

* `Factory.ap_15` – TIA Portal project archive
* `Factory.factoryio` – Factory I/O scene
* `Default tag table.pdf` – I/O mapping file
* `README.txt` – this file

Contact:
For questions or issues, contact the project author at [erceg@uwindsor.ca].
 
