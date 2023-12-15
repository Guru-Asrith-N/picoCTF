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

