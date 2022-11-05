TODO:
use your Lab 1 firefly code to generate ADPS9960 I2C traffic and display it on a lab oscilloscope
take a screenshot of some portion of this exchange, and figure out/annotate what's happening based on the protocol documentation in the ADPS9960 datasheet

Below is the result of the I2C traffic![8a124a2c8a1e840b879da6cb5146789](https://user-images.githubusercontent.com/113710845/200096573-ac745f73-8770-4a41-98d9-b672c2410253.jpg)
![dec04f5ae80a6679e9fffeee5eddb84](https://user-images.githubusercontent.com/113710845/200096577-27c5b2b3-eb52-4660-86a9-ae969f06ae47.jpg)
![edbaba9eff10a9d6287369a32666f9a](https://user-images.githubusercontent.com/113710845/200096579-8e69200a-cb7c-4bb7-b6cd-a35e4ee92878.jpg)
# annotation
![20190715145908215](https://user-images.githubusercontent.com/113710845/200096819-9b34699a-f46d-4f4f-8b3d-858f5401366c.png)<br>
Every time the host transmits a byte of data, that is, every time the peripheral receives a byte of data, the peripheral will pull down the SDA data line to answer (ACK) when the 9th clock pulse arrives. The SDA data line must be at a stable low level, indicating that a byte of data has been received
