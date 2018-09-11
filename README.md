# Raspberry Pi 3 setup

Download all files from repository folder ```pi``` on your computer to the SD
card (look for a drive named ```boot```).

On Windows run

```bat
copy pi\* E:\
```

On a Unix (like macOS) run

```sh
cp pi/* /Volumes/boot
```

# Connect via SSH

```sh
ssh pi@192.168.1.11
```

Password for the user ```pi``` is ```raspberry```.

# Connect via VNC

1. Enable VNC

	On the Raspberry Pi run

	```sh
	sudo raspi-config
	```

	and navigate to ```Interfacing Options``` and enable ```VNC```.

2. Install VNC client

	Download and install [RealVNC](https://www.realvnc.com/en/connect/download/vnc/) on your computer.

3. Connect to Raspberry Pi

	Open RealVNC and connect to ```192.168.1.11```.