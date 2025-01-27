# 3D Models and CAD Designs

## Overview
This subrepository contains the STL and STEP files for [the Powder Dispensing and Weighing Module Project Repository](https://github.com/loppe35/PowderDispensing_and_Weighing_Module.git). These files represent the 3D models and detailed CAD designs necessary for manufacturing or prototyping the hardware components of the powder dispenser system.

A render depicting the complete system with explanatory labels:

![Full Render Module](https://github.com/user-attachments/assets/2bc7e276-f9d4-4a36-a284-264e3dfc73b5)

When printed, built and assembled the setup will look as follows:

![Full System w. Dummy](https://github.com/user-attachments/assets/48b6c85f-f5f7-476c-8f0f-9b04f7af06fb)

Here a dummy input system is added for testing.

This repository also includes assembly instructions, renders, and labeled diagrams to help users understand the design and build the system efficiently.

---

## Repository Contents

### **1. 3D Model formats**
- **STL Files**: Ready for 3D printing on standard 3D printers.
- **STEP Files**: Suitable for detailed CAD work or integration into larger designs.

### **2. Detailed Component List**
This section provides the detailed names of STL and STEP files corresponding to each component:

#### **3D Printable parts**
Images and labeled diagrams of the assembled system and individual components are provided for visual reference:
1. **Load Cell Housing**
    ![Load Cell Housing](https://github.com/user-attachments/assets/364b0e8f-3878-472e-9461-1a37518e5141)
   - STL: `load_cell_housing.stl`
   - STEP: `load_cell_housing.step`
   - Function: Houses the load cell for precise measurements and serves as a rail for the dispensing head.

2. **Dispensing Head**
    ![Dispenser Head](https://github.com/user-attachments/assets/5b923712-4587-4be1-ad45-2eb070b85f1e)
   - STL: `dispensing_head.stl`
   - STEP: `dispensing_head.step`
   - Function: Holds the auger mechanism in place and aligns it for accurate dispensing.

3. **Syringe Bracket**
    ![Syringe Bracket](https://github.com/user-attachments/assets/3388dbb5-f76f-4f71-aa81-6bc54f8292c8)
   - STL: `syringe_bracket.stl`
   - STEP: `syringe_bracket.step`
   - Function: Secures syringes and attaches to the load cell unigrippers.

4. **Structural Plates**
   - STL: `base_plate_front.stl`, `base_plate_back.stl`
   - STEP: `base_plate_front.step`, `base_plate_back.step`
   - Function: Provide structural integrity and mounting points for system components.

5. **Magnetic Stirrer Mount**
   - STL: `stirrer_magnet_mount.stl`
   - STEP: `stirrer_magnet_mount.step`
   - Function: Holds magnets for the magnetic stirring mechanism.

6. **Magnetic Stirrer Magnet Mount**
   - STL: `MagFanMount.stl`
   - STEP: `MagFanMount.step`
   - Function: Used with a fan and 2 pieces of ![10mm x 10mm disc magnets](https://www.magnetpartner.com/products/power-magnets-disc-10x10-mm) to create a magnetic stirring setup.

7. **Stepper Motor Coupling Components**
   - STL: `StepperCoupling_In_Mag_5mm.stl`, `StepperCoupling_In_Mag_5mm.stl`
   - STEP: `StepperCoupling_In_Mag_5mm.step`, `StepperCoupling_In_Mag_5mm.step`
   - Function: Optional casing to hold a peristaltic pump and relay for dummy input testing.

8. **Dummy Input Components (Optional)**
    ![Dummy Input](https://github.com/user-attachments/assets/b19e5b40-38dd-4867-83e8-cbbfbe41542d)

   - STL: `dummy_input_casing_front.stl`, `dummy_input_casing_back.stl`
   - STEP: `dummy_input_casing_front.step`, `dummy_input_casing_back.step`
   - Function: Optional casing to hold a peristaltic pump and relay for dummy input testing.

9. **Peristaltic Pump Tube Mod (Optional)**
   - STL: `Pump_Mod.stl`
   - STEP: `Pump_Mod.step`
   - Function: Works as an adapter if one would need a smaller diameter tubing.



Additional renders and detailed images are available in the **Renders** and **Part_Pictures** directories.

#### **Additional Hardware Components**

This system requires additional non-3D-printed parts for full assembly. Below is a brief overview:
- **Microcontroller (e.g., Arduino)**: Executes the firmware for low-level control. The project was developed on a ![Sparkfun RedBoard Plus](https://www.sparkfun.com/sparkfun-redboard-plus.html).
- **Stepper Motor**: Drives the auger mechanism for powder dispensing. Here, a small Nema 17 stepper motor was used, also supplied from ![Sparkfun](https://www.sparkfun.com/stepper-motor-with-cable.html).
- **Stepper Motor Driver**: Controls the stepper motor, with a little help from the microcontroller. A bulky yet convenient ![Sparkfun Prodriver](https://www.sparkfun.com/sparkfun-prodriver-stepper-motor-driver-tc78h670ftg.html) was used.
- **Load Cell**: Measures the weight of dispensed material. For the intial development a ![100g load cell from Sparkfun](https://www.sparkfun.com/mini-load-cell-100g-straight-bar-tal221.html) was used. However, a higher resolution and precision was needed at lower capacities, so a 50g load cell was scraped off a ![high precision jewelry scale](https://www.amazon.de/-/en/Precision-High-Precision-Electronic-Calibration-Laboratory/dp/B09VBY575S/ref=sr_1_31?nsdOptOutParam=true&sr=8-31).
- **ADC or Scale Unit**: Converts the load cell signal for digital processing. ![Sparkfun Qwiic Scale](https://www.sparkfun.com/sparkfun-qwiic-scale-nau7802.html) was used.
- **Drain Pump**: Manages liquid flow during cleaning or operations. A ![low-cost peristaltic pump](https://www.amazon.de/-/en/Corrosion-Resistant-Peristaltic-Accessories-G528/dp/B08CZ3Y448/ref=sr_1_7?nsdOptOutParam=true&sr=8-7) was used
- **Relay**: Controls pumps and other external devices. ![Sparkfun Qwiic Relay](https://www.sparkfun.com/sparkfun-qwiic-single-relay.html)
- **2x Disc Magnets**: Sits in magnetic stirrer magnet mount. The required ![disc magnets](https://www.magnetpartner.com/products/power-magnets-disc-10x10-mm) are 10mm x 10mm.



### **3. Assembly Instructions**
Detailed instructions on assembling the hardware components are included in this repository. These instructions cover:
- **Part Identification**: Matching 3D-printed components with their respective functions.
- **Assembly Steps**: Step-by-step guidance for building the system.
- **Hardware Integration**: Connecting additional components like load cells, stepper motors, and electronics.

---

## Usage

To use the files in this repository:

### **1. 3D Printing**
1. Open the STL files in your preferred 3D printing software.
2. Adjust settings based on your printer’s requirements.
3. Print the parts using compatible materials (e.g., PLA, ABS).

### **2. Printing Settings**
Prints were all carried out on an Ultimaker S3 with standard black PLA filament. The following settings were used:
- **Layer Height**: 0.2 mm – Standard resolution for balanced quality and print time.
- **Infill Density**: 20% – Provides a good balance between strength and material usage.
- **Print Speed**: 50 mm/s – Optimal speed to ensure quality without significantly increasing print time.
- **Print Temperature**: 210°C – Ideal for PLA; temperatures may vary for other materials.
- **Bed Temperature**: 60°C – Recommended for PLA to ensure good bed adhesion.
- **Retraction Distance**: 6.5 mm – Helps reduce stringing between print parts.
- **Retraction Speed**: 25 mm/s – Balances speed and effectiveness of retraction.
- **Cooling Fan Speed**: 100% – Essential for overhangs and fine details.
- **Support Structures**: Everywhere – Used when printing complex models to support overhangs.
- **Build Plate Adhesion Type**: Brim – Helps to prevent warping and ensures the first layers stick well.

Additional notes:
- **Support Variations**: Tree-style support structures were used only for the back part of the base and the dispensing head.
- **Printing Orientation**: All parts, except the dispensing head, must be printed "laying down":
  - Front parts should be laid on their backs.
  - Backplate parts should be laid on their fronts.

### **3. CAD Design**
1. Import STEP files into CAD software (e.g., Fusion 360, SolidWorks).
2. Modify or integrate the designs into larger systems as needed.

### **4. Assembly Guide**

#### **Preparation**
1. Acquire all necessary parts listed above.
2. Print the 3D components using the settings provided in the **Printing Settings** section.
3. Gather tools and equipment as specified in the equipment list.

#### **Step-by-Step Assembly**

1. **Front Plate Assembly**:
   - Attach the 40x40mm fan using 4x M4 hex-socket screws.
   - Attach the peristaltic pump with 2x M3 hex-socket screws. Ensure wires pass through the designated holes.

2. **Backplate and Stepper Motor Preparation**:
   - Attach the stepper motor to the motor mount.
   - Prepare the load cell housing by following.

3. **Motor Shaft Coupling**:
   - Insert 5mm x 2mm magnetic discs into the designated holes. Ensure alternating magnetic polarity.
   - Use tools or glue to secure magnets if necessary.

4. **Structural Assembly**:
   - Secure the front and back plates to the structural build plate.
   - Slide wires through appropriate holes to maintain organization.

5. **Final Components**:
   - Attach additional parts such as the dispensing head and magnet mounts.
   - Fasten the dispensing head rail and motor coupling.

6. **Dispensing Head Assembly**:
   - Insert the tube into the dispensing head cartridge.
   - Drill necessary holes and attach the auger mechanism with bearings and couplings.
   - Ensure smooth rotation and secure the components with glue if needed.

7. **Wiring**:
   - Mount the Arduino board and connect wires as per the circuit diagram.
   - Organize wires to ensure a clean setup.

#### **Verification**
1. Ensure all components are securely fastened.
2. Check wiring for proper connections.
3. Test mechanical movement and rotation before powering the system.

### **Flashing Firmware**
Make sure the installation guide from the `PowderDispenserCPP` directory is succesfully followed. That all the necessary files are cloned from gitHub repository.
1. **Install Dependencies**:
   - Navigate to the directory in the software submodule.
   - Run the following command to install Python dependencies:
     ```bash
     pip install -r requirements.txt
     ```
2. **Compile Firmware**:
   Connect the Arduino Uno board with the computer, and flash it though the chosen IDE(PlatfomIO was used during this project), with the main.cpp file located in the source files of the ![software repository](https://github.com/loppe35/PowderDispenser_FWSW.git).
3. **Configure System**:
   - Edit the `config.json` file to match your specific hardware and operational parameters.
---

## Contributing
If you make any modifications or improvements to the designs, please consider sharing your modified files back with the community. Contributions are encouraged under the CERN OHL-W v2.0 licensing terms to foster collaboration and innovation.

---

## License
The 3D models and CAD designs are released under the CERN Open Hardware License v2.0 (OHL-W). This allows you to use, modify, and distribute the designs under the terms outlined in the license.

Refer to the `LICENSE` file for detailed information.
