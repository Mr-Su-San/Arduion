1. Download and install WinAVR. After installation, these two paths will automatically generate C:\WinAVR-20100110\bin C:\WinAVR-20100110\utils\bin and add the path to the system Path.

2. Edit the assemble code and generate the .hex file.

3. Download and install the Arduino IDE.

4. Go to the arduino installation directory and find the file \hardware\arduino\avr\boards.txt
	4.1. Find the corresponding board paragraph in the file, for example uno : uno.name=Arduino/Genuino Uno
	4.2. Protocol (arduino) : uno.upload.protocol=arduino
	4.3. baud rate (115200) : uno.upload.speed=115200

5. Edit Upload.bat
	5.1. avrdude -v -c [p] -P [c] -b [b] -p atmega328p -U flash:w:BeeClient.hex:i
	5.2. [p] is the communication protocol.
	5.3. [c] To connect arduino com port.
	5.4. [b] is baud rate.

6. Upload hex to upload hex to arduino.
