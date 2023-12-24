# RHCCV - Color Computer 2 S-Video and Composite Mod with Audio 

The ***RHCCV*** is a video mod for the ***Tandy Radio Shack Color Computer 2***. The modification **replaces** the **original** video **module** (the shiny metal box) of the *CoCo2*. It features a **6-pin** or **4-pin** compatible **Mini DIN** connector with **S-Video**, **Composite Video** and **Audio** outputs.

<img src="RHCCV-PCB.png" alt="MarineGEO circle logo" style="height: 375px; width:300px;"/>

## Assembly and Installation
### 4-pin Mini DIN installed *(S-Video only)*
The **PCB** populated with a **4-pin** Mini DIN connector delivers **S-Video** as the **only** available **output**. The **pinout** is **standard** S-Video, as described [here](https://en.wikipedia.org/wiki/S-Video "S-Video Wikipedia").

### 6-Pin Mini DIN installed *(S-Video, Composite and Audio)*
The **6-pin** connector installed on the **PCB** makes **all** outputs available **simultaneously**. However, this requires a **custom** made **breakout cable** in order to **access** the **signals** individually. A veteran **PS/2** cable can be **modified** but please note that in some cables **not all pins** are **connected**.

The 6-pin Mini DIN connector has the following **pinout**:
* Pin 1: **Audio** out
* Pin 2: **Composite** Video
* Pin 3: **GND**
* Pin 4: **GND**
* Pin 5: **Luma** (Y)
* Pin 6: **Chroma** (C)

The KiCad PCB design uses a custom footprint for *ASSMANN* Mini DIN Connectors:<br>
<https://www.assmann-wsw.com/uploads/datasheets/ASS_1622_CO.pdf>

### Installation
* Desolder the **clamps** of the **metal** box and the **pin headers** of the original video module from the **main board**. (I highly recommend using a **desoldering pump** and **solder wick**.)
* Carefully **desolder** the ***MC1372*** from the PCB of the original video module.
* Make sure that the **pins** of the *MC1372* are **free of solder** and plug it into the **socket** of the RHCCV. Mind the correct **orientation**.

The new PCB uses the **same** pin headers as the **original** module and does not need any additional wires to be pulled.

## The Mod
The **design** was **inspired** by the **efforts** and research of ***[AC's 8-bit Zone](https://youtu.be/tayGsz7Xs3A "ACs 8-bit Zone - YouTube")*** on *YouTube*. The RHCCV mod **combines** his S-Video and Conmposite Video **circuits** and casts them into a **single** board.

Since he didn't design a PCB for them, but instead modified the original hardware, he had to route some loose cables to the outside. In contrast, the use of **Mini DIN** connecors for this mod has some **advantages**:

* The **original** hardware stays **in tact** (desides desoldering the *MC1372*)
* **No loose cables** coming out of the TRS-80 case
* **No case modification** for additional connectors needed




