# Sample HTML website 

Sample HTML/CSS web app that you can deploy to any Cloud provider. 

yum install httpd git  -y 

git clone https://github.com/sonulodha/webpage.git

mv webpage/* /var/wwww/html/

create configuration file

    vim /etc/httpd/conf.d/ite.conf
       <Virtualhost *:80>
       Servername hostname
       ServerAdmin root@localhost
       DocumentRoot /var/www/html/
       </VirtualHost>

systemctl enable httpd

systemctl start httpd

firefox localhost



