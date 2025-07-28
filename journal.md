---
title: "CCMini"
author: "bcon"
description: "mini cross gantry cantilevered 3d printer"
created_at: "2025-07-18"
---
Total Time Spent: 32.5 Hours

## **7/18/2025 Log 1: A Fun Start**

I was browsing through youtube when I came upon [this video](https://www.youtube.com/watch?v=bA-R3nCNyYw). This was the second time I had stumbled upon this channel, the first being months ago with their first video on this. I then decided that I wanted to try to make a similar printer in my own style. 

I directly went into the CAD, as this was a system small enough for me to do in one document. 

<img width="765" height="737" alt="image" src="https://github.com/user-attachments/assets/f71a618a-2d31-48b8-a1ed-89e5321e4166" />

After some time, I got this base design. I built the linear rails into the bottom, printed, main housing for better rigidity. 

<img width="846" height="838" alt="image" src="https://github.com/user-attachments/assets/11553dd4-ec68-4276-abb1-d43534f805e7" />

These will house the motors, mainboard, and hopefulyl every oher electronic besides the power supply. 

I then started building out the z axis. I knew I wanted to do belted z for 2 reasons: 1, I have never done belted z before and wanted to try it. 2, it fit better for my design as if I were to do leadscrew, the motors would havbe to be rotated 90 degrees and not package as well. 

<img width="527" height="612" alt="image" src="https://github.com/user-attachments/assets/d8548b24-e347-42e1-b0c6-d6fc4af17e1a" />

From here, I built out the z axis, and ever started to put in the motors for the x and y, along with a base starting block for the x/y motion system. 

<img width="947" height="1157" alt="image" src="https://github.com/user-attachments/assets/efa19b63-7f5c-4348-bf52-b3ec709dfdc1" />

<img width="1265" height="971" alt="image" src="https://github.com/user-attachments/assets/30300381-0d03-4259-adc2-7e7a267ad23f" />

This z axis part actually utilizes a mirrored, yet flipped design in order to have one motor on top and one on bottom so the x/y system works properly. It holds the motors, linear rails, and the carriage for the z system all in one part. 

Finally, I decided on using an older SKR Mini E3 V3 board for my mainboard - it only has 4 stepper drivers, but 5 slots as I will be driving the 2 z motors off of the same driver. I already had this board, and wanted to use it for something, and didn't really want to have to get another board with 5 slots. 

Total Time Spent: 6 Hours

## **7/19/2025 Log 2: X/Y, and a Lot of Struggle

I then went to work on my X/Y motion system. Since it is cross gantry, the belt runs are simpler than that of core xy. However, since I am aiming to make this thing super small (120mmx120mm bed, it is less than 7 inches large in length and width), it becomes a lot harder to integrate everything I want to put here. 

<img width="658" height="700" alt="image" src="https://github.com/user-attachments/assets/de670a5d-3de7-4ecc-a9bb-ec2bb14d6b88" />

I first had to deal with these parts clipping, leading me to have to make over 10 micro adjustments to the part for clearances. 

<img width="856" height="1090" alt="image" src="https://github.com/user-attachments/assets/33c86021-ffa0-47be-866a-bfacb943ca43" />

I then made a simple part to link the 2 linear rails together. This is the basis of my toolhead and will be what holds the entire toolhead together. 

<img width="1517" height="913" alt="image" src="https://github.com/user-attachments/assets/a299589c-5aa3-4986-b346-e404fbad300d" />

<img width="697" height="677" alt="image" src="https://github.com/user-attachments/assets/442c7e26-9b52-4774-8303-d9742168e857" />

I am currently planning for the toolhead to be in this spot here. This gives the most clearance on both sides of the system and gives me the most room to do what I want. Something to think about with the toolhead will be minimizing weight as this is still cantilevered. 

Total Time Spent: 4.5 Hours

## **7/20/2025 Log 3: More Microadjustments, Belt Tensioning, and Onto the Toolhead

I first made this part to mount the x/y linear rails and clamp to the belt, allowing it to be controlled by the motor. 

<img width="592" height="632" alt="image" src="https://github.com/user-attachments/assets/210a02a6-3d4a-43b1-b9cb-14d97abdf23c" />

This part is nowhere near to final, and will be optomized later for printability and strength. 

<img width="910" height="977" alt="image" src="https://github.com/user-attachments/assets/2c7a8c6f-27e9-44f3-b1db-a07c2e37d9d5" />

This was done for both sides, essentially finishing the x/y system. 

I then went to my z axis to do the same. 

<img width="980" height="1135" alt="image" src="https://github.com/user-attachments/assets/6eb4d675-41dd-405b-a825-1aa3680ad7b4" />

The belt run will look like so. 

<img width="1412" height="972" alt="image" src="https://github.com/user-attachments/assets/11a853af-da1b-451d-9770-8a54b88f3d1e" />

After some more work with this, I had a similar belt clamp system for the z axis. 

This brought me to my next problem: Belt tensioning. While I will not be cranking the tension due to none of the motors being in double shear, I still want a way to make adjustments. 

After some thought about it, I settled on moving the motor itself. This keeps everything else relatively simple, as I only need an idler pulley on the other end. I am relatively confident in this, partially because the clamping force of 4 bolts is very strong, but also because I saw Ivan Miranda do this for a cnc once in a video. 

<img width="637" height="678" alt="image" src="https://github.com/user-attachments/assets/67664f9a-7f16-479d-ae77-2be5122b7411" />

i have abouyt 3mm of motion here, along with being able to adjust the belt itself on the clamp. 

Following this logic, I decided to do the same thing for the x/y system. 

<img width="1080" height="1007" alt="image" src="https://github.com/user-attachments/assets/5963232c-58c9-453c-93c7-ef2a5cfd9656" />

With this, I can now tension all of my belts. 

Next, I am going to work on the idlers for my belt runs to complete the motion system. 

<img width="1400" height="788" alt="image" src="https://github.com/user-attachments/assets/5339c066-3873-4ddd-9346-8a5090457ab0" />

I modified the z parts to include the idler built in. These ride on an m5 bolt. 

<img width="1455" height="796" alt="image" src="https://github.com/user-attachments/assets/5ef8fe62-e240-4c26-9653-6eddddfbeab0" />

Finally, I modified the top stiffener part to also include the idler built in. This is all a super compact, super packaged system that I am very proud of.

Total Time Spent: 6 Hours

## **7/27/2025 Log 4: Toolhead**

I have spend the past week working through how exactly I am going to make this toolhead. 

After much work, I decided on bowden drive, a Revo V6 Hotend, a 4010 Fan for part cooling, and a BL Touch. 

<img width="862" height="755" alt="image" src="https://github.com/user-attachments/assets/2b2b3f16-6c71-4213-b6ba-775408c952c4" />

<img width="1347" height="1137" alt="image" src="https://github.com/user-attachments/assets/a324b3ac-a718-4ef1-8ed5-bc2730f08ab5" />

This dark blue part bolts and clamps the hotend down. 

<img width="967" height="876" alt="image" src="https://github.com/user-attachments/assets/c6041247-9f32-4113-a1f1-f606140ec80f" />

The BL touch mounts to both of the parts that hold the Revo V6.

<img width="697" height="736" alt="image" src="https://github.com/user-attachments/assets/4851ecc5-a83c-42fd-9f75-6db6ddc39d54" />

The part cooling took by far the longest to figure out. I went babck and forth through different locations and size of fan, from going around the linear rails to putting them horizontal. I ended up with this, which mounts the part cooling fan to the hotend cooling fan, which given that we have a V6 hotend, should be fine to limit the airflow of the hotend slightly. 

<img width="1232" height="1047" alt="image" src="https://github.com/user-attachments/assets/193a98c5-0540-4707-957a-c7d1ec026a89" />

This duct will cool the part, combined with the fan mount gives one 4010 blower fan for cooling, which isn't optimal but will work to start. I am already looking into a way to get a 5015 blower fan on, but space is limited.

<img width="762" height="752" alt="image" src="https://github.com/user-attachments/assets/c3669826-3b4b-45e9-86d3-0a6f98e8d6f8" />

From there, I mounted the ProtoXTruder V2, acting as a bowden drive, to my top rail support block. This will take the filament in through the bottom and spit it out the top to the hotend. 

Total Time Spent: 10 Hours over Multiple Days

## **7/27/2025 Log 5: Finishing Up**

<img width="912" height="1055" alt="image" src="https://github.com/user-attachments/assets/2cafbec2-b947-49c0-bc4a-c9fa883e1e31" />

I have officially finished this printer! Colors have yet to be decided but I will figure them out before officially submitting. 

In this, I have done all of the electronics and mounted my Z Axis. 

<img width="1270" height="917" alt="image" src="https://github.com/user-attachments/assets/95eceaad-e10a-4a42-a799-39a7a7140854" />

The electronics are all bottom mounted to my frame, including the Pi 0 2 W, SKR Mini E3 V3, and Power Supply.

<img width="1178" height="887" alt="image" src="https://github.com/user-attachments/assets/05a023d9-b36c-4457-9edb-7fdeb2d2502a" />

Then, a bottom part is mounted to close it off, as well as use the stoppers from linear rails as feet. 

<img width="992" height="746" alt="image" src="https://github.com/user-attachments/assets/139200a2-e6b5-4deb-ba64-d05c95a30a4f" />

The bed is mounted with 3 bolts and spacers directly to the frame. 

All in all, this creates an electronics box that holds everything I need for this printer. 

<img width="1278" height="712" alt="image" src="https://github.com/user-attachments/assets/064180d2-89ec-45f7-8255-3bcdb9b24458" />

I also added these 2 3010 fans for electronics cooling that draw air through the system to cool all of the components. Ideally, the power supply doesnt affect the airflow too badly. This was done after realizing that I was sealing all of my electronics into a plastic box, which is never a good idea.
<img width="1343" height="1007" alt="image" src="https://github.com/user-attachments/assets/f218c175-4779-4828-80ca-bdb5fd8df72e" />

This was a lot of fun to design. I hope the different approach to the kinematic system will make for a fun project. 

<img width="807" height="1008" alt="image" src="https://github.com/user-attachments/assets/992e49dd-36d3-4716-a032-a02b23a6508e" />

Total Time Spent: 6 Hours
