<img width="3024" height="4032" alt="IMG_3508" src="https://github.com/user-attachments/assets/650ab2ce-5034-42dc-b2bc-07990930901d" />
# Smart-Mirror
I wanted to create a smart mirror which blended a distance sensor, webcam, and fully accessible mini pc. Its got a nice modern look to it, it can do things like tell you positive affirmations- tell you the time, etc. 
I made it because my current mirror isn't smart, which is boring. It doesn't have any lights or anything. I'm also trying to get into smart home things, mostly because I think it would be awesome. 

*The Design*
<img width="1118" height="807" alt="image" src="https://github.com/user-attachments/assets/80c11572-dfd5-4140-932e-0c95d1803f93" />

The mirror has a really prominent webcam compared to others, if you're not into that you don't have to make a webcam hole at all. 

The wood planks used are in 1 inch increments, so its easy to source. The final product should not be too heavy at all (have not made it yet) so you can probably use softwood, but I like hardwood.

You put the wood planks together with a pocket screw jig, and pocket screws. This can be delicate on 1 inch thick wood, so be careful and don't drill into it too much. Do research before or you'll split the wood. 

Beyond that to make the frame, you really just need a good saw, drill, (even a hacksaw would work) and a router. The router is important here 

On the back the mirror sets into the frame and is held in place by screws <img width="991" height="800" alt="image" src="https://github.com/user-attachments/assets/2c34b221-bd0f-4322-abc8-c5543fa1f9f5" />
Do not screw into the mirror. The screws need only hold the mirror in place lightly. Lay a thick bead of glue around the mirror to hold it in place. This, along with the screws and the 3D Printed part sleds will hold the mirror

*Wall Mounting*

Wall Mounting is handled in two parts so its easily take downable<img width="881" height="471" alt="image" src="https://github.com/user-attachments/assets/d7ebd356-2374-4472-b074-07c7d27eff79" />

Screw these hooks into your wall. Made of 2x2 and 1x2s. Sand the bottom face so the 2x2s are just slightly less than 2x2, maybe something like 2x1.9. Then sand a nice chamfer to guide the mirror in. The mirror has cooresponding receptacles which hold the hooks. <img width="907" height="567" alt="image" src="https://github.com/user-attachments/assets/4bc64522-e9f3-4408-bd95-27c7e5527eae" />



*Wood*

In the BOM, Wood is just listed by order so heres the breakdown
You need 2 counts 1/2 inch by 3 inch pieces, 29 inches, 2 of the same size face but 17 inches long
You need 2 counts 1 inch by 3 inch pieces, 29 inches, and 2 of the same size face but 21 inches long, and two more at 4 inches long
Two 1x2s, 27 inches long, two 1x2s each 5 inches long
Two 2x2s, each 10 inches long

*Electronics*

The project uses an older HP Mini pc, which plugs into a webcam, a monitor, and an esp32 wroom on a 3D Printed sled inside the casing. The esp runs an sht30 sensor for temp and humidity, and a distance sensor for a wakeup feature. Its all powered with an iec inlet which splits off.
<img width="950" height="728" alt="image" src="https://github.com/user-attachments/assets/e93e44f6-7df4-427b-bd7d-53c006d4f5a3" />

<img width="1505" height="932" alt="Wiring Diagram" src="https://github.com/user-attachments/assets/63730795-5202-4149-afad-41afa94aeb05" />



*Programming* 
The programming is mostly a configured version of Magic Mirror (The app version) made to run on the mini pc running ubuntu. Mine just also has modules to allow me to read humidity and temperature in the room and wakeup with the distance sensor. Its a simple install, you can use sudo.



Inspiration:
Credit for the idea to use pocket screws goes to the youtube channel Wicked Random. 

BOM
## Bill of Materials

| Part | Qty | Price (w/ Tax) | Link | Owned |
|------|-----|---------------|------|-------|
| Two Way Mirror 18x24 | 1 | $131.86 | [View](https://www.amazon.com/SupremeTech-See-Through-Two-Way-Mirror-Tempered/dp/B09SBX9JS2) | ❌ |
| HP Mini | 1 | - | [View](**https://www.amazon.com/HP-Prodesk-600-G3-Computer/dp/B07RLW1QB8**) | ✅  |
| 27" Monitor | 1 | $63.29 | [View](https://www.walmart.com/ip/seort/15706505660) | ❌ |
| 20" of 2x2 Lumber | 1 | $2.97 | [View](https://www.homedepot.com/p/2-in-x-2-in-x-8-ft-Furring-Strip-Board-165360/202076422) | ❌ |
| 64" of 1x2 Lumber | 1 | $1.72 | [View](https://www.homedepot.com/p/1-in-x-2-in-x-8-ft-Furring-Strip-Board-160954/100009348) | ❌ |
| 110" of 1x3 Oak Boards | 10 | $29.80 | [View](https://www.homedepot.com/p/Weaber-1-in-x-3-in-Random-Length-S4S-Oak-Hardwood-Boards-22055/207059034) | ❌ |
| 94" of 0.5x3 Oak Board | 1 | $11.98 | [View](https://www.homedepot.com/p/Weaber-1-2-in-x-3-in-x-4-ft-S4S-Oak-Board-27415/207058977) | ❌ |
| JSN-SR04T Ultrasonic Sensor | — | — | [View](https://www.amazon.com/HiLetgo-Integrated-Ultrasonic-Transducer-Waterproof/dp/B07X5H77T7) | ✅ |
| IEC Fuse | 1 | 10 | [View](https://www.amazon.com/FILSHU-Socket-Module-Wiring%EF%BC%8Ciec320-illuminated/dp/B08L2522DF) | ❌ |
| ESP32  | 1 | 18 | [View](https://www.amazon.com/HiLetgo-ESP-WROOM-32-Bluetooth-ESP32-DevKitC-32-Development/dp/B0CNYK7WT2/ref=sr_1_2_sspa?dib=eyJ2IjoiMSJ9.qMJJKscaTbDZH8KOrPXaSvL_Wne5ocv0hstobsx2BPxRZhxswDSoA84sKktYY5K4-POEZYa85W79ljFE73xazud66X76xJ5R_C_mREVpeS8L0eeds9uEiyg1kEH-FY1L1X3qvGT1tS2VXli5lwokEq2Eu7PNj6m2O2XuzCIex1J_wlddmR7v14a8MiZHvyLdvR3wBCael7z1MK9nL8nG6xa7NGz2iMOA0oEVPOui0aU.Bski68cJcIyjGGs4OURX38cbTpBKRHduls_TGJnNMgU&dib_tag=se&keywords=esp32+wroom&qid=1775413867&sr=8-2-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1) | ❌ |
| SHT30 Sensor| — | — | [View](https://www.adafruit.com/product/5064?srsltid=AfmBOorFtoxeVo1_rGB0Ptb9_4VkyDuGQjxKZTMGRHcSOYPGJ1WbQ4jiU8Y) | ✅ |
| Logitech C910| — | — | [View](https://www.ebay.com/itm/227025394101?chn=ps&mkevt=1&mkcid=28&google_free_listing_action=view_item) | ✅ |
| Estimated Total Project Cost | **$$161** |

- — = Cost not counted toward build total
