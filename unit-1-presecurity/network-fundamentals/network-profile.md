1. laitokseni ipv4 osoite on 192.168.101.2xx, ja mac osoite on 10-ff-e0-31-xx-xx
2. yksityinen ip näkyy vain omassa kotiverkossasi ja julkinen nökyy koko internettiin. kotiverkko käyttää turvallisuussyistä yksityistä ip:tä
3. ip osoite on muuttuva ja mac addresson laitteessa kiinteä. ip toimii kerroksella kolme ja mca kerroksella kaksi
4. osoitteita on maksimissaan 256. laitteille niistä käytettävissä on 254, koska yksi on verkko-osoite ja toinen on lähetys osoite.
jos ip osoite on tehtävässä mainittu 192.168.1.37/24, verkko osoite on 192.168.1.0 ja lähetys osoite on 192.168.1.255
5. laitteeni default gateway ip on 192.168.101.1
6. omalle gatewaylle keskimääräinen aika oli 0ms ja 1.1.1.1 oli 3ms. tämä johtuu siitä että toinen on suoraan omalla laitoksella
7. example.com pingaamisen mahdollistaa dns, joka muuttaa nettisivun IP-osoitteeksi
8. dns palvelimeni on sama kuin default gateway
9. example.com palautti yhteensä neljä eri osoitetta
10. jengi näkis ainaki varmaa jotai sivui mis meikä surffais
11. yhteensä 30.
12. yhteys voi olla rikki tai kyseessä voi olla jokin salattu asia.
13. -------
::                  49853
::                  49671
::                  49667
::                  49666
::                  49665
::                  49664
::1                 42050
::                   7680
::                   5357
::                    445
::                    135
0.0.0.0             64951
0.0.0.0             57621
127.0.0.1           51100
127.0.0.1           50100
0.0.0.0             49853
0.0.0.0             49671
0.0.0.0             49667
0.0.0.0             49666
0.0.0.0             49665
0.0.0.0             49664
127.0.0.1           27339
127.0.0.1           22112
127.0.0.1           13032
127.0.0.1           13031
127.0.0.1           13030
127.0.0.1            9014
127.0.0.1            9013
127.0.0.1            9012
127.0.0.1            8885
127.0.0.1            7768
127.0.0.1            6463
127.0.0.1            5354
0.0.0.0              5040
127.0.0.1            1043
127.0.0.1            1042
192.168.101.204       139
0.0.0.0               135

siinä kaikki portit wlh
14. portti 135 on joku microsoftin vibe koodattu softa ja portti 22 on ssh
15. laitos altistuu vähemmälle ku vois


# Network Profile — [Torsti]

## Identity
- IPv4 address: 192.101.2xx
- Subnet mask / CIDR: 255.255.255.0
- MAC address: 10-ff-e0-31-xx-xx
- Network address: 
- Broadcast address: ...

## Gateway and reachability
- Default gateway: ...
- Ping to gateway (avg): 0 ms
- Ping to 1.1.1.1 (avg): 3 ms

## DNS
- Configured DNS server(s): ...
- example.com resolves to: ...

## Path to the internet
- Hops to example.com: 30
- First hop:  2001-14ba-a18d-7900--1.rev.dnainternet.fi [2001:14ba:a18d:7900::1]/1ms

## Listening ports
| Port | Protocol | Interface (localhost / all) | Common use |
|------|----------|------------------------------|------------|
| ...  | ...      | ...                          | ...        |

## Reflection (150–200 words)
- What surprised you about your own network? netti on niin laaja asia etten oikein voi edes yllättyä mistään
- Which open port (if any) would you want to investigate or close? kaikki niistä
- Which command do you think you'll use most often, and why? varmaa pingailen kaikkee läpäl kosk se on kivaa


-KASPERI TALL-
17.8.2026
11.32pm

 
