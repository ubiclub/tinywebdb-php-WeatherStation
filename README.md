# tinywebdb-php
a textfile based TinyWebDB implement. not any db required.

TinyWebDB Protocol:  

|    Action        |URL                      |Post Parameters  |Response                          |
|------------------|-------------------------|-----------------|----------------------------------|
|    Get Value     |{ServiceURL}/getvalue    |tag              |JSON: ["VALUE","{tag}", {value}]  |
|    Store A Value |{ServiceURL}/storeavalue |tag,value        |JSON: ["STORED", "{tag}", {value}]|

Fertures:
- TinyWebDB API 
    - handle storevalue request, then save to a textfile. 
    - handle getvalue request and return content from the textfile. 
- Test Form: 
    - send storevalue request 
    - send getvalue request 
- Tag View
    - List all tags
    - The tags link to getvalue API
- Log tail viewer 
    - Daily log file 
    - last 20 lines view 

Test site URL :
- http://sensor.digilib.org/
