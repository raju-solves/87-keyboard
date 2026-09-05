# Keyboard Build Journal

## Project Overview

This journal covers the complete process of designing and preparing my custom keyboard project, from the first planning stage to the final BOM, firmware planning, DRC checks, CAD, PCB work, and final submission.

| Stage | Time |
|---|---:|
| Planning and Research | 1 hour |
| Schematic and Matrix Wiring | 3 hours |
| Starting PCB | 3 hours |
| Final PCB and 3D View | 3 hours |
| Basic CAD Work | 3 hours |
| Final CAD and Assembly | 3 hours |
| BOM, Firmware, DRC and Final Submit | 3 hours |
| **Total** | **19 hours** |

---

## 1. Planning and Research ( 1 sep )

**Time spent: 1 hour**  
**Running total: 1 hour**

I started by planning the overall design and figuring out what components I would need for the keyboard.

Even after building a macropad before, I underestimated how complex a full TKL keyboard would be. I worked out the layout with 87 keys, macros, and an encoder, and calculated the matrix and GPIO requirements.

Most of this stage was spent reading documentation and comparing parts, which took a lot longer than expected. I also began sourcing components like switches, diodes, USB-C parts, and the RP2040.

Along the way, I learned more about things like ESD protection, capacitors, and JLCPCB part categories.

This phase was slow, but it was important because it gave me a strong foundation before starting the schematic and PCB.


<img width="220" height="229" alt="1774334749925-idjm1u" src="https://github.com/user-attachments/assets/acea0529-a363-4312-b5d0-1b21a5f48a56" />
<img width="679" height="634" alt="1774334100199-u5o96o" src="https://github.com/user-attachments/assets/dde56d69-6ab7-48d9-9e71-69865a1377f2" />


---

## 2. Schematic and Matrix Wiring ( 1 sep )

**Time spent: 3 hours**  
**Running total: 4 hours**

After finishing the planning and sourcing, I moved on to creating the schematic.

This was where everything started coming together. I connected all the switches using diodes and arranged them into a proper keyboard matrix.

At first, managing all the rows and columns was a bit confusing, so I had to recheck my connections multiple times to avoid mistakes.

I also added the RP2040, USB-C connection, and supporting components such as capacitors and resistors.

The wiring was fairly straightforward because this was the second time I had gone through the RP2040 hardware documentation. The first time was while researching and sourcing parts, so I was already familiar with most of it.


<img width="1138" height="611" alt="1774335068468-b4xk0i" src="https://github.com/user-attachments/assets/c3ad824b-90f8-4f12-9d13-1c4e8ea065c2" />
<img width="1172" height="702" alt="1774335049380-znrj0v" src="https://github.com/user-attachments/assets/9c0bedaa-ebf5-4c51-807d-c577ea0c0776" />


---

## 3. Starting PCB ( 2 sep )

**Time spent: 3 hours**  
**Running total: 7 hours**

After finishing the schematic, I finally moved on to the PCB.

This was honestly much harder than I expected.

Placing all the switches took a while because I had to make sure everything lined up properly with the intended keyboard layout.

Once I started routing, things became even more confusing. There were many connections, and I kept reaching situations where one trace blocked another, so I had to undo parts of the routing and try again.

At one point I thought I had planned the routing properly, but it still did not work out.

After a lot of trial and error, I slowly managed to get most of the traces connected in a cleaner way.

Seeing the PCB finally start to come together after all the routing struggle felt really satisfying.


<img width="1235" height="412" alt="1774339837583-d92abk" src="https://github.com/user-attachments/assets/6d364136-0630-4c16-aef7-d43e5bf502bd" />
<img width="1235" height="412" alt="1774339837583-d92abk" src="https://github.com/user-attachments/assets/91e025e0-8034-4440-b227-3cccf9180e40" />



---

## 4. Final PCB and 3D View ( 3 sep )

**Time spent: 3 hours**  
**Running total: 10 hours**

I continued routing the PCB and connected most of the rows and columns.

I also rearranged the crystal so that I could create a better ground plane around it.

Most of this stage was fairly straightforward, but routing still became difficult in some areas. I had to keep rearranging parts so the traces could fit properly without blocking other connections.

Sometimes I had to stop and think about how to connect two tracks without boxing myself in for the remaining rows and columns.

I also noticed that some power symbols were using `3V3` while others were using `3.3`, which caused the nets to be slightly incorrect. I fixed those inconsistencies and continued wiring the board.

Most of this stage was also spent checking everything again and making sure I had not missed anything obvious.

