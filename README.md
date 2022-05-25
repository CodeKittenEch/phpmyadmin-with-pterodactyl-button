# phpmyadmin-with-pterodactyl-button
tutorial for phpmyadmin  instalation with a button for acess on pterodactyl panel 
![image](https://user-images.githubusercontent.com/85484107/170309186-28537bbb-b41e-409a-849f-dcd6f8e656af.png)
the button for acessing phpmyadmin will be placed here 

copy the bash script given below and install the phpmyadmin with button i recommend to use ubuntu 20.04 server 
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
