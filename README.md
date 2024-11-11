# UT25 Mechanical Braking System Development

## Introduction
This project focuses on the development of the UTFR Mechanical Braking System, ensuring precision and strict adherence to engineering standards and Formula Student Competition rules. The work involved managing design reviews and setting key milestones for DFA, DFC, and DFM on various components. The project aimed to uphold mechanical fundamentals and efficient practices in braking system design.

1.0 Mechanical Department Goals

![image](https://github.com/user-attachments/assets/bd6502bd-729a-4e5f-834d-59d3b41daa7e)

2.0 Brakes Section Goals

![Screenshot 2024-10-03 170544](https://github.com/user-attachments/assets/37cf747d-cc7c-4e1c-bb48-25c7054ad11f)
![Screenshot 2024-10-03 170601](https://github.com/user-attachments/assets/e50061ab-4456-4657-b88a-8043dfd93e69)
![Screenshot 2024-10-03 170626](https://github.com/user-attachments/assets/7f5e29cf-b62a-4df3-909b-45d282ecb651)

3.0 Mechanical Brakes Section Design

3.0.1 Design Rules: (https://www.fsaeonline.com/cdsweb/gen/DownloadDocument.aspx?DocumentID=4bafd174-62da-48b6-b016-589385ca5ae6)
### T.3 Brake System
- **T.3.1.1 - T.3.1.2**: The brake system must act on all four wheels, be operated by a single control, and must be able to lock all wheels.
- **T.3.1.3**: The brake system requires two independent hydraulic circuits to ensure braking on at least two wheels in case of a leak or failure.
- **T.3.1.4**: Each circuit must have its own fluid reservoir.
- **T.3.1.5 - T.3.1.7**: Brake by wire and unarmored plastic brake lines are prohibited; brakes must be protected from drivetrain failures.
- **T.3.1.8 - T.3.1.10**: The brake system should be shielded and critical fasteners should be used in assembly.

### T.3.2 Brake Pedal, Pedal Box, and Mounting
- **T.3.2.1 - T.3.2.2**: The brake pedal must be made of steel, aluminum, or titanium and withstand a 2000 N force without failure.
- **T.3.2.3**: Failure of non-loadbearing components should not affect brake pedal operation.

### T.3.3 Brake Over Travel Switch (BOTS)
- **T.3.3.1 - T.3.3.5**: A mechanical BOTS is required to open the shutdown circuit if brake travel exceeds the normal range. The driver must not be able to reset it.

### T.3.4 Brake Light
- **T.3.4.1 - T.3.4.4**: A visible red brake light, centrally mounted and meeting specific size and shape requirements, must be included.

### T.4 Electronic Throttle Components (APPS) – Pertinent to Accelerator Pedal
- **T.4.2.1 - T.4.2.12**: The APPS on the accelerator pedal must use dual springs and dual sensors to ensure redundancy, fail-safe mechanisms, and fault detection.

3.1 Full Pedal Tray Assembly
A full pedal tray assembly in our Formula SAE vehicle consists of the brake and throttle pedals, mounted on a lightweight, compact tray designed to fit within the driver’s footwell. Both pedals are carefully designed for ergonomic placement, quick response, and durability, ensuring safety, comfort, and efficient driver input during high-performance racing conditions.

3.1.1 Throttle Pedal
A throttle pedal is linked to the accelerator system through an electronic rotary sensor, allowing smooth and responsive control over the engine's power output.

![Screenshot 2024-11-11 062958](https://github.com/user-attachments/assets/d25d8be6-2bd6-4b7d-93be-c4c6c3a2d721)

3.1.1.1 APPS Rotary Sensor
The APPS (Accelerator Pedal Position Sensor) will be bolted to an extended shoulder on the throttle pedal, as shown in the image below. Since the bolt will be obscured by interference with the throttle shaft, it will be safety-wired for security. The flat surface of the APPS rod will align with the flat surface of the inner bushing, ensuring that when the driver presses the pedal, the throttle shaft and APPS rod rotate in unison. The inner bushing is offset by about 30 degrees from the neutral position. As the pedal is pressed, the rotation triggers the APPS sensor to send an electronic signal. This signal is then calibrated to control wheel speed. Please refer to the data sheet for more details. Additionally, if there’s more accurate information about how the APPS sensor sends electronic signals, please let Bararrey know so it can correctly control the car’s wheel rotation.

![Screenshot 2024-11-11 062735](https://github.com/user-attachments/assets/ae016989-9905-42ce-84c5-63210a8b727f)
![image](https://github.com/user-attachments/assets/9771a71d-fe18-48e7-9242-737c393548a6)
![image](https://github.com/user-attachments/assets/da494809-7a67-40c5-a169-964e38c4a93e)
![image](https://github.com/user-attachments/assets/0e07d790-77f8-4609-9737-4ce74466b8a1)

3.1.1.2 Throttle Spring system 
Our throttle system is equipped with two compression springs. The pedal shaft is designed to accommodate both the mounting of the pedal face and the spring mechanism. This spring system resets the pedal to its original position once the driver lifts their foot, ensuring the throttle returns to the default state. To prevent loosening, the springs are pre-compressed within the spring cap and shaft. This pre-compression is achieved by adjusting a nut at the tail of the shaft, creating an offset that secures the springs. We selected a spring rate of 8 lbs/in, which was tested to provide a comfortable and responsive feel for the driver, aligning with our primary ergonomic goals.

![image](https://github.com/user-attachments/assets/b01bac7f-3dc5-417a-a433-058a07afc746)

3.1.1.3 Throttle Face
The throttle pedal face will be designed with a length that accommodates all our drivers this season. It will also feature a tab at the end to help secure the driver’s foot, providing stability and preventing slippage during operation.

3.1.1.4 Heel Rest
The heel rest serves as ergonomic support for the driver’s heel, enhancing comfort and stability. To ensure durability, the back of the heel rest is reinforced with a base to prevent bending or wear over time.

![Screenshot 2024-11-11 063015](https://github.com/user-attachments/assets/3ac5b2ba-a49b-495e-929b-861a75bdcd90)

3.1.1.5 Metals
We will be using aliminum Al6061 due to the facts:
1. **Lightweight**: Aluminum has a high strength-to-weight ratio, making it ideal for reducing the overall mass of the vehicle, which can enhance performance, fuel efficiency, and handling.
2. **Corrosion Resistance**: Aluminum naturally forms a protective oxide layer that resists corrosion, helping components last longer, especially in environments exposed to moisture or varying temperatures.
3. **Machinability**: Aluminum is easy to machine, allowing for precise fabrication of complex parts, and it’s also weldable and compatible with a range of manufacturing processes.
4. **Strength**: While lighter than steel, certain aluminum alloys are still very strong and can withstand significant stress, making them suitable for high-performance applications.
5. **Heat Conductivity**: Aluminum dissipates heat well, which can be beneficial for components near the engine or brakes, as it helps manage temperatures and prevents overheating. 
6. **Cost-Effectiveness**: Compared to some advanced materials, aluminum is cost-effective and widely available, balancing performance with budget considerations.

3.1.1.6 Drawings with GD&T (Coming Soon)

3.1.1.7 FEA

![image](https://github.com/user-attachments/assets/28c07eed-c146-4d9c-b690-ca3f3513ca05)
![image](https://github.com/user-attachments/assets/0891e3a9-02d1-42d3-8167-9cb24fbb8db8)

3.1.2 Brake Pedal with Regen Actuator Pistons:
The brake pedal includes a dual-master cylinder system to provide precise braking force distribution with integration of a bias bar for front-to-rear braking balance adjustments.

3.1.2.1 Solidworks

![image](https://github.com/user-attachments/assets/9fa4819c-8c14-47ab-91a2-53e5b0270bf9)

3.1.2.2 FEA

![image](https://github.com/user-attachments/assets/42a6e605-d7f0-447f-9a2f-0a1238e77163)

3.1.2.3 Calculations

This multiphysics sheet includes the ongoing development of the UTFR Mechanical Braking System, with a focus on ensuring precision and strict adherence to engineering standards and Formula Student Competition rules. Since the first braking system was implemented on the car, this dedicated calculation sheet has been in created to assess braking performance. As the UT25 Braking System Lead, I am responsible for making adjustments and updating the new design parameters in this sheet to ensure compliance with engineering standards and the physical requirements of the vehicle on track.


<img width="1467" alt="Screenshot 2024-10-24 at 6 19 01 PM" src="https://github.com/user-attachments/assets/dcc0a04b-52dd-4e88-a946-dc136d72a667">

3.2 Floating Rotors:

The rotors were created by the previous Braking System Lead and will continue to be used due to their high thermal efficiency and reliable mechanical design. My responsibility is to ensure that the rotors can be installed with the calipers on the updated suspension system, which includes the upright and hub.

3.2.1 Solidworks

3.2.1.1 Front

![image](https://github.com/user-attachments/assets/c2cf99f3-121a-4357-abca-74880ddc50fe)

3.2.1.2 Rear

![image](https://github.com/user-attachments/assets/7a07f162-cbd2-4297-8296-30f322663c38)

3.2.1.3 Bobbin

![image](https://github.com/user-attachments/assets/c16f87c4-2a1b-4ce5-b93c-89a79a48b377)

3.2.1.3 Rear Caliper

![image](https://github.com/user-attachments/assets/d534f008-6ac7-4138-83f3-3e723b88ba93)

3.2.1.4 Front Caliper

![image](https://github.com/user-attachments/assets/c583817c-7b99-442a-8581-a2be7adf65fa)

3.3 Brake Light

3.3.1 SolidWorks
![image](https://github.com/user-attachments/assets/d7ca2135-3fd1-4461-97ce-72342330d5e8)