I cleaned up parts of the PCB as well so the board did not look too chaotic.

Seeing a complete PCB after all the routing work felt really satisfying.


<img width="1335" height="516" alt="1774340357177-igap18" src="https://github.com/user-attachments/assets/50ac4f7d-2b55-4e5e-ba34-0438ece87c02" />
<img width="1427" height="483" alt="1774340367724-7z4org" src="https://github.com/user-attachments/assets/115daaea-54d9-4444-84f3-f6096ea24897" />
<img width="1436" height="703" alt="1774340683749-1g0x80" src="https://github.com/user-attachments/assets/3da0cdbe-38be-489b-8d13-d74b2d2b1795" />


---

## 5. Basic CAD Work ( 3 sep )

**Time spent: 3 hours**  
**Running total: 13 hours**

After finishing the PCB, I started working on the plate and some basic CAD for the keyboard structure.

I am still pretty new to CAD, so making the case took longer than expected.

This part felt very different from the PCB work.

I had to make sure all the switch cutouts lined up correctly with the PCB, which required several adjustments.

I also experimented with how the top and bottom parts of the keyboard would fit together, even though I did not go too deep into making a complete enclosure.

Some measurements did not match at first, so I had to tweak the spacing and alignment.

It was not perfect, but this stage gave me a much better idea of how the keyboard would physically come together.

<img width="608" height="501" alt="1774341623539-49usxy" src="https://github.com/user-attachments/assets/7042acb2-cf5e-4822-b3a8-1be68bc0273e" />
<img width="807" height="408" alt="1774341606377-c016h3" src="https://github.com/user-attachments/assets/c6575c34-2132-46a9-9229-e427b8e3c628" />
<img width="836" height="367" alt="1774341495177-vj7xi5" src="https://github.com/user-attachments/assets/6cce59c1-f5fd-466f-8492-b301543adf4c" />
<img width="976" height="346" alt="1774341467706-7451nc" src="https://github.com/user-attachments/assets/e4084b5f-be18-43c0-84c6-84ab838f85a1" />


---

## 6. Final CAD and Assembly ( 4 sep)

**Time spent: 3 hours**  
**Running total: 16 hours**

After working on the plate and basic CAD, the next step was figuring out how everything would actually come together in the final build.

I started planning the assembly process, including how the switches, plate, PCB, stabilizers, and keycaps would fit together.

At the same time, I also looked into firmware and how the keymap would be implemented.

I added all the keycaps to the model, but this took much longer than it should have because I was initially moving and copying them one by one.

Later, I learned that I could use rectangular patterns, which made the process much faster.

Once the keycaps were finally in place, the whole keyboard started to look like a real finished product.

Seeing how the switches and stabilizers fit together in the model also helped me check for possible mistakes.

One of the next things I needed to verify was that there was enough space between the plate and PCB so nothing would get jammed or bent during assembly.

<img width="484" height="280" alt="1774355283896-w0w1fb" src="https://github.com/user-attachments/assets/4fab7b61-1329-4179-bcc9-5bbcbbb1dd75" />
<img width="872" height="498" alt="1774355250516-618swm" src="https://github.com/user-attachments/assets/9f2f4311-9640-4648-afed-94e9256eb313" />
<img width="976" height="365" alt="1774355236590-174on1" src="https://github.com/user-attachments/assets/c8fdcc47-238f-4b2f-9d8c-e034134169ec" />

---

## 7. BOM, Firmware, DRC and Final Submit ( 5 sep)

**Time spent: 3 hours**  
**Running total: 19 hours**

At this point, I was finally ready to wrap up and submit the project.

I had completed the CAD, assembly planning, PCB routing, and the rest of the main design work.

I reviewed the full project again and focused on making sure everything felt complete.

I finalized the BOM with all the components I had researched, including the RP2040, switches, diodes, stabilizers, and other supporting parts.

I also looked into the firmware side of the keyboard and planned how the keymap would be implemented based on my layout.

Finally, I ran the DRC check on the PCB.

The result showed **0 errors**, which was a great way to finish the design stage.

After all the planning, routing, CAD work, checking, and revisions, the project was finally ready for submission.

<img width="1919" height="868" alt="1774355875989-si8xcu" src="https://github.com/user-attachments/assets/cf79f2e4-817d-4f73-807f-898d4b32c2a3" />
<img width="830" height="592" alt="1774355792093-dncbrq" src="https://github.com/user-attachments/assets/553c262f-f745-444c-a3bf-d781ca6a8528" />


---

# Final Time

**Total project time: 19 hours**
