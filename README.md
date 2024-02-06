# Bi0s-phase2
      
# MISC
### **1**

![Screenshot from 2024-02-06 20-40-51](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/887df47a-bb7b-460b-a2a6-d93cda00af50)
- I have used strings commands to extract the strings in the executable file.Then i found some base64 text. I have decoded the text and found a file in a git repo.
 ![Screenshot from 2024-02-06 20-44-16](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/ebfbd463-6b0e-4b1a-b56e-b905f265fc13)
- Then i have a found octal encodig in the file and i have decoded it. Then i have found a base64 encoded image . Then i have decoded the image and found the flag
     
### **3**

![Screenshot from 2024-02-06 20-50-44](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/9f732866-4835-49b7-905d-6b3851385209)
- In the attachement i have found a mysterious wingding text. I have written a python script for wingding extraction .The link is below
  -[wingding repo link](https://github.com/komalrao1/wingding-extraction).
- Using the script i have found out the flag
     
### **4**
![image](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/1868e6cf-1e9d-4819-9b03-715b8ffcc78d)
- I have opened the attachment file and suspected the text encoding as base64 encoding. I have decoded the msg.txt file in terminal using **base64 -d** command.I have decode the msg.txt file 35 times at 35th time i have found a python script using that
  - ![image](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/9a18b3dc-cfe2-414d-8c96-785cd90297b8)
- I have understood the code and shorted the code to the following and got the flag
  - ![Screenshot from 2024-02-06 21-07-02](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/2c5d9aaa-2c30-4385-a8b4-d4f15e6f27dc)
      
### **5**
![image](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/498209ec-dae4-46db-b64f-b927310d03f4)
- I have opened the attachment file and confirmed the encoding as hex encoding . I have decoded it using hex and i have found the following text
  - ![Screenshot from 2024-02-06 21-11-36](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/4cd2b37b-f23b-4db9-950f-3ac9a9f2ec8c)
- I have tried many ways and read many writeups and found the text encoding as a pattern. If we assume the characters in each set of pattern in keyboard we can find a pattern such that there is a particular key in between the each set. For example if we consider **XDV** , **C** is between **XDV**. Like wise i found complete pattern



# REV 

### **1**
![image](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/8489bfce-5b92-4e48-8955-27ce9db8979e)
- Using Ghidra tool i have opened the source code and written a python script to solve the flag
  - ![Screenshot from 2024-02-06 21-26-22](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/3fb611e3-48e3-4ee2-a6bd-69ddec43a79b)
- The above code does the encrypted flag **XOR** with unicode of key - 22 . It results the flag

### **2**
![Screenshot from 2024-02-06 21-32-34](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/ef2884de-8d82-43d9-a8d4-f8ec6a585db3)
- I have deompiled the attachment chall.pyc to .py file using online compiler
  - ![Screenshot from 2024-02-06 21-34-29](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/554f3426-507d-46bc-9ae2-eebf3624ebff)
- Then i have written a python script to get the flag.
  - ![Screenshot from 2024-02-06 21-42-07](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/4f96768a-7f84-4bdd-9e7f-d62bf810dc0e)

### **3**
![Screenshot from 2024-02-06 21-43-46](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/d40364b9-15df-467c-9fff-ce312ed15bba)
- I have run the attachment executable file in terminal and undertood the syntax of executing the file
  - ![Screenshot from 2024-02-06 21-46-14](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/508c4504-b82a-4af8-abc8-d610c8e0028d)
- Then using **Ghidra** I opened the source code and found the passowrd in hex form which is **0x35010ff**.
  - ![Screenshot from 2024-02-06 21-47-36](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/e89638e8-310d-4868-bdc1-8a62533501cb)
- I have deocded the hex encoded password sing cyberchef .
  - ![Screenshot from 2024-02-06 21-56-36](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/6bfa34e2-5fd5-4f1c-a977-d3b2d117cc14)
- The i have run the exe file and got the flag
  - ![Screenshot from 2024-02-06 21-56-22](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/cfcc96d0-b12c-44f2-ad00-451113e15611)

### **4**
![Screenshot from 2024-02-06 21-59-06](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/e9b0047c-d614-4940-a1c0-beb8ff9cf0db)
- I have run the exe file in terminal and understood the syntax .Then i have opened the source code of the file using ghidra.
  - ![Screenshot from 2024-02-06 22-00-47](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/2de9ae7b-3d8b-44e7-b8c0-e6abcc714385)
- In the code the conditions of the password are the password must me 10 characters ans 5th character must be **@** ,Rest characters can be anything.Then i have run the file.
  -![Screenshot from 2024-02-06 22-05-04](https://github.com/komalrao1/Bi0s-phase2/assets/147682987/7ebfb218-529e-492b-9c7c-ddbac16c6345)



------------------------------------------------------------**THE END**------------------------------------------------------------










