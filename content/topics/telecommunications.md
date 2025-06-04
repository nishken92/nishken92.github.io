+++
date = '2025-05-28T22:29:55+05:30'
draft = false 
title = 'Network Generations'
+++

### Introduction

Telecom generations from 1G to 5G can be considered as different network architecture
 - 1G : Provided basic Voice call services
 - 2G : Based on GSM network. Provided voice call services SMS services and Data services are introduced. Both used circuit switching
 - 2.5G : This is a bridge stage between 2G and 3G. Data services used Packet switching
 - 3G : This is based on completely new network architecture, that is UMTS
 - 4G : Also called long term evolution. Both Voice and Data services are packet switched
 - 5G : Enhanced network than 4G LTE with low latency

### Standardizing Units

 Telecommunication industry standards are decided by two international entities
  1. International Telecommunications Union (ITU):
      This is an UN organization. Overall system definitions like what latency is allowed for each generation is decided by ITU
  2. Third Generation Partnership Project (3GPP):
      It is a global collaboration projects with multiple companies as stakeholders. This decides the capabilities of the networks

![alt text](/topics/test3.jpg)

### User Equipment
 user Equipments includes mobile phones, WiFi, laptops, IoT devices etc. Along with the evolution in network generations, it is important for the user devices are also to be evolved to cop up with the network advancement.

### Radio Access Network (RAN)

 Radio Access Network is a gateway between user equipement and Core network. Cell site is a part of RAN which has two type of antennas
  1. GSM Antenna
  2. Microwave Antenna

GSM antenna is a transreceiver of data with UE, while microwave antenna takes care of the data transmission with other antennas. A Cell site is also known as Telecom mast. At the bottom of each cell site, there will be a base station.
Base station consists of two components
 1. Radio Unit
 2. Base Band Unit

### Transmission Network

 Transmission from RAN to Core Network(CN) is called Transmission network. It is carried out through three modes of transmission
 1. Microwave Antenna
 2. Optical Fibers
 3. Satellite
 Each mode of transmission has it's own pros and cons. Mobile Network Operators(MNO) deides the mode of transimission and topology based on the terrestrial conditions.

### Core Network
 Core Network or CN in short is known as the brain of the Network. It can be depicted as a large data processing centre. Core Network connects the UE with PSTN or Internet based on the request. PSTN implies Public Switching Telephone Network. 
 
Some of the primary responsibility of CN are
 1. Performing user autherization to make sure only the authentic users are accessing the network
 2. To check if the user is sibscribed to the services which he / she requesting for
 3. Ensure the correct switching from source to destination

Core Network is devided into two planes functionaly.
 - Control Plane : Performs authetication and autherization
 - User Plane : Where actual data transfer happens

#### Control Plane

 Two systems works hand to hand perform the control plane's functionality
 - Mobility Management Entity(MME) - This takes care of user identity
 - Home Subscriber Server - Checks if the user is subscribed to the services he / she is requesing for

Spectrum : It is a band of Electromagnetic frequency which is used to transmit data. Spectrum is a limited resource, MNOs pays millions of dollars to but spectrum.

### 4G and 5G Core Networks

 4G provides low latency seamless service. 5G is more smatter than 4G LTE, which makes the data processing almost real time. 

#### 4G CN Architecture

![alt text](/topics/test4.jpg)

 - MME : Mobility Management Entity
 - HSS : Home Subscriber Server
 - SGW : Session Gateway
 - PGW : Packet Data Gateway
 - PCRF : Policy and Charging Rules Function

#### 5G Architecture

![alt test](/topics/test5.jpg)

 - AMF : Access and Mobility Function
 - AUSF : Authentication Server Function
 - UDM : Unified Data Management
 - PCF : Policy Control Function
 - SMF : Session Management Function
 - UPF : User Plane Function 
