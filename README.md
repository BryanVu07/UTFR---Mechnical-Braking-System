# UT25 Mechanical Braking System Development

## Introduction
This project focuses on the development of the UTFR Mechanical Braking System, ensuring precision and strict adherence to engineering standards and Formula Student Competition rules. The work involved managing design reviews and setting key milestones for DFA, DFC, and DFM on various components. The project aimed to uphold mechanical fundamentals and efficient practices in braking system design.

1.0 Mechanical Department Goals

![image](https://github.com/user-attachments/assets/bd6502bd-729a-4e5f-834d-59d3b41daa7e)

2.0 Brakes Section Goals

![image](https://github.com/user-attachments/assets/f5c83527-676a-4fd1-ae23-345690f29e08)
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

3.0.2 Metals

We will be using aliminum Al6061 due to the facts:
1. **Lightweight**: Aluminum has a high strength-to-weight ratio, making it ideal for reducing the overall mass of the vehicle, which can enhance performance, fuel efficiency, and handling.
2. **Corrosion Resistance**: Aluminum naturally forms a protective oxide layer that resists corrosion, helping components last longer, especially in environments exposed to moisture or varying temperatures.
3. **Machinability**: Aluminum is easy to machine, allowing for precise fabrication of complex parts, and it’s also weldable and compatible with a range of manufacturing processes.
4. **Strength**: While lighter than steel, certain aluminum alloys are still very strong and can withstand significant stress, making them suitable for high-performance applications.
5. **Heat Conductivity**: Aluminum dissipates heat well, which can be beneficial for components near the engine or brakes, as it helps manage temperatures and prevents overheating. 
6. **Cost-Effectiveness**: Compared to some advanced materials, aluminum is cost-effective and widely available, balancing performance with budget considerations.

3.0.3 Brake Fundamentals

![image](https://github.com/user-attachments/assets/70c021f4-2d7a-4aff-ae0a-79c6f559e0ef)
![image](https://github.com/user-attachments/assets/94d8087a-62b0-43ce-8150-84c465d88c5c)
![image](https://github.com/user-attachments/assets/b7649da0-5840-45ef-b2f5-d1473f248037)
![image](https://github.com/user-attachments/assets/da33940f-53c0-4bc0-b650-994a8169b43b)
![image](https://github.com/user-attachments/assets/feb6a38f-5155-43b6-95d5-c2800a312659)
![image](https://github.com/user-attachments/assets/a2e178db-79d0-4364-b070-f02cee4e0dac)
![image](https://github.com/user-attachments/assets/6861fd91-4b01-4cb5-be8a-d917d09c7139)

3.1 Full Pedal Tray Assembly

A full pedal tray assembly in our Formula SAE vehicle consists of the brake and throttle pedals, mounted on a lightweight, compact tray designed to fit within the driver’s footwell. Both pedals are carefully designed for ergonomic placement, quick response, and durability, ensuring safety, comfort, and efficient driver input during high-performance racing conditions. The brake and throttle pedal assembly will be bolted onto a composite floor panel, which will be positioned within the front space of the chassis. This setup ensures a secure and stable mounting for the pedal system while maintaining the vehicle’s lightweight structure.

![Screenshot 2024-11-11 071437](https://github.com/user-attachments/assets/7dcb975a-4643-4e5d-b90f-5e108a272572)
![image](https://github.com/user-attachments/assets/2c2514e6-5be4-4f9a-998f-fab46656fb28)

3.1.1 Throttle Pedal

A throttle pedal is linked to the accelerator system through an electronic rotary sensor, allowing smooth and responsive control over the engine's power output.

![Screenshot 2024-11-11 062958](https://github.com/user-attachments/assets/d25d8be6-2bd6-4b7d-93be-c4c6c3a2d721)

3.1.1.1 APPS Rotary Sensor

The APPS (Accelerator Pedal Position Sensor) will be bolted to an extended shoulder on the throttle pedal, as shown in the image below. Since the bolt will be obscured by interference with the throttle shaft, it will be safety-wired for security. The flat surface of the APPS rod will align with the flat surface of the inner bushing, ensuring that when the driver presses the pedal, the throttle shaft and APPS rod rotate in unison. The inner bushing is offset by about 30 degrees from the neutral position. As the pedal is pressed, the rotation triggers the APPS sensor to send an electronic signal. This signal is then calibrated to control wheel speed. Please refer to the data sheet for more details. 

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

3.1.1.5 Tray and Rail

The entire throttle assembly will be mounted using bolts and nuts onto a pedal tray. This tray is designed to slide along a rail and will be secured with a safety pin. The adjustable tray allows for easy customization to accommodate different driver heights, ensuring optimal ergonomics and comfort.

![Screenshot 2024-11-11 063015](https://github.com/user-attachments/assets/3ac5b2ba-a49b-495e-929b-861a75bdcd90)

3.1.1.6 Drawings with GD&T (Coming Soon -> After Design Freeze on Nov 15th)

3.1.1.7 FEA

![image](https://github.com/user-attachments/assets/28c07eed-c146-4d9c-b690-ca3f3513ca05)
![image](https://github.com/user-attachments/assets/0891e3a9-02d1-42d3-8167-9cb24fbb8db8)

3.1.2 Brake Pedal 

The brake pedal includes a dual-master cylinder system to provide precise braking force distribution with integration of a bias bar for front-to-rear braking balance adjustments.

![Screenshot 2024-11-11 071733](https://github.com/user-attachments/assets/e76f1814-bb47-4deb-9e2f-22ab4c9be998)

3.1.2.1 Brake Overtravel Switch

The brake over-travel switch on an FSAE vehicle is a safety feature that prevents excessive travel of the brake pedal beyond its designed range. It will be used to detect when the brake pedal moves too far, indicating a potential issue such as a brake system malfunction or a loss of pressure. When the switch is triggered, it sends a signal to the vehicle's electronic control system, which can activate a warning or shutdown mechanism to prevent damage or ensure driver safety. This switch plays a crucial role in maintaining reliable brake performance and ensuring the vehicle operates within safe parameters during competition.

![Screenshot 2024-11-11 071825](https://github.com/user-attachments/assets/d53083b5-6185-4f76-99c5-78c890a6cb88)

3.1.2.2 Master Cylinders 

The master cylinders were selected based on the multiphysics sheet below. Due to design changes each year to accommodate new systems, I will adjust the parameters accordingly and determine the optimal master cylinder bore size. This will ensure the best brake feel and the appropriate force required by the driver to achieve maximum braking efficiency without excessive effort. The goal is to achive 1.4G deceleration where our tire can handle.

This multiphysics sheet includes the ongoing development of the UTFR Mechanical Braking System, with a focus on ensuring precision and strict adherence to engineering standards and Formula Student Competition rules. Since the first braking system was implemented on the car, this dedicated calculation sheet has been in created to assess braking performance. As the UT25 Braking System Lead, I am responsible for making adjustments and updating the new design parameters in this sheet to ensure compliance with engineering standards and the physical requirements of the vehicle on track.

![image](https://github.com/user-attachments/assets/a52753d5-c73f-43c2-9289-9da292b5eb1c)
![image](https://github.com/user-attachments/assets/b95456d6-2770-4c2c-bad0-50f75356f7da)

3.1.2.3 Regenerative Braking

Regenerative braking will be implemented this year, incorporating a linear potentiometer mounted to the pedal tray and pedal shaft to measure travel distance. Due to the positioning of the electric motor on the rear wheels, there is an energy disadvantage to regenerative braking, requiring techniques to optimize the intervention of the electric braking system. Specifically, it is crucial to prevent the hydraulic braking from dissipating energy during electric braking. This can be achieved by adjusting the setting cylinders that connect the pistons of the pumping elements to the brake pedal. Since the regenerative braking system is partially integrated into the Autonomous Braking System, further details will be provided in the Autonomous Braking System Design repository.

![Screenshot 2024-11-11 071813](https://github.com/user-attachments/assets/319496ef-66ab-4375-9165-0920fce5472c)
![image](https://github.com/user-attachments/assets/ca28616d-1e6f-42ed-a20c-e6e2350b8cf4)
![image](https://github.com/user-attachments/assets/48e57ace-05ce-4499-a5f2-4a90eb78eca8)

3.1.2.4 Bias Bar

In our FSAE rear-wheel-drive vehicle, the bias bar system is used to adjust the brake balance between the front and rear wheels. The bias bar functions by allowing the driver to modify the brake force distribution between the front and rear axles, which is crucial for maintaining optimal braking performance and vehicle stability. We have 45% front and 55% rear brake bias, the system is designed to apply more braking force to the rear wheels, which is suitable for a rear-wheel-drive vehicle. This distribution helps to prevent the front wheels from locking up too early and provides more stability during braking, especially under heavy braking conditions or on slippery surfaces.

![image](https://github.com/user-attachments/assets/d8450cfb-4422-4f58-88dd-aa49faba9d62)
![image](https://github.com/user-attachments/assets/730efe6c-16d9-47c5-a3b8-27492285afc6)


**Adjustment**: 
A proportioning valve will be used in the braking system to control the amount of braking force applied to the front and rear wheels. It regulates the hydraulic pressure delivered to the rear brakes, limiting it to prevent rear-wheel lockup, which could lead to instability or oversteering. This is especially important in vehicles with a rear-wheel-drive configuration, as the rear wheels are more prone to locking under heavy braking.

![image](https://github.com/user-attachments/assets/2b2ec2d8-6024-4e72-b66e-d89a9e5328f5)
![image](https://github.com/user-attachments/assets/6d20b285-e519-4d05-b7fb-20146653df8c)

3.1.2.5 Pressure sensor

A pressure sensor in the braking system measures hydraulic pressure, converting it into an electrical signal to monitor braking force. This data helps optimize brake performance by ensuring proper brake balance and detecting issues like pressure loss. It provides real-time feedback to adjust the braking system for consistent performance, improving brake feel and safety.

![Screenshot 2024-11-11 075927](https://github.com/user-attachments/assets/cda197b1-43ba-44db-b59a-123e646ea2ba)

3.1.2.6 Drawings with GD&T (Coming Soon -> After Design Freeze on Nov 15th)

3.1.2.7 FEA

![image](https://github.com/user-attachments/assets/42a6e605-d7f0-447f-9a2f-0a1238e77163)
![Screenshot 2024-12-15 114246](https://github.com/user-attachments/assets/2f7e733e-6142-4b68-a61f-a8220234c13d)

3.1.3 Floating Rotors:

The rotors were created by the previous Braking System Lead and will continue to be used due to their high thermal efficiency and reliable mechanical design. My responsibility is to ensure that the rotors can be installed with the calipers on the updated suspension system, which includes the upright and hub.

![image](https://github.com/user-attachments/assets/6efc8723-142c-4912-b6ed-02ab16509e32)
![image](https://github.com/user-attachments/assets/b6d95604-1eca-4d24-a0b1-1af7da0e9dce)

3.1.3.1 Front Rotor

![image](https://github.com/user-attachments/assets/c2cf99f3-121a-4357-abca-74880ddc50fe)

3.1.3.1.1 Metal

We decided to use 1020 steel for the floating rotor due to a combination of performance, cost-effectiveness, and ease of manufacturing. This material provides a good balance of strength and durability, essential for withstanding the high stresses experienced during braking without warping or failing. Additionally, 1020 steel is affordable, which helps keep costs down while still offering the necessary performance for a racing environment.Lastly, its wear resistance ensures that the rotor will maintain performance over time, making it a practical and reliable choice for our needs.

![image](https://github.com/user-attachments/assets/1857c746-c0cc-4ed6-b30e-8c4f0b75a5f2)


3.1.3.2 Rear Rotor

![image](https://github.com/user-attachments/assets/7a07f162-cbd2-4297-8296-30f322663c38)

3.1.3.2.1 Metal 

We chose 1020 steel for the floating rotor because it offers a good balance of strength, durability, and cost-effectiveness. It's easy to machine, allowing precise manufacturing, and provides adequate heat resistance and wear resistance for racing conditions. This makes it a reliable and affordable choice for our braking system.

3.1.3.3 Temperature Sensor

The **temperature sensor** in the braking system is used to monitor the heat generated by the brake components, such as the rotors and calipers, during braking. It provides critical data to prevent overheating, which can lead to brake fade or reduced performance. We will mount the sensor to the upright since it is a central structural component of the suspension that directly supports the wheel and brake system, making it an ideal location for the sensor to get an accurate reading of the brake components' temperature. 

### Functioning of the Temperature Sensor:
1. **Heat Detection**: The temperature sensor detects the temperature of the brake components by measuring the heat generated during braking. It works by sensing the changes in temperature and converting this data into an electrical signal.
2. **Signal Transmission**: The sensor sends the temperature data to the vehicle’s data acquisition system or ECU, which processes the information to monitor the system's performance in real time.
3. **Preventing Overheating**: By continuously monitoring the temperature, the sensor helps ensure that the brake components do not exceed safe temperature limits, which could cause degradation in braking performance (e.g., brake fade).

![Screenshot 2024-11-11 081604](https://github.com/user-attachments/assets/df049b92-0894-42b0-8785-18c68687ae58)

3.1.3.4 Bobbin

![image](https://github.com/user-attachments/assets/c16f87c4-2a1b-4ce5-b93c-89a79a48b377)

3.1.3.4.1 Metal 

We chose 7075 aluminum for the bobbin due to its high strength-to-weight ratio, excellent durability, and resistance to corrosion. This makes it ideal for components that need to handle high loads while keeping weight low, such as in the braking system. 7075 also offers good machinability, allowing precise manufacturing of the bobbin. Its ability to withstand the stresses and harsh conditions of racing, combined with its lightweight properties, makes it the perfect material for optimizing performance without adding unnecessary weight.

3.1.3.5 Calipers

We chose ISR calipers because they are among the lightest available, which is crucial for reducing overall vehicle weight. Additionally, they are widely used by FSAE teams around the world, demonstrating their reliability and proven performance in motorsport applications. This makes them a trusted choice for our braking system.

3.1.3.5.1 Rear Caliper

![image](https://github.com/user-attachments/assets/d534f008-6ac7-4138-83f3-3e723b88ba93)

3.1.3.5.2 Front Caliper

![image](https://github.com/user-attachments/assets/c583817c-7b99-442a-8581-a2be7adf65fa)

3.1.3.6 Brake Pads
![image](https://github.com/user-attachments/assets/56cbd3df-2983-444d-a633-32649cc9a76d)

3.1.4 Brake Light

The brake light will be attached to the rear of the chassis tube and connected to the brake light pressure sensor switch. The brake light pressure sensor switch activates the brake light when hydraulic pressure in the braking system reaches a certain threshold, indicating that the driver is applying the brakes. This ensures the brake light turns on whenever braking occurs, enhancing visibility and safety.

![image](https://github.com/user-attachments/assets/d7ca2135-3fd1-4461-97ce-72342330d5e8)


