# iCurb - intelligent Curb

Award nominated construction of a smart parking detection and activation system for electric cars. Disclaimer: The work is based upon patent DE102010046263A1 and the development has been assisted by following people. The curbs has been provided by MEA Water Management GmbH.

The purpose of the project is to describe two tasks:

* eFind ( Find and Charge ) : how a user can reserve a parking spot and get authenticated automatically when he reaches the parking spot.
* iCurb: the methods to install an iCurb at events and in parking garages.

```
1. Driving the LEDs using Chromoflex , [Oemer Kayar; Vikas Agrawal]
2. Choosing the right sensor network protocol, [Niharika Ramachandramurthy; Vikas Agrawal]
3. Mecahnical design of the iCurb: [Daniel Borrmann, Lieselotte Ade, Vikas Agrawal]
4. Magnetic Sensor tests with Waspmote: [ Leander John, Vikas Agrawal]
5. Driving a charging unit over the bluetooth: [Julio Rodriguez, Andreas Sauter, Vikas Agrawal]

```

Sensor Box consisting of

* Parking detection and LED controller module
* Relay module to start / stop charging unit and authentication module using bluetooth
* Zigbee module to communicate with a gateway
* Smart Phone App to request starting and stopping the charging unit.

Parking detection and LED controller module

<figure><img src=".gitbook/assets/icurb/die_sensorik_und_led_mit_bordstein.jpg" alt=""><figcaption></figcaption></figure>

Relay module to start / stop charging unit and authentication module using bluetooth

<figure><img src=".gitbook/assets/icurb/authentifizierung.jpg" alt=""><figcaption></figcaption></figure>

Zigbee module to communicate with a gateway

<figure><img src=".gitbook/assets/icurb/kommunikations_technik_icurb.jpg" alt=""><figcaption></figcaption></figure>

Smart Phone App to request starting and stopping the charging unit.

<figure><img src=".gitbook/assets/icurb/smart_phone_app_icurb_zu_bedienen.jpg" alt=""><figcaption></figcaption></figure>

The prototype involves a

* A Smart Phone app
  * to interact with the bluetooth module integrated in the infrastructure.
  * to query the parking garages and get the available parking spots for the electric vehicles
* A On Board Unit integrated in the car
  * with a bluetooth module to interact with the bluetooth module integrated in the infrastructure
  * that can query the parking garages to get the available parking spots for the electric vehicles.
* A LED Module embedded in the charging unit
  * To display the current situation of the parking spot.
  * RED indicates the parking spot is already reserved.
  * GREEN indicates the parking spot is not reserved and can be occupied.
  * BLUE indicates an ongoing authentication is taking place as the car reaches the parking spot.
  * BREATHING RED indicates that the CAR is being charged.
* Bluetooth Module embedded in the charging unit
  * To authenticate an incoming user with his Bluetooth MAC Address.
  * To be able to get the status of the charging unit over the bluetooth communication.
* Magnetic sensor embedded in the charging unit ◦
  * To be able to detect the presence of the car in the vicinity.
* Relay to start the charging process after a successful authentication.
* Zigbee communication module
  * The zigbee communication module interacts with the parking garage server and sends data of the occupancy of the parking spots.
  * Kommunikation zwischen verschiedenen iCurbs

Wie man hier sieht, einzelen icurb kommunizieren mit einanderen und übermitteln Ihre aktuelle Status ( Energie, Parkplatzbelegung etc. )

<figure><img src=".gitbook/assets/icurb/icurb_kommunizieren_mit_einanderen.jpg" alt=""><figcaption></figcaption></figure>

***

Prototype for the charging unit.

<figure><img src=".gitbook/assets/icurb/iCurb_Uebersicht_gerendert.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/icurb/iCurb_Elektrik-Gehaeuse_gerendert.png" alt=""><figcaption></figcaption></figure>

The prototype of the charging unit involves • Upper part of the curb ◦ contains the slot for the LED ◦ contains the method to lock the upper part with the lower part of the curb. ◦ contains the possibility to mount the box containing the electrical parts. • Lower part of the curb ◦ Contains the high voltage wires to charge the cars. ◦ Contains a hole to connect the socket with the incoming wires.

3 Areas of application:

```
    3.1 Events, Parking garages, On Street
```

The iCurb has a potential to provide robust channels to provide the required infrastructure of charging units. The projects can be applied 1. during the organization of big events with adhoc requirement of charging units. 2. Integrate the curbs already during the construction of new parking garages.

Einfache Installation bei Veranstaltungen: Skizze für die Installation des iCurbs bei Veranstaltungen. Man sieht ganz rechts eine Gateway

<figure><img src=".gitbook/assets/icurb/Overview.JPG" alt=""><figcaption><p>Electric charging station</p></figcaption></figure>

<figure><img src=".gitbook/assets/icurb/Overview_blur1.jpg" alt=""><figcaption><p>Blue labels denote embedded electronic units </p></figcaption></figure>

<figure><img src=".gitbook/assets/icurb/Overview_blur2_desc.jpg" alt=""><figcaption><p>Red dotted line denotes communication with the charging unit</p></figcaption></figure>

IKT for finding and reserving a parking place from a smart phone or an OBU: Ein Button in Autoradio iCurbs zu finden ( mögliche Industrieprojekt )

<figure><img src=".gitbook/assets/icurb/ikt_auto_radio.jpg" alt=""><figcaption></figcaption></figure>

Das Smart Auto lädt über iCurb

<figure><img src=".gitbook/assets/icurb/smart_laden_ueber_icurb.jpg" alt=""><figcaption></figcaption></figure>

LED Laufschrift um zu erkennen wie viele Parkplätze noch frei sind:

<figure><img src=".gitbook/assets/icurb/ledlaufschrit.JPG" alt=""><figcaption></figcaption></figure>

