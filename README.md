# IoT NodeRed project

As part of the DAS410103 - _Conceitos Básicos de IoT e de Sistemas Distribuídos_ course at UFSC (20242)

## Running the constainer

To build the image from the Dockerfile:

```docker build -t iot-node-red ./node-red/```

To run the image:

```docker run -it -p 1880:1880 -p 1883:1883 --rm -v ./node-red:/data --name node-red-container iot-node-red```