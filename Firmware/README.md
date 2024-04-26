# [Tutorial about customizing your own keymap](https://github.com/ZitaoTech/zmk_config_Q10)  
If you have any questions about the keymap or you want your own keymap but don't know how to make it, please contact me.

## Interpretation to the different firmware:

bbq10_US_layout_2024.03.07.uf2: default firmware.  

bbq10_sticky_shift.uf2: default firmware feature + sticky shift  
What is [sticky shift](https://zmk.dev/docs/behaviors/sticky-key)?  
A sticky shift stays pressed until another key is pressed, By using a sticky shift, you don't have to hold the shift key to write a capital.  
Why sticky shift?  
Because the keyboard has no integrated diodes, so there might be some ghost typing when you hold some keys together like shift + X.  
So sticky shift is very useful when you want to type some letters capitalized.  
How to check which keys can't be pressed together?  
![Q10_sticky_shift_doc](https://github.com/ZitaoTech/BBQ10-USB_BLE_Keyboard/assets/145678024/0f0f983f-ca8d-41c4-8454-bdd59d8b2e78)  
Go to this [file](https://github.com/ZitaoTech/zmk_config_Q10/blob/main/config/boards/bbq10/bbq10.dts) For those keys that start with same numbers, by the default firmware they are shift, X and B, when you hold shift and press X or B, the keyboard just won't output anything.
