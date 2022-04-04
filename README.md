# DN3000ATX
Apollo DN3000 ATX Power Supply adaptor. Use at your own risk

![image](https://user-images.githubusercontent.com/24400566/161471010-ecb330ee-9b76-4635-b812-2b97119ffbe3.png)
![image](https://user-images.githubusercontent.com/24400566/161471025-c6857aa9-3000-424d-b61b-e27cf80d2e00.png)


BoM:
1X ROHM BA17809FP-E2;
1X MC7905ACD2;
1X MIC5270-4.1YM5;
4X 10uF, 25V 1210 MLCC caps, X5R;
1X 20 position MiniFit male header (what you stab the ATX PSU cable into);
Random wire with appropriate terminating connectors for the Apollo board (KK396 for P12, random .100" DuPont thing for P13)

Extant online documentation is rather vague and I can only guess what's supposed to be on P13 - it is fed +3.3V straight from the ATX header, and -4.1V down-regulated via an LDO from -5V, which in turn is derived from -12V. ATX -5V is left unconnected on the header and only generated on-board, since most PSUs (all modern ones) no longer have it.

At the time of writing, OSHPark of Portland, OR (recommended) charges $17.20 for making 3 boards out of these Gerbers, $34/10pcs if using the Medium Run service.
