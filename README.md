# ops-sat-swan (temporary name)

![](https://www.esa.int/var/esa/storage/images/esa_multimedia/images/2021/04/ops-sat_logo/23286333-1-eng-GB/Ops-Sat_logo.jpg)

A repository that contains links to various OPS-SAT projects being undertaken at Swansea University. It also contains links to useful information.

## Intro Talk
An intro talk on some of our ideas can be viewed here. [[here](https://www.youtube.com/watch?v=Buv8cqYmaug&t=728s)].

## The Swansea Flat-Sat

Our FlatSat is a development version of the OPS-SAT cube sat hosted in the Computational Foundry. Using this platform we can try to simulate the FPGA onboard OPS-SAT, the SDR, and the general linux environment onboard. The FlatSat currently consists of:

* A critical links MitySoM Cyclone V FPGA module (the same as onboard)
* A BladeRF SDR board. (Not the exact same device as onboard, but uses the same SDR chip.)
* A small LoRa ESP32 board -- for emulating terrestrial LoRa signals. 

## Connecting to the Swansea FlatSat

Currently the FlatSat is hosted in Shane's office, but we are looking for a better home for it. Once you have your account setup you can connect to the host machine via ssh. This has all the FlatSat hardware connected to it along with the tools that can be used to configure the FlatSat, such as Quartus for FPGA development.  

To SSH in you'll need to either be on the VPN or use the mutli-factor authentification (MFA) ssh gateway.

### Via the VPN

Connect to the Swansea University VPN using the _lovely_ PulseSecure software: https://vpn.swansea.ac.uk/

Once on the VPN you can then ssh into the FlatSat host with:

```
ssh <your OPSSAT username>@cs-s-fleming-pc.swan.ac.uk
```

You will specify your OPSSAT usename when you set up your account with one of the FlatSat sysadmins.

### Via the MFA ssh gateway

First ssh into the gateway server:

```
ssh <your university username>@iss-toran.swan.ac.uk -p 22995
```

This will require you to approve the login with your multifactor auth setup, such as via the phone app. Once you have connected to that server you can then ssh into the FlatSat host machine from the gateway machine.

```
ssh <your OPSSAT username>@cs-s-fleming-pc.swan.ac.uk
```

## OPS-SAT Technical Documentation
* [Official Payload Specification](https://ideas.esa.int/apps/IMT/UploadedFiles/00/f_d4aa96ccd0c7141ac4d10e072fb44d38/OPSSAT-SYS-PAY-ExperimenterICD_v0.5.pdf?v=1624349519)
* [Webpage detailing architecture](https://directory.eoportal.org/web/eoportal/satellite-missions/o/ops-sat)

## Other links
* [Flickr account containing OPS-SAT Images](https://www.flickr.com/photos/esa_events/albums/72157716491073681)
* [Where is OPS-SAT right now](https://www.n2yo.com/satellite/?s=44878)]
