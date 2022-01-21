---
layout: post
author: Yohan
title: GPS, What The FAQ?
description: The not complete "how to" about GPS
summary: Your GPS is maybe fake, buy a genuine GPS!
tags: [gps]
date: 2022-01-21 20:40:00 -0800
---
# GPS : THE FAQ

## 1. How can I get my GPS happy even when he’s not?
Three easy solutions to get your GPS happy :
-   Power the GPS standalone before the rest of the stuff and wait for it to get a fix. Disconnect the standalone cable and reconnect the GPS to the rest.
-   Try powering runcams, video transmitters and telemetry radios **ONLY ONCE** GPS fix is acquired.
- If none of above worked, the *"guide of the good engineer 2022 (updated edition)"* recommends  using a hammer as a deterrent tool. GPS will quickly understand who's the boss, and in case he doesn't, he will quickly cease to be a GPS. 

<br>

## 2. Sometimes my GPS is really happy and then a few hours after he’s not, what to do?
-   The integrated battery on your GPS keep the informations needed for a hot start (happy GPS) for about 3 hours, afterwards your GPS will have to wait to be happy on startup again

<br>

## 3. Can my GPS be happy even higher than so called “COCOM” limits?
-   **YES**, your GPS can perfectly be happy up to 50km or even 80km above sea level, you just have to put it in the “airborne <4G mode” if it’s a Ublox GPS. The SAM-M8Q can for example go up to 50km, and the NEO-M9N up to 80km. Oh and by the way *“CoCom ceased to function on March 31, 1994, and the then-current control list of embargoed goods was retained by the member nations until the successor, the [Wassenaar Arrangement](https://en.wikipedia.org/wiki/Wassenaar_Arrangement), was established.”* :)

<br>

## 4. Is it legal to put my GPS into the illegal dangerous bad (gone wrong!!) “airborne <4G mode”
-   NO. N**O** NO**OOOOO**OO**OOOOO**, it’s not illegal to put your GPS into the illegal dangerous bad (gone wrong!!) “airborne <4G mode”. **It’s designed for**. You have to send the right setup command to the GPS via serial. The command is not the same for different GPS models. Try looking for the GPS's datasheet, and then the communication protocol for your specific GPS model. 

<br>

## 5. I want my GPS to only send data when I want, how can I do this?
-   Most GPS sends data at a fixed rate that you can set using the settings. All the libraries proposing so called “polling” functions are just going to freeze your code until the next time the GPS decides to send a message because he’s happy. 

<br>

## 7. Why does the military want to limit my GPS at 4G??!!!
-   They don’t give a shit about your GPS accelerating at more than 4G but physics does. This is not a limitation but a physical limit. After this limit the GPS position precision will drop.

<br>

## 8. I can't get my GPS to speak the same language as my TEVECEEE flight computer, what can I do? 
- Check the baud rate used for the communication between your computer and the GPS (AKA the UART serial port). Use 9600 as a first value. Most GPS use this baud speed as a factory setting. 
- TX and RX are not gay, TX goes with RX and RX goes with TX.

<br>

## 9. I want to change the settings of my GPS how to do? 
- Download and install U-Center if it's a Ublox GPS, otherwise you're pretty much not happy to not say f.. yeah you got it no need to write it. 
- Get yourself a UART to USB converter (search for a FTDI dongle) to connect the GPS to your PC. Alternative solution: butcher an Arduino Nano to use it as and FTDI dongle. 

<br>

## 10. My GPS can connect to U-Center but I can't change the settings 
- Open the serial monitor right when you connect the GPS, and look at the first sentence sent by the GPS. 
- Open google and search for "Fake Ublox GPS, how to recognise them?" and learn why it was a bad idea to buy a GPS on Amazon for 7$ *(you can replace "GPS" by any other hardware you want, it's pretty much the same)*. 

<br>

## 11. Damn.. so my GPS is a fake, what can I do now?
- The SAM-M8Q GPS is a really good, small GPS. You can find a lot of differents breakouts easy to use. I'm sure you know what you have to do. 

<br>  
  
<br>  

<br>  

<br>    
 
<br>  

<br>  

<br>  

did you notice point 6 was missing? 

:) 

