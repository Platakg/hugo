+++
title = "Bytes to String"
date = "2019-04-26"
description = "There's a difference"
draft = false
+++

<img src="/images/sunflowers.jpg" alt="hello-hugo photo" style="width:642px;height:442px;"> 


I was reminded of this once-murky concept while using the requests module of python.

Using: <br>
    
    r = requests.get(url, param)
	
    payload = r.context		# <--returns bytes    '*' Bytes are (UTF-8)
    payload = r.text 		# <--returns string

From here I needed to parse out my response for which I used the json module to load my bytes response to a list and then dump to familiar json format.


Helpful StackExchange:
https://stackoverflow.com/questions/40059654/python-convert-a-bytes-array-into-json-format
