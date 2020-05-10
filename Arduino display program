#include <Arduino.h>
#include <U8g2lib.h>
#include <Wire.h>

U8G2_SSD1309_128X64_NONAME2_F_HW_I2C u8g2(U8G2_MIRROR,/* reset=*/ U8X8_PIN_NONE);



void setup(void) 
{
  u8g2.begin();  
}

void loop(void) 
{
  
  u8g2.clearBuffer();					// clear the internal memory
  u8g2.setFont(u8g2_font_5x8_tf);	// choose a suitable font
  u8g2.setDisplayRotation(U8G2_R1);
  u8g2.drawUTF8(0,10,"Hello World!");	// write something to the internal memory
  u8g2.sendBuffer();					// transfer internal memory to the display
  delay(1000);  
  
}
