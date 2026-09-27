osa 1

1.1 

Decimal	Binary
10	00001010
210	11010010
168	10101000
16	00010000
255	11111111
128	10000000
192	11000000
248	11111000
0	00000000
1.2 

Binary	Decimal
11000000	192
11111111	255
10101000	168
00010000	16
11111000	248
11010010	210

1.3

full ip conversion
10.210.168.16

00001010.11010010.10101000.00010000

192.168.0.1

11000000.10101000.00000000.00000001

172.16.5.100

10101100.00010000.00000101.01100100

reverse conversion
11000000.10101000.00000001.00000001

192.168.1.1

00001010.00001010.00000000.01001011

10.10.0.75

osa 2

2.1
Address		Class		Default mask		CIDR
10.0.0.5	A		255.0.0.0		/8
192.168.1.1	C		255.255.255.0		/24
172.16.4.20	B		255.255.0.0		/16
8.8.8.8		A		255.0.0.0		/8
200.100.50.25	C		255.255.255.0		/24

2.2
Dotted-decimal		CIDR		Binary
255.255.255.0		/24		11111111.11111111.11111111.00000000
255.255.0.0		/16		11111111.11111111.00000000.00000000
255.0.0.0		/8		11111111.00000000.00000000.00000000
255.255.255.192		/26		11111111.11111111.11111111.11000000
255.255.248.0		/21		11111111.11111111.11111000.00000000
255.255.255.128		/25		11111111.11111111.11111111.10000000

2.3
Class	Default CIDR	Number of possible networks	Number of hosts per network
A	/8		128 nets			16,777,214 usable hosts
B	/16		16,384 nets			65,534 usable hosts
C	/24		2,097,152 nets			254 usable hosts

osa 3

3.1

172.16.0.0/16
Subnet mask: 255.255.0.0

Network address: 172.16.0.0

Default gateway: 172.16.0.1

Host range start: 172.16.0.2

Host range end: 172.16.255.254

Broadcast: 172.16.255.255

3.2

10.10.0.0/26
Subnt mask: 255.255.255.192

Network address: 10.10.0.0

Default gateway: 10.10.0.1

Host rrange start: 10.10.0.2

Host range end: 10.10.0.62

Broadcast: 10.10.0.63

3.3

192.168.5.0/28
Subnet mask: 255.255.255.240

Network address: 192.168.5.0

Default gateway: 192.168.5.1

Host range start: 192.168.5.2

Host range end: 192.168.5.14

Broadcast: 192.168.5.15

3.4

10.0.0.0/30
Subnet mask: 255.255.255.252

Network address: 10.0.0.0

Default gateway: 10.0.0.1

Host range start: 10.0.0.2

Host range end: 10.0.0.2

Broadcast: 10.0.0.3

3.5

192.168.100.128/25
Subnet mask: 255.255.255.128

Network address: 192.168.100.128

Default gateway: 192.168.100.129

Host range start: 192.168.100.130

Host range end: 192.168.100.254

Broadcast: 192.168.100.255


osa 4

4.1

10.10.0.75/26
A /26 has blocks of 64:

0–63

64–127

128–191

192–255

75 is in the 64–127 block

Network address: 10.10.0.64

Broadcast: 10.10.0.127

Valid host? kyllä

miksi? 75 ei ole kumpikaan network addresseista (64) eikä broadcasteista (127).

4.1

192.168.1.200/26
/26 blocks are 0–63, 64–127, 128–191, and 192–255.

Network address: 192.168.1.192

Broadcast: 192.168.1.255

Valid host? Yes.

200 is between 193 and 254 so it is a usble host address.

4.3

172.16.5.130/25
A /25 has blocks of 128:

0–127

128–255

jonka takia:

Network address: 172.16.5.128

Broadcast: 172.16.5.255

Valid host? jeps.

130 is between 129 and 254.

4.4

10.0.0.0/30
A /30 sisältää:

Network: 0

Usable hosts: 1, 2

Broadcast: 3

joten:

Network address: 10.0.0.0

Broadcast: 10.0.0.3

Valid host? naaaaah.

se on network address eikä host address.

osa 5

5.1 

neljä samaa /26 subnettiä
A /24 sisältää 256 addresses. A /26 sisältää 64 joten:

256 ÷ 64 = 4 subnets

Subnet 1 — 192.168.10.0/26
Network: 192.168.10.0

Gateway: 192.168.10.1

Host range: 192.168.10.2 – 192.168.10.62

Broadcast: 192.168.10.63

Subnet 2 — 192.168.10.64/26
Network: 192.168.10.64

Gateway: 192.168.10.65

Host range: 192.168.10.66 – 192.168.10.126

Broadcast: 192.168.10.127

Subnet 3 — 192.168.10.128/26
Network: 192.168.10.128

Gateway: 192.168.10.129

Host range: 192.168.10.130 – 192.168.10.190

Broadcast: 192.168.10.191

Subnet 4 — 192.168.10.192/26
Network: 192.168.10.192

Gateway: 192.168.10.193

Host range: 192.168.10.194 – 192.168.10.254

Broadcast: 192.168.10.25

5.2

Enough hosts?

CIDR		Total addresses		Usable hosts
/24		256			254
/25		128			126
/26		64			62
/27		32			30
/28		16			14
/29		8			6
/30		4			2

osa 6

6.1

Hex ↔ decimal ↔ binary

Hex		Decimal		Binary
0		0		0000
5		5		0101
a		10		1010
f		15		1111

6.2

Compress the ipv6 addresses

1.
alkuperäinen:

2001:0df8:23f2:0000:0000:0000:0000:0f11

tiivistetty:

2001:df8:23f2::f11

2.
alkuperäinen:

2001:0000:00d0:00f2:0000:0000:0000:0f11

tiivistetty

2001:0:d0:f2::f11

3.
alkuperäinen
fe80:0000:0000:0000:0000:0000:0000:0001

tiivistetty:

fe80::1

6.3 

WHy do we need ipv6

ipv6 tarvitaan, koska laitteiden määrä on vuosien aikana kasvanut niin paljon, että perus ipv4 osoitteet eivät pysty tukemaan niitä kaikkia. Ipv6 tarjoaa suuremman osoitetilan, peräti 128 bittisen, jolla voidaan teoreettisesti yhdistää (googlen mukaan) 340 undeciljoonaa (2^128) laitetta nettiin.

	


