# Network adapter

## WSL

In case WSL is been used, the MQTT address won't be available from external nodes in the network, but windows allows you to route external connection to any WSL with:

```netsh interface portproxy add v4tov4 listenaddress=<Host-IP> listenport=1883 connectaddress=<WSL-IP> connectport=1883```

To find each of the IPs you can do:

- Windows:
```ipconfig```

- WSL:
```ip addr```
(look for the eth connection)