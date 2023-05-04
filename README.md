                                                    LAB1_MCU

I. Exercise 1

    From the simulation on Proteus, one more LED is connected to pin PA6 of the STM32 (negative pin of the LED
    is connected to PA6). The component suggested in this exercise is LED-YELLOW, which can be found from the 
    device list. In this exercise, the status of two LEDs are switched every 2 seconds, as demonstrated in the
    figure bellow.
![image](https://user-images.githubusercontent.com/106461205/236115237-e84a9f6c-2065-4e37-8171-76735bbc8723.png)

II. Exercise 2
    
    Extend the first exercise to simulate the behavior of a traffic light. A third LED, named LED-GREEN is added
    to the system, which is connected to PA7. A cycle in this traffic light is 5 seconds for the RED, 2 seconds
    for the YELLOW and 3 seconds for the GREEN. The LED-GREEN is also controlled by its negative pin.
![image](https://user-images.githubusercontent.com/106461205/236116979-1bc70daa-4528-45e7-a6e0-bd7c5fafbfc3.png)
    
III. Exercise 3

    Extend to the 4-way traffic light. Arrange 12 LEDs in a nice shape to simulate the behaviors of a traffic light.
    A reference design can be found in the figure bellow.
![image](https://user-images.githubusercontent.com/106461205/236115480-91707802-13a4-409c-b837-a3827776d1f7.png)

IV. Exercise 4

    Add only one 7 led segment to the schematic in Exercise 3. This component can be found in Proteus by the keyword
    7SEG-COM-ANODE. For this device, the common pin should be connected to the power supply and other pins are supposed
    to connected to PB0 to PB6. Therefore, to turn-on a segment in this 7SEG, the STM32 pin should be in logic 0 (0V).
    
    Implement a function named display7SEG(int num). The input for this function is from 0 to 9 and the outputs are 
    listed as following:
![image](https://user-images.githubusercontent.com/106461205/236115660-0d506f5f-0153-487c-97d3-420910078c6a.png)
    
V. Exercise 5

    Integrate the 7SEG-LED to the 4 way traffic light. In this case, the 7SEG-LED is used to display countdown value.
    
    In this exercise, only source code is required to present. The function display7SEG in previous exercise can be re-used.
![image](https://user-images.githubusercontent.com/106461205/236115875-e2d8a817-bccc-44f5-bf99-ea21e935eaf8.png)

VI. Exercise 6

    In this exercise, a new Proteus schematic is designed to simulate an analog clock, with 12 different number. The
    connections for 12 LEDs are supposed from PA4 to PA15 of the STM32. The arrangement of 12 LEDs is depicted as follows.

![image](https://user-images.githubusercontent.com/106461205/236116236-697966ec-5a10-4a24-915e-5a6281bfdad9.png)

VII. Exercise 7

    Implement a function named clearAllClock() to turn off all 12 LEDs. Present the source code of this function.
    
    void clearAllClock () {
    
    // TODO
    
    }
    
VIII. Exercise 8

    Implement a function named setNumberOnClock(int num). The input for this function is from 0 to 11 and an appropriate
    LED is turn on. Present the source code of this function.
    
IX. Exercise 9 

    Implement a function named clearNumberOnClock(int num). The input for this function is from 0 to 11 and an appropriate
    LED is turn off.
    
X. Exercise 10

    Integrate the whole system and use 12 LEDs to display a clock. At a given time, there are only 3 LEDs are turn on for
    hour, minute and second information.
