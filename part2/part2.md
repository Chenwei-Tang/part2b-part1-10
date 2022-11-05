TODO:
Create a REPL to let you read and write RP2040 registers from a console. You should be able to:

select any 32-bit address to read/write (even if not a valid RP2020 address)
read/write any 32-bit value to this address
read/write using any of the atomic bit-setting aliases and a 32-bit mask

I attach the code in the folder. Below are the results.


I read the value of ADDRESS: GPIO_BASE+0X0A8,then i get the 18 bit of it, it's "1". At last I write to GPIO_BASE+0X0E8, then I read it and verify.
![image](https://user-images.githubusercontent.com/113710845/200096325-5562867a-4650-44d3-b866-7569c8f6e50d.png)
