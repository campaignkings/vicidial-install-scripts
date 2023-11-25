# vicidial-install-scripts

hostnamectl set-hostname xxxxxx.xxxxx.xxx
### Use YOUR SubDomain

vi /etc/hosts
##Change domain name for actual server ip (xxx.xxx.xxx.xxx   complete domain name    subdomain only)

timedatectl set-timezone America/New_York

yum check-update
yum update -y
yum -y install epel-release
yum update -y
yum install git -y
yum install -y kernel*

#Disable SELINUX
<br>
sed -i 's/SELINUX=enforcing/SELINUX=disabled/g' /etc/selinux/config    
<br>
reboot


cd /usr/src/
<br>
git clone https://github.com/campaignkings/vicidial-install-scripts.git
<br>
cd vicidial-install-scripts
<br>
chmod +x alma9.sh
./alma9.sh
