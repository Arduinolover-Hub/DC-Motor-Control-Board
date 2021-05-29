# DC-Motor-Control-Board
DC Motor Control Board Circuit board to control 2 DC motors, with Arduino Nano y Módulo Bluetooth

# Resume
This printed circuit board can control 2 DC motor, after we assembly, it is ready to use, for example, We can put on out robot car. The main features :

Controled by Arduino Nano
Module Bluetooth HC-05
Ultrasonic sensor HC-SR04
H-Bridge L293D

# Schematic diagram

Now let's take a look of the schematic circuit, in this oportunity We used EasyEDA for the design, it is totally Free and easy to use, provide a good number of components and footprint, very recommended for fast design. You can create an account using the next linl: https://easyeda.com/
We can see now, the controller in case the Arduino Nano, we do not use all the pins, just the necesary. Also We can see the Tags M1/INPUT1, M1/INPUT2 wich means inputs 1 and 2 from Motor 1; and the same in the case of Motor 2 (M2/INPUT1; M2/INPUT2).Then We can see the Tags TRIG and ECHO, these correspond for the Bluetooth HC-05 conexion.

El pin the RX ( UART-RX) has to connected to the TX pin of the Arduino Nano by a voltage divisor, it is important to consider this part, because the Bluetooth module voltage work is 3.3V level.

The next part of our circuit is the important L293D which is a H-Bridge. The L293D is an H-Bridge with two possible outputs. Meaning, you can connect two things to it, and you can control the direction of current flow in both.
The next part of our schematic circuit is the ultrasonic sensor HC-SR04, basically We should respect as in the below imagen. The pin TRIG and ECHO can be any pin from the Arduino Nano, does not need to be PWM or analog input.

# PCB Layout

Before We continue with the PCB layout, it is important to indicate that You can use any software for PCB Desing, believe me there are many options, even if you use the best software it will not mean that you are the best pcb desinger, so in this case We are going to use EasyEda highly recommended if you want to enter in the pcb design world.
So after We finished and check our schematic circuit We need to switch from schematic to PCB layout. We can see the PCB with the Ground Plane, this helps for noise filter on the pcb.

Here after we finish the pcb layout We can get the Gerber files, there are two kind of gerber files we have to pay attention to it, the first GerberX2 and the other Gerber RS274X, most of the manufacturer use the second one Gerber RS274X, in some software we will just GerberX2 and Gerber (In the case of Altium Designer).

You can also download the GerberFiles:https://oshwlab.com/Ardlover

# 3D View

One of the features of EasyEda is the 3D visualization, the 3d visualization is important and it give us the posibility to see and check our PCB and how it would be in real, also it can show us the components distribution and dimensions.

# How to Order on JLCPCB

We are going to order from EasyEDA to JLCPCB, they are co-companies and We just jump from our desing to the orders, lets check it out.

JLCPCB: https://jlcpcb.com/IAT

1.Click on File -> Generate PCB Fabrication

After we select this options We can see a brief resume about our order and we have to continue in JLCPCB

2.Indicate the Features
3.Add your shipping address
4.Make the payment and finish the order
5.Receive your PCB

# Why JCLPCB?

JLCPCB has been at the forefront of the PCB industry. With over 14-year continuous innovation and improvement based on customers' need, we have been growing fast, and becoming a leading global PCB manufacturer, who provides the rapid production of high-reliability and cost-effective PCBs and creates the best customer experience in the industry.

Most Efficient, Economic, Innovative PCB Solutions
Higher Quality
Lower Cost
Faster Delivery

#  Building the PCB

Attached you will find the BOM (bill of materials) needed to build the PCB, as you can see in the list you can the designator that You can check also with the schematic circuit.

#  Thanks
Thank to:

JLCPCB: https://jlcpcb.com/IAT

EasyEDA: https://easyeda.com/
