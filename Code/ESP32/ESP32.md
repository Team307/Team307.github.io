This is to storing Teams ESP32 code

<br/>

![Topic](https://user-images.githubusercontent.com/122499998/235216091-8686b6fc-fce7-4e7c-8b9d-a43471017788.png)

<br/>
  <br/>
  
  Main.C Code
  
  <br/>
  
#include "mcc_generated_files/mcc.h"
#include "mcc_generated_files/examples/i2c2_master_example.h"
#include "mcc_generated_files/i2c2_master.h"
#include "mcc_generated_files/examples/i2c1_master_example.h"
#include "mcc_generated_files/i2c1_master.h"

void EUSART1Transmit(void)
{
    EUSART1_Receive_ISR();

    volatile uint8_t unixData;

    if(EUSART1_is_rx_ready()){
        unixData = EUSART1_Read();
        if(EUSART1_is_tx_ready()){
            EUSART1_Write(unixData);
        }
        if(EUSART1_is_tx_done()){

        }
        //LED_0_Toggle();
    }
    // add your EUSART2 interrupt custom code
}

void main(void)
{

    
    SYSTEM_Initialize();
    EUSART1_SetRxInterruptHandler(EUSART1Transmit);
    
    
    INTERRUPT_GlobalInterruptEnable();
    INTERRUPT_PeripheralInterruptEnable();
    
    printf("starting");
    
    int8_t var;
    uint8_t buff[4];
    uint16_t conver = 0;
    double humidity = 0;
    
    while (1)
    {
        {
   var = I2C2_Read1ByteRegister(0x4C, 0x00);
   printf("Temp: %u C \n \r", var);

      __delay_ms(1000);
        }   
        
    { 
     //we want to trigger the chip to take a 'measurement' and wait for that to happen;
     I2C1_ReadNBytes(0x27, buff, 2); 
     __delay_ms(50); 
     //I2C1_ReadNBytes(0x27, buff, 4);
     //conver = (buff[0] << 8 | buff[1]) & 0x3fff;
     
     for(int i=0; i<sizeof(buff); i++){
     humidity = 10*conver + buff[i];
     }
     
     printf("The Humidity is %u \r \n", humidity);

     __delay_ms(1000);
 
    }
  }
}

<br/>