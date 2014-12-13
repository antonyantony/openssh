How to restrict ssh remote portforwarding to specified port(s).

This is a fork of OpenSSH Linux port with an extra patch; permitremoteopen="XXX" in ~/.ssh/authorized_file  

permitremoteopen limits the port(s) allowd to remote forward with -R option.
the patch will work on 6.7p1, 6.6p1, 6.5p1, 6.4p1 and 6.3p1

./configure
make 

example: for ~/.ssh/authorized_keys
permitremoteopen="2026" ssh-rsa AAAA3NzaC1 antony@phenome.org
Only port 2026 will allowed with -R option
