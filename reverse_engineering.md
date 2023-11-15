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


#### ARMassembly 0

opened the challenge     
downloaded the file `wget https://mercury.picoctf.net/static/b3b17204c7ce77f184a397c4fae4a35b/chall.S`   
used `file chall.S` . It is assembly source and ASCII text   
used `cat chall.S`    
didn't know what to do after this so referred writeups 'https://ctftime.org/writeup/26962'    
from writeup w0 =3854998744  and w1 = 915131509     
subtract w1 from w2 (smaller from larger)     
didn't understand so referred this 'https://www.youtube.com/watch?v=BMvda3d0dt8'    
converted largest value to 32 bit hexadecimal      
```
flag : picoCTF{e5c69cd8}
```
