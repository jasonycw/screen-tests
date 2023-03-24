# What is this?
To reporduce rtings' black uniformity test pattern from https://www.rtings.com/monitor/tests/picture-quality/black-uniformity for testing blooming and black ligth bleeding.
[![image](https://www.rtings.com/images/test-materials/2015/203_Black_Uniformity.png)](https://www.rtings.com/images/test-materials/2015/203_Black_Uniformity.png)

## ChatGPT prompt

1. ```
   Create a webpage with black background and a white cross in the middle of the screen
   ```
2. ```
   It is not a cross shape and the line are not crossing together.
   Also, don't need any round corner for the cross
   ```
3. ```
   This only result in 2 horizontal line and a dot on top, not a cross
   ```
4. ```
   I don't want to have a border surrounding the cross. And I want a cross like "+" not "x"
   ```
5. ```
   Good, now I want the length of the horizontal line to be 25% of the screen width and the vertical line to be 20% of the screen height
   Also, the lines width should be 8px
   ```
6. ```
   The vertical line is a bit off center, should be move downward a bit
   Also, change the horizontal line to be 30% of the width
   ```
7. ```
   Now the whole cross is off center
   Vertical line should be moved down a bit
   Horizontal line should be moved up a bit
   ```
8. ```
   Now this is not a cross anymore
   The horizontal line is still too low, margin-top -8px seems to be more centered
   The vertical line is completely off now and not crossing the horizontal line properly
   ```
9. ```
   Now the length of the line are not relative to the screen anymore
   ```
10. ```
    This is incorrect, the cross is now relative to the div class=cross instead of relative to the screen
    ```
11. ```
    No, this is incorrect again, the cross is still relative to the .cross div instead of the screen
    ```
12. ```
    No, this is incorrect, the cross is not relative to the screen again. It is too small
    ```
13. ```
    Now the cross is not the correct size anymore
    The length of the horizontal line to be 30% of the screen width and the vertical line to be 19% of the screen height
    Also, the lines width should be 8px
    ```
14. ```
    The cross is stuck at 150x150
    ```
15. ```
    Should remove margin-top: -4px; and margin-left: -4px; to properly align the cross in the centre of the screen
    ```
16. ```
    Now add a 40x40 white square in the middle of the screen as well
    ```
    
![chatGPT](https://user-images.githubusercontent.com/4518597/227432443-f0fb3ca5-eb33-45b0-8fa3-2c22da6fe415.png)

