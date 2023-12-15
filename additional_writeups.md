## additional writeups

### Forensics

#### sleuthkit intro 

opened the challenge     
downloaded the file using `wget` command         
used `cat disk.img.gz` . Didn't work       
used `nc saturn.picoctf.net 64605 ` . It started asking about length of linux partition        
went through the primer for help        
learnt that you have to use the mmls command     
used `mmls disk.image.gz` . Didn't work      
used `mmls disk.image` . Gave data      
used `nc saturn.picoctf.net 64605` . Entered the length of the linux distribution given     
got the flag    
```  
flag - picoCTF{mm15_f7w!}  
```

#### sleuthkit apprentice

opened the challenge     
downloaded the file using `wget`      
extracted the file using `gunzip`      
used `mmls` command       
found the fourth partition to be the most lengthiest      
read through the basics of disk analysis in primer      
used `fls -o 360448 disk.flag.img `        
used `fls -o 360448 disk.flag.img 1995` to enter root directory     
used `fls -o 360448 disk.flag.img 2371` to enter my_folder directory      
used `icat -o 360448 disk.flag.img 2371` to read the data in my_folder     
got the flag     
```
flag - picoCTF{by73_5urf3r_adac6cb4}
```

