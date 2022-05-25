# phpmyadmin-with-pterodactyl-button
tutorial for phpmyadmin  instalation with a button for acess on pterodactyl panel 
![image](https://user-images.githubusercontent.com/85484107/170309186-28537bbb-b41e-409a-849f-dcd6f8e656af.png)
the button for acessing phpmyadmin will be placed here 

copy and paste  the command given below and install the phpmyadmin with button, I recommend to use ubuntu 20.04 server 
```
bash <(curl https://raw.githubusercontent.com/CodeKittenEch/phpmyadmin-with-pterodactyl-button/main/pma.sh)
```
after the installation if your panel or php artisan is down please remeber to make it up 

```
php /var/www/pterodactyl/artisan up 
```
or 
```
php artisan up 
```

after the sucessfull installation 
go to the ssh of your server in which installed the pterodactyl and the phpmyadmin
login via root or 
```
sudo su -
```
after this  
use command 
```
nano /var/www/pterodactyl/public/pma_redirect.html
```
![image](https://user-images.githubusercontent.com/85484107/170313487-0f4eee2e-22e6-471a-b10c-189bacde50c1.png)
edit the location.replace(http://yourdomain.com/phpmyadmin) to your phpmyadmin adress
example with deafualt location if my domain is endcloudhost.com 
![image](https://user-images.githubusercontent.com/85484107/170314082-3c5a25d6-6839-4aec-b897-112b7bea4af6.png)
or if my server ip is 172.1.1
![image](https://user-images.githubusercontent.com/85484107/170314290-157b23d0-b41a-4eeb-a301-20fc975d7c81.png)

if you domain is'nt connecting don't forgot to correct https or http

after editin hit ctrl key + x 
![image](https://user-images.githubusercontent.com/85484107/170314640-eecb7c6f-2e9b-4480-a759-38ab291f3f77.png)
and y 
![image](https://user-images.githubusercontent.com/85484107/170314710-e40f4882-0dcb-4201-a635-c567d130023c.png)
and the enter key

after you come back to the ssh normal windows do restart the nginx webserver by 
```
service nginx restart
```

for support contact me on discord
!  {Cᴏᴅᴇ} _Kɪᴛᴛᴇɴ™ </>#9960



