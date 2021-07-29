# COMP4336_9336_21T2

## Tutorial Timetable
| Tutorial_ID	|Time|	Tutor|	Zoom link|	Recording Link|
|-------------|----|-------|-----------|---------------|
|T12A|	Tue 12:00 - 14:00|	Wei	  | [link](https://unsw.zoom.us/my/weisonglabs) |	[link](https://drive.google.com/drive/folders/1c66aiem3LrNVdekhe6oGm_eC_nn_DnAG)
|T14A|	Tue 14:00 - 16:00|	Wei	  | [link](https://unsw.zoom.us/my/weisonglabs)|	[link](https://drive.google.com/drive/folders/1c66aiem3LrNVdekhe6oGm_eC_nn_DnAG)
| T18A|	 Tue 18:00 - 20:00|	 Rui	|  [link](https://unsw.zoom.us/my/ruilabs)|	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FbRCpqOxxMzq5jzlehaX6E0)
| W14A|	 Wed 14:00 - 16:00|	 Rui	|  [link](https://unsw.zoom.us/my/ruilabs)|	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FazqYHua7-xroReksn1-q-H)
|W16A|	Wed 16:00 - 18:00|	Gary	| [link](https://unsw.zoom.us/j/4245058685)|	-
|H14A|	Thu 14:00 - 16:00|	Gary	| [link](https://unsw.zoom.us/j/4245058685)| - 
| H16A|	 Thu 16:00 - 18:00|	 Rui	|  [link](https://unsw.zoom.us/my/ruilabs)| 	 [link](https://www.youtube.com/playlist?list=PL62Uy8LvT4FbGloHuJf92plEATVT76GOX)
--------------------------------  

## Project  
### Due time changed to: 
	**4pm 05 August**
### Flexibility for the project:  
1. You can extend your gesture duration (for example, you can design a 6 seconds gesture)  
2. Object in the hands is allowed, you can have an object in your hand.  
3. You can use different platforms to do the project, e.g. RaspberryPI, Arduino.  

### Help session:
## Tutorial Timetable
| Help session	|Time|	Tutor|	Zoom link|	
|-------------|----|-------|-----------|
|1|	Mon 10:00 - 12:00|	 Rui	|  [link](https://unsw.zoom.us/my/ruilabs)|
|2|	Mon 18:00 - 20:00|	 Rui	|  [link](https://unsw.zoom.us/my/ruilabs)|
|3|	Tue 10:00 - 12:00|	Wei	  | [link](https://unsw.zoom.us/my/weisonglabs)|
|4|	Tue 18:00 - 20:00|	 Gary	|  [link](https://unsw.zoom.us/j/4245058685)|	
|5|	 Wed 10:00 - 12:00|	 Wei	  | [link](https://unsw.zoom.us/my/weisonglabs)|
|6|	 Wed 18:00 - 20:00|	 Gary	|  [link](https://unsw.zoom.us/j/4245058685)|	

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
[lab recording](https://youtu.be/5gnzImIi8us)  

Task1 - key steps:
  - Apply a SSID filter:  `wlan.ssid==SSID_NAME`
  - Create a new column:  Select the information, then Right click it, Apply as Column.
  - Export CSV: File - Export Packet Dissections - As CSV...
  - Plot: You can plot the graph with Excel or Python.

Task2:
  - How to capture: 
    - Mac/Linux: Use Wireshark
    - Win10: Use Microsoft Network Monitor 3.4


**General questions**:
 - I can't capture the packet with Wireshark/Microsoft Network Monitor.  
         --> You may need to have a look at your configuration, for win10, you may need to install npcap and reboot before you start to capture. For more help please post your problem at the forum.
 - I can't capture 802.11 packets.  
         --> this may happen since some wireless network card does not support us to get the raw 802.11 packets, but you may be able to find some TCP/UDP packets that have "signal strength", then you can use them to finish your task.

    
 - There is no SSID information inside the packet.  
         --> this is normal in win10, just descript what happened in your report.
 - There is only signal strength but no noise lvl and SNR ratio?  
         --> this is normal in win10, just descript what happened in your report.
 
 - How to turn on the Monitor mode (in order to capture the raw 802.11 packets) in MAC?  
         --> please refer to [this document](https://github.com/lrlrlrlr/COMP4336_9336_21T2/blob/main/macOS%20'Monitor'%20issue.pdf)
--------------------------------  
 

## Lab3   

 - How to calculate the slope?
	- Linear Regression ([Excel](https://www.youtube.com/watch?v=L_a8Z0BVjyM&ab_channel=MonaSchraer) , [numpy](https://numpy.org/doc/stable/reference/generated/numpy.polyfit.html))  
	- Drop the *outlier* if needed	

 - How to calculate the R-squared ?  
	- simply use the [calculator](https://ncalculators.com/statistics/r-squared-calculator.htm)  

 - What if I can’t capture the packets? 
    - Make sure your configuration is correct.  
    - Borrow a laptop  
    - Buy a wireless adapter [example](https://www.kogan.com/au/buy/timetech-australia-usb-wifi-wireless-n-300m-adapter-wi-fi-dongle-high-signal-gain-80211ngb-6595190423749-39667288572101/?utm_source=google&utm_medium=product_listing_ads&gclid=CjwKCAjw_JuGBhBkEiwA1xmbRU3QRyBFBKzhLe1AGVTXb7eelCgkqiWQBI9rR2VRSKc4WjiDxRweXBoC_g8QAvD_BwE)

--------------------------------

## Lab4   

 - How many dataset (.csv files)?
 	- 4 csv file should be submitted:  3x with obstacle + 1x without obstacle
 	

 - What kind of graph should I use in the report?
 	- Violin plot recommended
 	- You can use any kind of plot as you want, as your can clearly show the distribution of RSS
 
 - How to choose Band/Frequency for your hotspots?
	- Android: it will be very easy, please have a check of your hotspot configuration.
	- Laptop: it will be very easy, please have a check of your hotspot configuration.
	- iPhone: You may not be able to switch the band as you want with iPhone, if you are using iPhone 12, then have a try [here](https://www.idownloadblog.com/2020/11/04/iphone-personal-hotspot-wi-fi-bands-tutorial/)


 - I can only capture 10 packets per minute?
  	- You can increase the traffic between your device and hotspot. By:
		 - Play an online video while capturing
	 	 - Use ping command while capturing

 - My RSSI or Signal strength is positive?
	 - Since RSSI is a completely arbitrary value that has no relationship to any particular physical parameter, it can also be represented in a positive form, where the RSSI value is 0 to 100, with 100 being the strongest signal possible.

--------------------------------

## Lab5  

 - Can not observe the data rate change?  
	 - Try different distance, if possible, try outdoor(you can have more distance)

 - Still not working (can not capture any packet with MCS index and data rate)?  
	 - A sample is provided in [this link](https://www.dropbox.com/s/2xssie4i8txh05e/Lab%205%20sample%20dataset.zip?dl=0) 
	 - Note: if you are using this sample dataset, you should specify in your report, and tell us the reason why you can not capture the packets by yourself. If you failed to prove your effort, you might lose the mark on data collection part.

--------------------------------

## Lab8
 -  Notice: the old lab9(Gesture detection with WiFi RSS) is switch to lab8 now;
 -  What if I can not get the 50-100 packets per second in the task?  
	 -  It doesn't matter, just try your best to get as much as you can.  
 -  How to have the regular intervals for each packets?  
 	-  You can use the ping command to get a stable interval.Limited to the accuracy of our equipment, the interval time does not need to be very precise, such as 0.1s, 0.13s and 0.9s. We can roughly think that their intervals are equal.



--------------------------------

## You may find [this](https://github.com/lrlrlrlr/COMP4336_9336_21T2/blob/main/Quiz_samples.pdf) is useful for your quiz preparation.

## How can I get help?  
 - post it on the forum.  
 - join any of the online tutorials.  

**Important: this is not the official support from COMP4336/9336, all the information here is for reference only.**  
 
**If you have any doubt/question, please post them into the Moodle forum.**
