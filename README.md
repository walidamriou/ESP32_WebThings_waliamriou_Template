# ESP32_WebThings_waliamriou_Template
 Template to implement webthings at Espressif ESP32 boards by ESP-IDF framework 


### WebThings
Web of things (WoT) is subset of IoT, where the communication is limited to web technologies, WoT is giving connected devices URLs on the World Wide Web.

### Tools used in this project
- VScode (to coding)
- Platformio (to compile and upload the code to ESP32 board)
- Postman (To test, send requestes to the device, and prototyping the project)

### Note
If you build & upload directly the current project you will get wifi access point in your esp32 board, with name: Walid Amriou WebThings device and password 123456789, but if you want to use this template to build your one sensor or device that connect to wifi so use wifi lib from this project: https://github.com/walidamriou/WalidAmriou_ESP_IoT

### API
_REST API links_    
For current implementation, the {ip} is 192.168.4.1    

{ip}/walidamriou/about  
{ip}/walidamriou/CurrentStatus  
{ip}/walidamriou/config  

__* GET {ip}/walidamriou/about__  
When you send request to {ip}/walidamriou/about you will get a reponse with the information about the device:  
     - The Name of the device: Walid Amriou Device  
     - Developer: Walid Amriou  
     - Firmware version: 1.0.0  
     - Chip: Espressif Systems ESP32 PICO (4M)  

__* GET {ip}/walidamriou/data__ 
When you send request to {ip}/walidamriou/data , you will get a reponse with the information about the current data status :  
     - Data1: Data  
     - Data2: Data 
     - Data3: 5646848   
     - Data4: 563.23  
     
__* POST {ip}/walidamriou/config__  
When you send request to {ip}/walidamriou/CurrentStatus , you will change the configuration of the system 


I have used JSON structure for all the structure of information and configuration  

### Copyright CC 2020 Walid Amriou

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

__You are free to:__
- __Share__ copy and redistribute the material in any medium or format

__Under the following terms:__
- __Attribution__ You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

- __NonCommercial__ You may not use the material for commercial purposes.

- __NoDerivatives__ If you remix, transform, or build upon the material, you may not distribute the modified material.

- __No additional restrictions__ You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

the software or Code or Scripts or any files in this source is provided "as is" and the author disclaims all warranties with regard to this files including all implied warranties of merchantability and fitness. in no event shall the author be liable for any special, direct, indirect, or consequential damages or any damages whatsoever resulting from loss of use, data or profits, whether in an action of contract, negligence or other tortious action, arising out of or in connection with the use or performance of this software or code or scripts or any files in this source.
