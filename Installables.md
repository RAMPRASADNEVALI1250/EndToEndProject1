Install Java,Jenkins,git and neccessory packages

1. Install java 
    yum list avilable | grep openjdk

    yum install {openjdk-11-from above list}

2. Install Jenkins
    wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo

    yum install deltarpm

    rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
    
    yum upgrade

    yum install jenkins

    systemctl daemon-reload


4. Install git
    
    yum install git


Other installs
    
    yum install wget
    yum install tree


