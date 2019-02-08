# Blog
---
During Summer Studio B, we were tasked to work in correspondence to agile project methodology. This means we divided our work into the concept of 'sprints'.

In these sections, I will reflect on my experience throughout each sprint and attach some artifacts as evidence to my learnings.

## Sprint 1
I built an [IoT Data Logger](http://iot.nortcele.win/doc/index.html), components and schematics provided by courtesy of the studio's tutor, Danon. We were introduced to some of the IoT technologies we will be working with. These included a WiFi microcontroller unit, [ESP8266](https://arduino-esp8266.readthedocs.io/en/latest/index.html), and a piece of software called Blynk. I am working on a project with another person, Callum. We are addressing the maintenance of small potted plants through the use of IoTs. Our current concept is a soil moisture sensor that is remote, and can initiate a watering procedure should the soil moisture reach below a certain threshold.

I have built this portfolio this week. The repository is accessible through the artifacts in this entry. The portfolio is a website using [Vuepress](https://vuepress.vuejs.org), and is deployed using the CI/CDN service known as [Netlify](https://netlify.com). I have linked the site to domain registered by our tutor https://summerstudio.xyz. This portfolio currently resides on the subdomain <https://sebastian.summerstudio.xyz> (which is this site!).

I explored a communication protocol used in IoT devices called [MQTT](http://mqtt.org/) (MQ Telemetry Transport). Without getting into the specifics, MQTT allows machines to communicate with one another in real-time. It requires a 'broker' server to handle the communication between clients. I have developed an MQTT broker locally and am intending on deploying it in the cloud for machines to access via. the internet. Our tutor, Danon, has some online compute instances available for us to use in the case we want to host anything on the cloud. It is attached to an infrastructure-as-a-service called [Vultr](https://www.vultr.com). The repository for it is in the artifacts for this sprint. I will learn more about Docker so that I can containerise future deployments of the server, rather than setting up virtual machines manually to host my code.

For the next sprint, I'm going to try and bootload the ESP mcu with some custom firmware that uses the MQTT protocol, and point it towards the MQTT broker I will deploy.

#### Artifacts
> Portfolio <https://github.com/sguillema/ssb19_iot_portfolio/tree/sebastian>

> Backend Repo - MQTT Broker <https://github.com/sguillema/ssb19_iot_be>

<!-- ## Sprint 2

#### Artifacts

## Sprint 3

#### Artifacts

## Sprint 4

#### Artifacts -->