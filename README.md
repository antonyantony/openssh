OpenSSH 6.5p1 

this is a fork of openssh Linux port with an extra patch.  permitremoteopen="XXX" in ~/.ssh/authorized_file  
limit the port(s) allowd to remote forward with -R option.

the patch works on 6.5p1, 6.4p1 and 6.3p1 


./configure
make 




