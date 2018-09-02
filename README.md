## RpiWebControl

A simple HTTP remote control project for Raspberry Pi using array-gpio, express and angular.

Turn ON/OFF the actuators/peripherals connected to your Raspberry Pi using your mobile device.

![](https://github.com/EdoLabWorks/ximgs/blob/master/raspberry-remote1.png)

### Raspberry Pi Pin Setup

Using the GPIO physical pin number, choose the pins you want to use as outputs.

Configure the pins in the app.js file as shown below.

For this project, you only need to provide the output pins you will use.

~~~~
gpio.setOutput(pin1, pin2 ... pin4); // max. 4 outputs
~~~~

### Features

- Real-time update of GPIO pin state.
- Control remote devices from within your private network using your mobile device browser.  

### Installation 

Git clone or download the application from your Raspberry Pi.
```console
$ git clone https://github.com/EdAlegrid/PiWebControl.git
```

In the root folder, install all dependencies.
```console
$ cd PiWebControl
$ npm install
```

Run the application as shown below. 
```console
$ node app
```

You will see the details of your Raspberry Pi local web server.
```console
$ node app
*** http server ***
HttpServer started: http://192.168.1.125:3000
```

Open a web browser and enter your web server details.
```console
http://192.168.1.125:3000
```

### License

MIT
