#Tp réseau 1

🌞 Adresses IP de ta machine

```
ipconfig /all
Adresse IPv4 : 10.33.79.0
```

🌞 Si t'as un accès internet normal, d'autres infos sont forcément dispos...

```
PS C:\Users\Ethan> ipconfig /all
Carte réseau sans fil Wi-Fi :

   Suffixe DNS propre à la connexion. . . :
   Description. . . . . . . . . . . . . . : Realtek RTL8821CE 802.11ac PCIe Adapter
   Adresse physique . . . . . . . . . . . : 74-97-79-66-39-B3
   DHCP activé. . . . . . . . . . . . . . : Oui
   Configuration automatique activée. . . : Oui
   Adresse IPv6 de liaison locale. . . . .: fe80::23f8:c185:1b16:5353%19(préféré)
   Adresse IPv4. . . . . . . . . . . . . .: 10.33.79.0(préféré)
   Masque de sous-réseau. . . . . . . . . : 255.255.240.0
   Bail obtenu. . . . . . . . . . . . . . : vendredi 27 septembre 2024 13:38:40
   Bail expirant. . . . . . . . . . . . . : samedi 28 septembre 2024 13:38:40
   🌞 Passerelle par défaut. . . . . . . . . : 10.33.79.254
   Serveur DHCP . . . . . . . . . . . . . : 10.33.79.254
   IAID DHCPv6 . . . . . . . . . . . : 292853625
   DUID de client DHCPv6. . . . . . . . : 00-01-00-01-2E-46-80-B3-74-97-79-66-39-B3
   Serveurs DNS. . .  . . . . . . . . . . : 1.1.1.1
                                       1.0.0.1
   NetBIOS sur Tcpip. . . . . . . . . . . : Activé
   ```

🌞 Envoie un ping vers...

```
PS C:\Users\Ethan> ping 10.33.79.0

Envoi d’une requête 'Ping'  10.33.79.0 avec 32 octets de données :
Réponse de 10.33.79.0 : octets=32 temps<1ms TTL=128
Réponse de 10.33.79.0 : octets=32 temps<1ms TTL=128
Réponse de 10.33.79.0 : octets=32 temps<1ms TTL=128
Réponse de 10.33.79.0 : octets=32 temps<1ms TTL=128

Statistiques Ping pour 10.33.79.0:
    Paquets : envoyés = 4, reçus = 4, perdus = 0 (perte 0%),
Durée approximative des boucles en millisecondes :
    Minimum = 0ms, Maximum = 0ms, Moyenne = 0ms

```

```
PS C:\Users\Ethan> ping 127.0.0.1

Envoi d’une requête 'Ping'  127.0.0.1 avec 32 octets de données :
Réponse de 127.0.0.1 : octets=32 temps<1ms TTL=128
Réponse de 127.0.0.1 : octets=32 temps<1ms TTL=128
Réponse de 127.0.0.1 : octets=32 temps<1ms TTL=128
Réponse de 127.0.0.1 : octets=32 temps<1ms TTL=128

Statistiques Ping pour 127.0.0.1:
    Paquets : envoyés = 4, reçus = 4, perdus = 0 (perte 0%),
Durée approximative des boucles en millisecondes :
    Minimum = 0ms, Maximum = 0ms, Moyenne = 0ms
```

```
PS C:\Users\Ethan> ping 10.33.79.254

Envoi d’une requête 'Ping'  10.33.79.254 avec 32 octets de données :
Délai d’attente de la demande dépassé.
Délai d’attente de la demande dépassé.
Délai d’attente de la demande dépassé.
Délai d’attente de la demande dépassé.

Statistiques Ping pour 10.33.79.254:
    Paquets : envoyés = 4, reçus = 0, perdus = 4 (perte 100%),
```

```
PS C:\Users\Ethan> ping 10.33.66.78

Envoi d’une requête 'Ping'  10.33.66.78 avec 32 octets de données :
Réponse de 10.33.66.78 : octets=32 temps=115 ms TTL=64
Réponse de 10.33.66.78 : octets=32 temps=35 ms TTL=64
Réponse de 10.33.66.78 : octets=32 temps=53 ms TTL=64
Réponse de 10.33.66.78 : octets=32 temps=77 ms TTL=64

Statistiques Ping pour 10.33.66.78:
    Paquets : envoyés = 4, reçus = 4, perdus = 0 (perte 0%),
Durée approximative des boucles en millisecondes :
    Minimum = 35ms, Maximum = 115ms, Moyenne = 70ms
```

