# rasp-led-service
systemd service to switch off Raspberry LEDs on boot time 


# How to install

1.) Copy service file to systemd unit files:
```
sudo cp rasp-led-service.service /etc/systemd/system/
chmod 664 /etc/systemd/system/rasp-led-service.service
```

2.) Reload the demon

```
sudo systemctl daemon-reload
```

3.) Activate the service

```
sudo systemctl enable rasp-led-service.service
sudo systemctl start rasp-led-service.service
```
