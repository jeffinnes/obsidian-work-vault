## Rando Mongo queries:

Find all records after a time stamp

```JavaScript
{createdAt: { $gt: ISODate('2021-05-08T11:54:32.097') }}
```

  

## Helpful JavaScript things

Just a pause in execution

```JavaScript
const wait = (timeToDelay) => new Promise((resolve) => {
  setTimeout(resolve, timeToDelay);
});

...

await wait(3000);
```

  

## Git commands

Local commands to run after changing "master" branch to "main" on GitHub

```Bash
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```

  

## Find top TCP connections on LiquidWeb server

Shell Command to find the top 10 TCP Connection IP sources. For good measure, the IP addresses can be checked on [https://www.abuseipdb.com/](https://www.abuseipdb.com/)

```Bash
[root@host ~]#  grep -r "03/Feb/2025" /var/www/vhosts//buffaloexchange.com/logs/access_ssl_log | awk '{print $1}'|cut -d':' -f1|sort |uniq -c|sort -n|tail -n10
    217 99.138.105.59
    230 66.249.65.237
    356 13.56.238.252
    414 35.88.87.248
    443 195.242.10.185
    577 66.249.65.236
    580 172.16.166.76
   1542 65.2.146.204
   1597 66.249.65.235
 390420 198.23.212.26 
```