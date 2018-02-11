# RFM2Pi - Arduino IDE board support
## ATmega328 Optiboot @ 38,400baud w/ 8MHz Int. RC Osc.
- Arduino board json file to support [RFM2Pi hardware](https://wiki.openenergymonitor.org/index.php/RFM12Pi_V2)
- Introduced `ARDUINO_AVR_ATMEGA328_384_8` preprocesor macro 
```
#ifdef  ARDUINO_AVR_ATMEGA328_384_8   
   //RFM2Pi specific code
#else
  //OTHER CODE
#endif
```

### Installation via Boards Manager
#### Short procedure
- Add this link to your boards manager. `https://raw.githubusercontent.com/vvvlc/RFM2Pi-Arduino/master/boardsmanager/package_rfm2pi_index.json`
- Install *RFM2Pi AVR Board*

#### Detailed steps
- In Arduino IDE, Select menu *File*, *Preferences*
- Click icon next to *Additional Boards Manager URLs:*
- Add `https://raw.githubusercontent.com/vvvlc/RFM2Pi-Arduino/master/boardsmanager/package_rfm2pi_index.json` on new line.
![Preferences](/doc/preferences.png)
- Click Ok
- Go to *Tools*, *Board*, *Boards Manager...*
- Select Type: *Contributed*
- Click install *RFM2Pi AVR Board*
![Boards Manager](/doc/boardsmanager.png)
- Close it
- New *ATmega328 Optiboot @ 38,400baud w/ 8MHz Int. RC Osc.* board should show in *Tools/Board* menu
