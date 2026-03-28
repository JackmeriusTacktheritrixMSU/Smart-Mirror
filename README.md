# Smart-Mirror
I wanted to create a smart mirror which blended a distance sensor, webcam, and fully accessible raspberry pi. Its got a nice modern look to it, it can do things like tell you positive affirmations- tell you the time, etc. 
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

Screw these hooks into your wall. Made of 2x2 and 1x2s. Sand the bottom face so the 2x2s are just slightly less than 2x2, maybe something like 2x1.9. Then sand a nice chamfer to guide the mirror in. The mirror has cooresponding receptacles <img width="907" height="567" alt="image" src="https://github.com/user-attachments/assets/4bc64522-e9f3-4408-bd95-27c7e5527eae" />
Which hold the hooks.


*Wood*
In the BOM, Wood is just listed by order so heres the breakdown
You need 2 counts 1/2 inch by 3 inch pieces, 29 inches, 2 of the same size face but 17 inches long
You need 2 counts 1 inch by 3 inch pieces, 29 inches, and 2 of the same size face but 21 inches long, and two more at 4 inches long
Two 1x2s, 27 inches long, two 1x2s each 5 inches long
Two 2x2s, each 10 inches long
*Electronics*
The project uses a Raspberry Pi 5 (Or any number of PI that can run Magic Mirror OS). The PI5 sits on a 3D Printed electronics sled which screws into the frame, along with a DC-DC Converter. The DC-DC Converter is automotive grade with a 5A max. The purpose here is so you can use just one power supply unit, at 12V and no less than 5A, to power the monitor and the Raspberry Pi. The PSU plugs in via Barrel Jack Receptacle. Additionally, you may want some kind of push button switch. Get one with a threaded circular back and just drill a hole for it. For AR capabilities, you need a webcam as well. You can route a hole, and plug it in via usb to the raspberry pi. If you're totally neurotic like me, you'll probably craft a way to send the webcam to a gpio pin just because you don't want to route usb all the way to the other side of the pi because it would look bad
<img width="860" height="615" alt="image" src="https://github.com/user-attachments/assets/8fdbb6a1-4102-4015-ba40-87086d25fd3e" />
<img width="1346" height="848" alt="WiringDiagram" src="https://github.com/user-attachments/assets/9a23f0ae-6b83-45a6-b674-f6a674a32ade" />

*Programming* 
The mirror uses Magic Mirror OS. Full credit goes to Guysoft and their collaborators https://github.com/guysoft/MagicMirrorOS



Inspiration:
Credit for the idea to use pocket screws goes to the youtube channel Wicked Random. 

BOM
## Bill of Materials

| Part | Qty | Price (w/ Tax) | Link | Owned |
|------|-----|---------------|------|-------|
| Two Way Mirror 18x24 | 1 | $131.86 | [View](https://www.amazon.com/SupremeTech-See-Through-Two-Way-Mirror-Tempered/dp/B09SBX9JS2) | ❌ |
| Raspberry Pi 4B | 1 | $56.25 | [View](https://vilros.com/) | ❌ |
| 27" Monitor | 1 | $63.29 | [View](https://www.walmart.com/ip/seort/15706505660) | ❌ |
| 20" of 2x2 Lumber | 1 | $2.97 | [View](https://www.homedepot.com/p/2-in-x-2-in-x-8-ft-Furring-Strip-Board-165360/202076422) | ❌ |
| 64" of 1x2 Lumber | 1 | $1.72 | [View](https://www.homedepot.com/p/1-in-x-2-in-x-8-ft-Furring-Strip-Board-160954/100009348) | ❌ |
| 110" of 1x3 Oak Boards | 10 | $29.80 | [View](https://www.homedepot.com/p/Weaber-1-in-x-3-in-Random-Length-S4S-Oak-Hardwood-Boards-22055/207059034) | ❌ |
| 94" of 0.5x3 Oak Board | 1 | $11.98 | [View](https://www.homedepot.com/p/Weaber-1-2-in-x-3-in-x-4-ft-S4S-Oak-Board-27415/207058977) | ❌ |
| JSN-SR04T Ultrasonic Sensor | — | — | [View](https://www.amazon.com/HiLetgo-Integrated-Ultrasonic-Transducer-Waterproof/dp/B07X5H77T7) | ✅ |
| 16mm Momentary Switch | — | — | [View](https://amazon.com/APIELE-Momentary-Waterproof-Stainless-Terminals/dp/B09SLHQVHL) | ✅ |
| DC-DC Converter | — | — | [View](https://amazon.com/Stabilizer-DROK-Waterproof-Transformer-Television/dp/B081RG8XP5) | ✅ |

---

## 💰 Project Cost Summary

| Category | Cost |
|----------|------|
| Parts to Purchase | **$297.87** |
| Components Already Owned | 3 |
| Estimated Total Project Cost | **$297.87** |

- — = Cost not counted toward build total
