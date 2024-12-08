# Network adapter

## WSL

In case WSL is been used, the MQTT address won't be available from external nodes in the network, but windows allows you to route external connection to any WSL with:

```netsh interface portproxy add v4tov4 listenaddress=0.0.0.0 listenport=1883 connectaddress=<WSL-IP> connectport=1883```

**ATENÇÃO:** A sequência `0.0.0.0` **não** é pra ser substituida pelo IP da máquina windows

To find each of the IPs you can do:

- Windows:
```ipconfig```

- WSL:
```ip addr```
(look for the eth connection)