# lcd_driver
1x16 HD44780 LCD driver for stm32. 
The LCD in question uses addressing 0x00-0x07 for first 8 and 0x40-0x47 for the last 8 chars.

## Usage
Call  ```lcd_init()```  before anything else.

### GPIO pin naming
Header main.hh is included to get the CubeMX generated GPIO pin and port macros. Naming is as follows:
- Enable: LCD_EN_GPIO_Port, LCD_EN_Pin
- Register select: LCD_RS_GPIO_Port, LCD_RS_Pin
- Read/Write: LCD_RW_GPIO_Port, LCD_RW_Pin
- Data bus pins: LCD_DBX_GPIO_Port, LCD_DBX_Pin
