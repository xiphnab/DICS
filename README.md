# DICS
Digitizer Interface Control Software

The purpose of this software is to replace failing hardware solution with a maintainable software solution that exceeds the reliability of the original.


Digitizer ----- Radio ----- Radio ----- DICS ----- Station Processor

DICS to Digitizer Communication 
Request for Data RS232 Packet
  Ranges in length from 18*4=72 bits long to 12*4= 48 bits long
  Counts down device number, when device ID number is less then 0a, packet length is 48
  7e : Start and End of packet
  Seems to be constructing the packet in bytes.  
    First and last Byte is "7e"
    Second Byte is the device ID
    Third is 93 from 0a to 1e, 20 to 23, 25
    Fourth through eighth seems random thought i am sure there is a purpose
    
