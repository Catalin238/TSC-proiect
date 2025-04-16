# TSC-proiect

1. Diagrama Bloc

![image](https://github.com/user-attachments/assets/a9e8e494-4cfa-4854-8f94-42a557fe4d2d)

2. Bill of materials


| Piece Name | Quantity | Link |
|------------|----------|------|
| ESP32 | 1 | https://www.snapeda.com/parts/ESP32-C6-WROOM-1-N8/Espressif%20Systems/view-part/?ref=search&t=ESP32-C6-WROOM-1-N8 |
| BME680 | 1 | https://www.snapeda.com/parts/BME680/Bosch%20Sensortec/view-part/?ref=search&t=bme680 |
| DS3231SN | 1 | https://www.snapeda.com/parts/DS3231SN%23/Analog%20Devices/view-part/?ref=search&t=DS3231SN%23 |
| W25Q512JVEIQ | 1 | https://www.snapeda.com/parts/W25Q512JVEIQ/Winbond%20Electronics/view-part/?ref=search&t=W25Q512JVEIQ |
| MCP73831 | 1 | https://componentsearchengine.com/part-view/MCP73831T-2ACI%2FOT/Microchip |
| MOSFET | 1 | https://componentsearchengine.com/part-view/DMG2305UX-7/Diodes%20Incorporated |
| SAMACSYS_PARTS_USB4110-GF-A | 1 | https://www.snapeda.com/parts/USB4110-GF-A./Global%20Connector%20Technology/view-part/ |
| USBLC6-2SC6Y | 1 | https://www.snapeda.com/parts/USBLC6-2SC6Y/STMicroelectronics/view-part/?ref=dk&t=USBLC6-2SC6Y&con_ref=None |
| BD5229G-TR | 1 | https://www.snapeda.com/parts/BD5229G-TR/Rohm/view-part/?ref=search&t=BD5229G-TR |
| QWIIC_CONNECTOR | 1 | https://www.snapeda.com/parts/PRT-14417/SparkFun/view-part/ |
| CPH3225A | 1 | https://www.snapeda.com/parts/CPH3225A/Seiko/view-part/ |
| BUTTON_CUSYOMV1 | 3 | https://www.snapeda.com/search/?q=EVQP7L01P&search-type=parts |
| ADAFRUIT_LEDCHIP-LED0603 | 1 | https://www.snapeda.com/parts/KP-1608SURCK/Kingbright/view-part/?ref=search&t=LED%200603 |
| C0402 | 1 | https://componentsearchengine.com/part-view/CC0402MRX5R5BB106/YAGEO |
| 112ATAARR03 | 1 | https://www.snapeda.com/parts/112A-TAAR-R03/Attend/view-part/ |
| 744043680 | 1 | https://eu.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D |
| R0402 | 1 | https://componentsearchengine.com/part-view/R0402%201%25%20100%20K%20(RC0402FR-07100KL)/YAGEO |
| SD0805S020S1R0 | 1 | https://componentsearchengine.com/part-view/SD0805S020S1R0/Kyocera%20AVX |
| VARISTOR | 1 | https://ro.mouser.com/ProductDetail/EPCOS-TDK/B72520T0350K062?qs=dEfas%2FXlABIszF52uu7vrg%3D%3D |
| SRJ | 1 | https://componentsearchengine.com/part-view/FH34SRJ-24S-0.5SH(99)/Hirose |
| MBR0530 | 1 | https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/ |
| PGB1010603MR | 1 | https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/ |
| RCL_CPOL-EU | 1 | https://grabcad.com/library/tantalum-smd-capacitor-type-b-3528-1 |
| SI1308EDL-T1-GE3 | 1 | https://www.snapeda.com/parts/SI1308EDL-T1-GE3/Vishay/view-part/ |
| XC6220A331MR-G | 1 | https://ro.mouser.com/ProductDetail/Torex-Semiconductor/XC6220A331MR-G?qs=AsjdqWjXhJ8ZSWznL1J0gg%3D%3D&utm_source=octopart&utm_medium=aggregator&utm_campaign=865-XC6220A331MR-G&utm_content=Torex%20Semiconductor |


3. Functionalitati Hardware

Structura si Functionalitati:

ESP32-C6-WROOM-1-N8
Functie: Procesor central al sistemului, gestioneaza protocoalele de comunicare (SPI, I2C, UART), achizitia datelor de la senzori si controlul dispozitivelor periferice.

Connector USB-C cu Protectie ESD
Functie: Ofera posibilitatea incarcarii prin port USB-C si implementeaza circuite de protectie impotriva descarcarilor electrostatice.

Controller de Incarcare (MCP73831)
Functie: Administreaza procesul de incarcare pentru acumulatorul Li-Po si regleaza parametrii curentului de incarcare.

Acumulator Li-Po
Functie: Furnizeaza energie autonoma, permitand functionarea dispozitivului independent de conexiunea USB.

Regulator de Tensiune LDO
Functie: Converteste si mentine o tensiune stabila de 3.3V pentru alimentarea microcontrolerului si a componentelor auxiliare.

Memorie Flash NOR Externa 64MB
Functie: Asigura spatiu de stocare aditional pentru date operationale si actualizari de firmware.

Modul RTC (DS3231SN)
Functie: Asigura cronometrarea precisa si mentinerea datei/orei curente.
Conectivitate: Protocol I2C, include functii de alarma si baterie de rezerva pentru mentinerea timpului.

Senzor de Mediu (BME688)
Functie: Colecteaza parametri ambientali precum temperatura, umiditatea, presiunea atmosferica si compusi organici volatili.
Conectivitate: Comunicare I2C, optimizat pentru consum redus in standby, cu capacitati avansate de detectare a gazelor.
Implementare: Utilizeaza interfata standardizata Qwiic / Stemma QT pentru conectare plug-and-play.

Circuit de Control pentru Afisaj E-Paper si Conector
Functie: Produce semnalele specifice pentru operarea afisajelor electroforetice si faciliteaza compatibilitatea cu diferite tipuri de ecrane.
Conectivitate: Protocol SPI, cu linii dedicate pentru control (Busy, Reset, DC, CS).

Card SD
Functie: Faciliteaza stocarea extinsa a datelor, fisierelor de configurare si inregistrarilor pe termen lung.
Conectivitate: Interfata SPI cu linie dedicata de selectie.

Supervisor de Tensiune si Butoane Reset/Boot
Functie: Supravegheaza nivelul tensiunii de alimentare si controleaza secventele de initializare si repornire ale ESP32-C6.

Interfete si Protocoale de Comunicare:

I2C: Implementat pentru comunicarea cu BME688 si DS3231SN.
SPI: Utilizat pentru accesarea memoriei Flash NOR, controlul afisajului E-Paper si operatiunile cu cardul SD.
UART: Disponibil pentru debugging si integrarea modulelor externe optionale.
Wi-Fi si Bluetooth LE: Functionalitati native ale ESP32-C6.

Analiza Consumului Energetic:

ESP32-C6:
Consum in regim activ: ~80-240 mA (variabil in functie de activitatea Wi-Fi/BT).
Consum in regim economic: sub 1 mA (in modul deep sleep).


BME688:
Consum caracteristic: ~2.1 µA in repaus, maxim ~3.1 mA in operare completa.


Memorie Flash NOR:
Consum la citire/scriere: 5-15 mA, in asteptare: sub 10 µA.


DS3231SN:
Consum constant: aproximativ 150 µA cu functia de backup activa.


Regulator LDO:
Randamentul energetic variaza in functie de diferenta dintre tensiunea de intrare si cea de iesire (3.3V) si de curentul total solicitat.


4. Pini ESP32-C6


| Pin ESP32-C6  | Componenta / Rol                       | Descriere                             |
|---------------|---------------------------------------|---------------------------------------|
| IO8 (SCK)     | SPI Clock                             | Semnal de clock SPI                   |
| IO6 (MOSI)    | SPI MOSI catre NOR Flash, E-Paper, SD Card | Transfer date catre periferice SPI   |
| IO7 (MISO)    | SPI MISO din NOR Flash, E-Paper, SD Card | Receptie date de la periferice SPI |
| IO9 (CS1)     | Chip Select NOR Flash                 | Control dedicat pentru NOR Flash      |
| IO11 (CS3)    | Chip Select SD Card                   | Control dedicat pentru SD Card        |
| IO10 (CS2)    | Chip Select E-Paper Display           | Control dedicat pentru Display        |
| IO15 (SCL)    | I2C SCL catre BME688 si DS3231SN      | Semnal de clock I2C                   |
| IO14 (SDA)    | I2C SDA catre BME688 si DS3231SN      | Date pentru I2C         |
| IO21          | Reset/Boot control                    | Butoane de reset si boot              |
| IO16, IO17    | UART RX, TX (debug)                   | Debug serial si configurare           |

