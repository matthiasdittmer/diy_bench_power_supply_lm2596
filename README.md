# DIY Bench Power Supply LM2596
There is a ton of material on the internet about DIY bench power supplies based on TI LM2576 [1] and TI LM2596 [2] buck converters.

I used [3], [4] and [5] as a starting point for my own design.

# Repository structure
```
/software/      Bare-metal firmware implementation with OOP approach (PlatformIO project)
/hardware/      Circuit schematics and simulations as documentation
/mechanics/     Housing design files
/misc/          Material of built version
```

# Features
* Two channels with on/off LED and button per channel
* Adjustable voltage
* Settable and adjustable current limit
* LED indicators for enabled current limit and reached limit
* LCD showing current voltages, currents and current limits per channel
* Buzzer feedback (acoustic button feedback, current limit warning)

# Design / Components
* Arduino Pro Mini as controller (mainly because of the 8 analog pins)
* LM2596 buck converter boards [6]
* HP notebook 90W power supply brick (19V, max. 4.74A)

References:
* [1] Website TI LM2576: https://www.ti.com/product/LM2576
* [2] Website TI LM2596: https://www.ti.com/product/LM2596
* [3] GreatScottLab LM2596 modification project: https://www.instructables.com/id/Adding-a-Current-Limit-Feature-to-a-BuckBoost-Conv/
* [4] Youtube Video LM2576 design: https://www.youtube.com/watch?v=EVL7TzCde8I
* [5] Website article LM2576 design: https://www.smbaker.com/lm2576-constant-voltage-constant-current-switching-power-supply
* [6] Converter from ebay Germany: https://www.ebay.de/itm/3x-LM2596-DC-Step-Down-Spannungswandler-Arduino-Modul-Regler-LM2596S/252785167788

