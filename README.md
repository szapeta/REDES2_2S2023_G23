# REDES2_2S2023_G23
## Configuración de Switches

### SW1A_G5B


SW1A_G5B
SW2A_G5B
SW3A_G5B
SW4A_G5B
SW5A_G5B
SW6A_G5B
SW7A_G5B
SW8A_G5B
SW9A_G5B
SW10A_G5B
SW11A_G5B
SW12A_G5B

#CONFIGURACION VTP (PIRAMIDE IZQ)
## ---------SW1A_G5B----------------
```bash

SWITCH# hostname SW1A_G5B
SW1A_G5B# vtp domain g5
SW1A_G5B# vtp password seguro
SW1A_G5B# vtp mode server
SW1A_G5B# exit
copy running-config startup-config
SW1A_G5B# interface range fastEthernet 0/1 – 5
SW1A_G5B# switchport mode trunk
SW1A_G5B# exit
copy running-config startup-config
SW1A_G5B# show vlan brief
SW1A_G5B# vlan 15
SW1A_G5B# name Primaria
SW1A_G5B# vlan 25
SW1A_G5B# name Basicos
SW1A_G5B# vlan 35
SW1A_G5B# name Diversificado
SW1A_G5B# show vlan brief
copy running-config startup-config

```
## ---------SW2A_G5B----------------
```bash
SWITCH# hostname SW2A_G5B
SW2A_G5B# vtp domain g5
SW2A_G5B# vtp password seguro
SW2A_G5B# vtp mode server
copy running-config startup-config
SW2A_G5B# interface range fastEthernet 0/1 – 5
SW2A_G5B# switchport mode trunk
SW2A_G5B# exit
copy running-config startup-config
SW2A_G5B# show vlan brief
SW2A_G5B# vlan 15
SW2A_G5B# name Primaria
SW2A_G5B# vlan 25
SW2A_G5B# name Basicos
SW2A_G5B# vlan 35
SW2A_G5B# name Diversificado
SW2A_G5B# show vlan brief
copy running-config startup-config
```
## ---------SW3A_G5B----------------
```bash
SWITCH# hostname SW3A_G5B
SW3A_G5B# vtp domain g5
SW3A_G5B# vtp password seguro
SW3A_G5B# vtp mode server
copy running-config startup-config
SW3A_G5B# interface range fastEthernet 0/1 – 5
SW3A_G5B# switchport mode trunk
SW3A_G5B# exit
copy running-config startup-config
SW3A_G5B# show vlan brief
SW3A_G5B# vlan 15
SW3A_G5B# name Primaria
SW3A_G5B# vlan 25
SW3A_G5B# name Basicos
SW3A_G5B# vlan 35
SW3A_G5B# name Diversificado
SW3A_G5B# show vlan brief
copy running-config startup-config
```
## ---------SW4A_G5B----------------
```bash
SWITCH# hostname SW4A_G5B
SW4A_G5B# vtp domain g5
SW4A_G5B# vtp password seguro
SW4A_G5B# vtp mode client
copy running-config startup-config
SW4A_G5B# interface range fastEthernet 0/1 – 2
SW4A_G5B# switchport mode trunk
SW4A_G5B# exit
SW4A_G5B# interface range fastEthernet 0/3 – 24
SW4A_G5B# switchport mode access
SW4A_G5B# exit
copy running-config startup-config
SW4A_G5B# interface range fastEthernet 0/11 – 12
SW4A_G5B# switchport access vlan 15
SW4A_G5B# exit
copy running-config startup-config

```
## ---------SW5A_G5B----------------
```bash
SWITCH# hostname SW5A_G5B
SW5A_G5B# vtp domain g5
SW5A_G5B# vtp password seguro
SW5A_G5B# vtp mode client
copy running-config startup-config
SW5A_G5B# interface range fastEthernet 0/1 – 2
SW5A_G5B# switchport mode trunk
SW5A_G5B# exit
SW5A_G5B# interface range fastEthernet 0/3 – 24
SW5A_G5B# switchport mode access
SW5A_G5B# exit
copy running-config startup-config
SW5A_G5B# interface range fastEthernet 0/11 – 12
SW5A_G5B# switchport access vlan 25
SW5A_G5B# exit
copy running-config startup-config
```
## ---------SW6A_G5B----------------
```bash
SWITCH# hostname SW6A_G5B
SW6A_G5B# vtp domain g5
SW6A_G5B# vtp password seguro
SW6A_G5B# vtp mode client
copy running-config startup-config
SW6A_G5B# interface range fastEthernet 0/1 – 2
SW6A_G5B# switchport mode trunk
SW6A_G5B# exit
SW6A_G5B# interface range fastEthernet 0/3 – 24
SW6A_G5B# switchport mode access
SW6A_G5B# exit
copy running-config startup-config
SW6A_G5B# interface range fastEthernet 0/11 – 12
SW6A_G5B# switchport access vlan 35
SW6A_G5B# exit
copy running-config startup-config

```
## ---------SW7A_G5B----------------
```bash
#CONFIGURACION VTP (PIRAMIDE DER)
SWITCH# hostname SW7A_G5B
SW7A_G5B# vtp domain g5
SW7A_G5B# vtp password seguro
SW7A_G5B# vtp mode server
copy running-config startup-config
SW7A_G5B# interface range fastEthernet 0/1 – 5
SW7A_G5B# switchport mode trunk
SW7A_G5B# exit
copy running-config startup-config
```
## ---------SW8A_G5B----------------
```bash
SWITCH# hostname SW8A_G5B
SW8A_G5B# vtp domain g5
SW8A_G5B# vtp password seguro
SW8A_G5B# vtp mode server
copy running-config startup-config
SW8A_G5B# interface range fastEthernet 0/1 – 5
SW8A_G5B# switchport mode trunk
SW8A_G5B# exit
copy running-config startup-config
```
## ---------SW9A_G5B----------------
```bash
SWITCH# hostname SW9A_G5B
SW9A_G5B# vtp domain g5
SW9A_G5B# vtp password seguro
SW9A_G5B# vtp mode server
copy running-config startup-config
SW9A_G5B# interface range fastEthernet 0/1 – 5
SW9A_G5B# switchport mode trunk
SW9A_G5B# exit
copy running-config startup-config

```
## ---------SW10A_G5B----------------
```bash
SWITCH# hostname SW10A_G5B
SW10A_G5B# vtp domain g5
SW10A_G5B# vtp password seguro
SW10A_G5B# vtp mode client
copy running-config startup-config
SW10A_G5B# interface range fastEthernet 0/1 – 2
SW10A_G5B# switchport mode trunk
SW10A_G5B# exit
SW10A_G5B# interface range fastEthernet 0/3 – 24
SW10A_G5B# switchport mode access
SW10A_G5B# exit
copy running-config startup-config
SW4A_G5B# interface range fastEthernet 0/11 – 12
SW4A_G5B# switchport access vlan 35
SW4A_G5B# exit
copy running-config startup-config

```
## ---------SW11A_G5B----------------
```bash
SWITCH# hostname SW11A_G5B
SW11A_G5B# vtp domain g5
SW11A_G5B# vtp password seguro
SW11A_G5B# vtp mode cliente
copy running-config startup-config
SW11A_G5B# interface range fastEthernet 0/1 – 2
SW11A_G5B# switchport mode trunk
SW11A_G5B# exit
SW11A_G5B# interface range fastEthernet 0/3 – 24
SW11A_G5B# switchport mode access
SW11A_G5B# exit
copy running-config startup-config
SW4A_G5B# interface range fastEthernet 0/11 – 12
SW4A_G5B# switchport access vlan 25
SW4A_G5B# exit
copy running-config startup-config

```
## ---------SW12A_G5B----------------
```bash
SWITCH# hostname SW12A_G5B
SW12A_G5B# vtp domain g5
SW12A_G5B# vtp password seguro
SW12A_G5B# vtp mode client
copy running-config startup-config
SW12A_G5B# interface range fastEthernet 0/1 – 2
SW12A_G5B# switchport mode trunk
SW12A_G5B# exit
SW12A_G5B# interface range fastEthernet 0/3 – 24
SW12A_G5B# switchport mode access
SW12A_G5B# exit
copy running-config startup-config
SW4A_G5B# interface range fastEthernet 0/11 – 12
SW4A_G5B# switchport access vlan 15
SW4A_G5B# exit
copy running-config startup-config
```
