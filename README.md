## Getting started with ESP 8266 001 Wifi Module project 

## Module Details

* [ESP8266 001](https://www.amazon.com/Makerfocus-ESP8266-Wireless-Transceiver-Compatible/dp/B01EA3UJJ4/ref=sr_1_fkmrnull_12_sspa?keywords=esp8266+001&qid=1556673961&s=electronics&sr=1-12-fkmrnull-spons&psc=1) - Buy on Amazon

## Specs 
* Black
* 1 MB memory 
* DC 3.0-3.6V 

## Components Required for this project
1) [Ardunio Uno R3](https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6) - Buy on Amazon
2) [Jumper wires](https://www.amazon.com/Elegoo-EL-CP-004-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=sr_1_2?keywords=wires+for+arduino&qid=1559065046&s=electronics&sr=1-2-spell) - Buy on Amazon
3) Serial cable
4) [Bread board](https://www.amazon.com/EL-CP-003-Breadboard-Solderless-Distribution-Connecting/dp/B01EV6LJ7G/ref=sr_1_1_sspa?keywords=Bread+board%5D&qid=1559065145&s=electronics&sr=1-1-spons&psc=1) - Buy on Amazon
5) [Download and install Ardunio IDE on to your computer] (https://www.arduino.cc/en/Main/Software) - offical website


## Defination

Baud rate: It is the rate at which wifi module (ESP8266 001) communicates with the computer via Wireless acess point 

Note: Change baud rate if necessary: AT+CIOBAUD=9600 (or) AT+CIOBAUD=11200 ( 9600 baud rate best worked for me) 

## Procedure -1 is to configure wifi module (i.e change the baud rate)

1) Make the circuit connections as stated in circuit diagram below 
   ![Capture](https://user-images.githubusercontent.com/48098768/58503676-b6740600-814e-11e9-8d91-683b3530c7e0.JPG)



2) Connect the serial cable to USB of your computer
3) Open Arduino IDE, click "file" ( top left corner, on the bar ), click "new" to upload the below code

                     void setup() {
                       // put your setup code here, to run once:

                     }

                     void loop() {
                   // put your main code here, to run repeatedly:

                     }

4) Clieck on "tools" and ensure Ardunio/Genuino Uno borad is selected and Apporiate port number is selected 
5) Now verify and upload the code 
   Note: This code is a void code used in order to use transmission and receiver pin on Ardunio to communicate with the ESP8266 001
6) Now Arunio IDE will state that the code has finished uploading also Ardunio and ESP 8266 001 inbuild LED will flash a couple of  
   times.
7) Now open the serial monitor on the Ardunio IDE and send AT commands
8) Send "AT" and recieve acknowledgment
9) Send "AT+ CIOBAUD=9600" and recieve acknowledgment
   Note: dont copy paste but type the code, follow image below for other scrolldown options.
   
   ![Capture 19](https://user-images.githubusercontent.com/48098768/58503972-4c0f9580-814f-11e9-831c-d02dcc45c337.JPG)

   
## Procedure -2 is to connect wifi module to Internet (or) Wireless Acess point

1) 
