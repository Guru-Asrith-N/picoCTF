### writeup on reverse engineering

#### GDB baby step 1

opened the challenge    
downloaded the the file `wget https://artifacts.picoctf.net/c/512/debugger0_a`     
used `gdb debugger0_a`     
got stuck            
referred to writeups      
enetered functions . Didn't work     
entered info functions . worked      
made the syntax format as intel since it is the most widely used processor    
used `set disassembly-flavor intel`     
used `disassemble main`     
found eax and next to it the register number in hexadecimal format     
converted the hexadecimal format to decimal since it was asked in question     
got the decimal as '549698'     
got the flag     
```
flag : picoCTF{549698}
```


#### 
