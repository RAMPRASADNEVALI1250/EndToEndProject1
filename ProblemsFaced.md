Before troubleshooting any problems **reboot** ur system and check if anything works(classic) 

1. Installing Jenkins
     When installing jenkins gotthe below error
   **YUM updates fail with: [Errno 14] curl#60 - "Peer's Certificate has expired."**
   for me it was docker that is having issues(using old VM)
   Resolution:
         The affected repository will need to be fixed or disabled until such time as the SSL error is no longer occurring.
         The repository will be located in the /etc/yum.repos.d/ directory and it can be disabled by changing the "enabled=1" lines to "enabled=0".
