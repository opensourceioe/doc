---
weight: 10
title: API Reference
---
# Application Details

>![This is an image](/images/main.png)

> APPLICATION: https://openioe.in

> ENDPOINT: https://us-central1-smartapp-iot.cloudfunctions.net/api/

![This is an image](/images/logo.png)


***Open IoE is Open source Internet of Things platform.*** The application is hosted at ***[https://openioe.in](https://openioe.in/)***





# Getting Started

## Quick Start

>![This is an image](/images/dash.png)

> To communicate with Open IoE, use this code:

```matlab
url = 'https://us-central1-smartapp-iot.cloudfunctions.net/api/';
options = weboptions('ContentType','text');
api=strcat(url,'read/<APIKey>/<DeviceID>/<DevicePIN>')
value = webread(url,options)
```


```python
#Pip install requests
import requests
url=https://us-central1-smartapp-iot.cloudfunctions.net/api/
api=url+"read/<APIKey>/<DeviceID>/<DevicePIN>"
response = requests.get(api)
print response.text
```

1. Application Level

	a. Login to [https://openioe.in/login](https://openioe.in/login)
	
	b. Create and select Project
	
	c. Create and select Device: Note down device id and pin
	
	d. Create and select API Key: Note down API Key
	
	e. Create default data
	
2. Device Level

	a. Connect to application
	
	b. Send and recieve data

## Detailed Procedure

Comming soon...

# Applications

## Ohms law in Electrical system




> V=IR

Problem: Find R if I and V are sensed using Raspberry Pi SBC via sensors.

R=V/I;

`Assumptions: DC circuit`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>
