# cron project
```
crontab -e //add cron
crontab -l //see cron
```
# code cron
```
* * * * * perintah yang akan dieksekusi
– – – – –
| | | | |
| | | | +—– day of week (0 – 7) (Sunday=0)
| | | +——- month (1 – 12)
| | +——— day of month (1 – 31)
| +———– hour (0 – 23)
+————- min (0 – 59)
```
# example cron 
```
* * * * * /home/user/script.sh //tiap menit
```
# example cron to log
```
0 */8 * * * /root/cek.sh >> /root/cek.log // cron tiga kali sehari
```
# example sh script
```
#!/bin/bash
tanggal=$(date +"%m-%d-%Y")
waktu=$(date +"%T")
echo "Active On $tanggal pukul $waktu."
```
