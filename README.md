# University WiFi Configuration file
Wifi configuration for linux user connecting to a university i.e entreprise network

## Setup

From user keith on [Stackoverflow](https://askubuntu.com/questions/279762/how-to-connect-to-wpa2-peap-mschapv2-enterprise-wifi-networks-that-dont-use-a-c) : 

```
sudo su
cd /etc/NetworkManager/system-connections
sudo touch SSID #SSID is the name of the profile, e.g. eduroam
sudo nano SSID
```

And edit the following lines the repo's code  

add your SSID e.g ETS-Campus 
```
id=my_SSID
```
change to your user instead of my_user
```
permissions=user:my_user:;
```
add your id
```
identity=am00000
```

and you can add your password by replacing
```
password-flags=1 
```
with 
```
password=my_password
```
