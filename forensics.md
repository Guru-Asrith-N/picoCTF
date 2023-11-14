### writeup on forensics

started reading primer initially whose link is sent in readme

#### tunn3l_v1s10n

openned the tunn3l_v1s10n challenge    
downloaded the link in webshell using `wget https://mercury.picoctf.net/static/01be2b38ba97802285a451b94505ea75/tunn3l_v1s10n `    
used `file tunn3l_v1s10n` . It showed that it is a data file   
used `cat tunn3l_v1s10n` . It didn't work  
used `grep picoCTF tunn3l_v1s10n` . It didn't work     
used `strings tunn3l_v1s10n` . It didn't work       
used `grep pico tunn3l_v1s10n | cat > data`. It didn't work     
got stuck for a while     
saw writeups 'https://github.com/vivian-dai/PicoCTF2021-Writeup/blob/main/Forensics/tunn3l%20v1s10n/tunn3l%20v1s10n.md'   
opened ubuntu because hex editor is required   
opened it using a image viewer. Got to know it was a 'BMP' file as well as the fact that there was a problem in the header     
downloaded 'GHex editor'      
downloaded the file in computer    
opened it in 'GHex editor'   
read about this file 'http://www.ece.ualberta.ca/~elliott/ee552/studentAppNotes/2003_w/misc/bmp_file_format/bmp_file_format.htm' and 'http://www.novell.com/documentation/ndsv8/usnds/c1help/novell_common/hexeditor.html' in the writeup to understand about hex editor and BMP header   
noticed the incongruencies in header and width size . Increased the height of image as indicated in hint . Made the size of the width and header equal to make it a square     
opened the image in a photo editor 'photopea.com' to view the image   
got the flag    
```
flag : picoCTF{qu1t3_a_v13w_2020}
```




