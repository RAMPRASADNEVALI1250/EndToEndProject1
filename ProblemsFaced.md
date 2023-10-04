Before troubleshooting any problems **reboot** ur system and check if anything works(classic) 

1. Installing Jenkins
     When installing jenkins gotthe below error
   **YUM updates fail with: [Errno 14] curl#60 - "Peer's Certificate has expired."**
   for me it was docker that is having issues(using old VM)
   Resolution:
         The affected repository will need to be fixed or disabled until such time as the SSL error is no longer occurring.
         The repository will be located in the /etc/yum.repos.d/ directory and it can be disabled by changing the "enabled=1" lines to "enabled=0".

2. Firewalls - firewalld
   When working on the VM(created via virtual box) uses Bridged adoptor
   since jenkins runs on port 8080 by default - not able to access jenkins console using vm ip:8080
   a. tried using ufw package - ufw enable,allow etc
   b. but the default firewall manager worked **firewall-cmd --add-port=8080/tcp**  -- with this I am able to access the
        jenkins console