```
PS C:\Users\Ethan> ping root-me.org

Envoi d’une requête 'ping' sur root-me.org [212.129.28.16] avec 32 octets de données :
Réponse de 212.129.28.16 : octets=32 temps=12 ms TTL=55
Réponse de 212.129.28.16 : octets=32 temps=12 ms TTL=55
Réponse de 212.129.28.16 : octets=32 temps=17 ms TTL=55
Réponse de 212.129.28.16 : octets=32 temps=14 ms TTL=55

Statistiques Ping pour 212.129.28.16:
    Paquets : envoyés = 4, reçus = 4, perdus = 0 (perte 0%),
Durée approximative des boucles en millisecondes :
    Minimum = 12ms, Maximum = 17ms, Moyenne = 13ms
```

```
PS C:\Users\Ethan> nslookup thinkerview.com
Serveur :   one.one.one.one
Address:  1.1.1.1

Réponse ne faisant pas autorité :
Nom :    thinkerview.com
Addresses:  2a06:98c1:3120::6
          2a06:98c1:3121::6
          188.114.96.6
          188.114.97.6

```

```
PS C:\Users\Ethan> nslookup www.wikileaks.org
Serveur :   one.one.one.one
Address:  1.1.1.1

Réponse ne faisant pas autorité :
Nom :    wikileaks.org
Addresses:  51.159.197.136
          80.81.248.21
Aliases:  www.wikileaks.org
```

```
PS C:\Users\Ethan> nslookup torproject.org
Serveur :   one.one.one.one
Address:  1.1.1.1

Réponse ne faisant pas autorité :
Nom :    torproject.org
Addresses:  2a01:4f9:c010:19eb::1
          2a01:4f8:fff0:4f:266:37ff:fe2c:5d19
          2620:7:6002:0:466:39ff:fe7f:1826
          2a01:4f8:fff0:4f:266:37ff:feae:3bbc
          2620:7:6002:0:466:39ff:fe32:e3dd
          204.8.99.146
          116.202.120.165
          204.8.99.144
          95.216.163.36
          116.202.120.166
```


🌞 Effectue un scan du réseau auquel tu es connecté
```
🌞 PS C:\Users\Ethan> nmap -sn -PR 10.33.64.0/20
RTTVAR has grown to over 2.3 seconds, decreasing to 2.0
Stats: 0:00:34 elapsed; 0 hosts completed (0 up), 4095 undergoing ARP Ping Scan
ARP Ping Scan Timing: About 25.49% done; ETC: 17:30 (0:01:39 remaining)
Stats: 0:00:35 elapsed; 0 hosts completed (0 up), 4095 undergoing ARP Ping Scan
ARP Ping Scan Timing: About 25.87% done; ETC: 17:30 (0:01:40 remaining)
Nmap scan report for 10.33.66.78
Host is up (0.055s latency).
MAC Address: E4:B3:18:48:36:68 (Intel Corporate)
Nmap scan report for 10.33.69.82
...
Nmap done: 4096 IP addresses (166 hosts up) scanned in 132.43 seconds
```

🌞 Changer d'adresse IP

```
Carte réseau sans fil Wi-Fi :

   Suffixe DNS propre à la connexion. . . :
   Description. . . . . . . . . . . . . . : Realtek RTL8821CE 802.11ac PCIe Adapter
   Adresse physique . . . . . . . . . . . : 74-97-79-66-39-B3
   DHCP activé. . . . . . . . . . . . . . : Non
   Configuration automatique activée. . . : Oui
   Adresse IPv6 de liaison locale. . . . .: fe80::23f8:c185:1b16:5353%19(préféré)
   🌞Adresse IPv4. . . . . . . . . . . . . .: 10.33.79.4(préféré)
   🌞Masque de sous-réseau. . . . . . . . . : 255.255.240.0
   🌞Passerelle par défaut. . . . . . . . . : 10.33.79.254
   IAID DHCPv6 . . . . . . . . . . . : 292853625
   DUID de client DHCPv6. . . . . . . . : 00-01-00-01-2E-46-80-B3-74-97-79-66-39-B3
   Serveurs DNS. . .  . . . . . . . . . . : 1.1.1.1
                                       1.0.0.1
   NetBIOS sur Tcpip. . . . . . . . . . . : Activé

``` 