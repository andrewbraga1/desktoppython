##Passos para execução do PL2303
#Listando as portas
python -m serial.tools.list_ports
/dev/ttyUSB0
>>> import serial
>>> ser = serial.Serial('/dev/ttyUSB0')  # open serial port
>>> print(ser.name)         # check which port was really used
>>> ser.write(b'hello')     # write a string
>>> ser.close() 
