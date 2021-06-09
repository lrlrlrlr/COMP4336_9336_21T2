# COMP4336_9336_21T2

## Tutorial Timetable
| Tutorial_ID	|Time|	Tutor|	Zoom link|	Recording Link|
|-------------|----|-------|-----------|---------------|
|T12A|	Tue 12:00 - 14:00|	Wei	  | [link](https://unsw.zoom.us/my/weisonglabs) |	[link](https://drive.google.com/drive/folders/1c66aiem3LrNVdekhe6oGm_eC_nn_DnAG)
|T14A|	Tue 14:00 - 16:00|	Wei	  | [link](https://unsw.zoom.us/my/weisonglabs)|	[link](https://drive.google.com/drive/folders/1c66aiem3LrNVdekhe6oGm_eC_nn_DnAG)
| T18A|	 Tue 18:00 - 20:00|	 Rui	|  [link](https://us02web.zoom.us/j/81571193242?pwd=dlcxS1dCK2wrRXkxWWRJam00dE5Vdz09)|	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FbRCpqOxxMzq5jzlehaX6E0)
| W14A|	 Wed 14:00 - 16:00|	 Rui	|  [link](https://us02web.zoom.us/j/87087314897?pwd=YVZiM05DaHRXWm1ZTisvMTJYRU9BQT09)|	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FazqYHua7-xroReksn1-q-H)
|W16A|	Wed 16:00 - 18:00|	Gary	| [link](https://unsw.zoom.us/j/4245058685)|	-
|H14A|	Thu 14:00 - 16:00|	Gary	| [link](https://unsw.zoom.us/j/4245058685)| - 
| H16A|	 Thu 16:00 - 18:00|	 Rui	|  [link](https://us02web.zoom.us/j/83907740986?pwd=b0tJMlBJNGpBTkk0Mk01b1JkQTNaZz09)| 	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FbGloHuJf92plEATVT76GOX)

--------------------------------
## Lab1  
 ### Installation
  #### Mac
  - Wireshark: to analyse the packets. [download link](https://www.wireshark.org/download.html)
 #### Linux
  - Wireshark: to analyse the packets.   
   
       Installation command:  
       `sudo apt install wireshark`  
   
 #### Windows 10
  - Wireshark: to analyse the packets. [download link](https://www.wireshark.org/download.html)
  - Microsoft Network Monitor 3.4: to collect the 802.11 packets. [download link](https://www.microsoft.com/en-us/download/details.aspx?id=4865)
  - Npcap: you may also need to install this to make Microsoft Network Monitor 3.4 working properly. [link](https://nmap.org/npcap/)


 ### Basic operation of wireshark
   video: [learn wireshark in 10min](https://www.youtube.com/watch?v=lb1Dw0elw0Q)  

  You should be able to:  
  - capture the packet
  - open a .cap file
  - apply a filter
  - create/remove a column
  - output to .CSV file
--------------------------------  

## Lab2 
[lab recording](#todo)
(underconstruction, coming soon...)  
Task1:
  - what we need to do?
  - how?

Task2:
  - how to capture

**General questions**:
 - I can't capture the packet with Wireshark/Microsoft Network Monitor.  
         --> You may need to have a look at your configuration, for win10, you may need to install npcap and reboot before you start to capture. For more help please post your problem at the forum.
 - I can't capture 802.11 packets.  
         --> this may happen since some wireless network card does not support us to get the raw 802.11 packets, but you may be able to find some TCP/UDP packets that have "signal strength", then you can use them to finish your task.

    
 - There is no SSID information inside the packet.  
         --> this is normal in win10, just descript what happened in your report.
 - There is only signal strength but no noise lvl and SNR ratio?  
         --> this is normal in win10, just descript what happened in your report.
 

--------------------------------  

**Important: this is not the official support from COMP4336/9336, all the information here is for reference only.**  
 
**If you have any doubt/question, please post them into the Moodle forum.**
