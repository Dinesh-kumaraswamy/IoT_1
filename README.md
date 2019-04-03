#include <SoftwareSerial.h>
SoftwareSerial esp(2, 3);

void setup() { 

Serial.begin(9600);   // 9600 IS BAUD RATE FOR SERIAL CONNECTION BETWEEN ARUDNIO AND ARUNIO IDE ( DISPLAYED ON COM )
esp.begin(9600);      //  9600 IS BAUD RATE FOR CONNECTION OF esp 8266 WIFI MODULE
esp.println("AT"); 
response(2000); 
esp.println("AT+CIOBAUD=9600"); 
response(1000); 
esp.println("AT+CWMODE=1"); 
response(2000);
esp.println("AT+CWJAP=\"SSIDNAME\",\"SSIDPASSWORD\"\r\n"); 
response(10000);  

}
void loop() { 

}
