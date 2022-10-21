# its-bio-project-22
Tre sensori di distanza Ultrasonici attaccati al Wio terminal, che danno in feedback su una striscia a led addressable. 
Per comppilare il codice é necessario installare la libreria [Ultrasound di Seeed](https://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/) e Adafruit Neopixel (trovabile dalle libreie) 

Problema: i sensori ad ultrasuoni hanno un delay() per funzionare. Leggendone più insieme si rallenta in maniera consistente lo sketch. 
Probabilmente togliendo il delay(250); alla fine del codice si può far andare più spedito il tutto. 

Possibile soluzione (parzialmente già messa in atto): usare un array di sensori LDR


![Wio Terminal GPIO Explained](https://files.seeedstudio.com/wiki/Wio-Terminal/img/WioT-Pinout.jpg)

Reference:
* [Wio Terminal GPIO Documentation](https://wiki.seeedstudio.com/Wio-Terminal-IO-Overview/)

