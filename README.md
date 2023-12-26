# Kali Linux Support Wi-Fi adaptor List 
This is the list of Kali supported Wi-Fi adaptor and chipset


| Chipset      | Packet injection & Monitor mode Support | Plug And Play | Band Support Recommended 2.4 GHz & 5 GHz | Tx Power    | Fake access point (Rogue AP) | Eaphammer    | VIF Mode (virtual interface) | Wifipumpkin3 | Kali Nethunter (Rooted Android) |
|--------------|----------------------------------------|---------------|----------------------------------------|-------------|------------------------------|--------------|------------------------------|--------------|---------------------------------|
| AR9271 (150Mbps) | Yes                                    | Yes           | 2.4 GHz                                | 20 dBm      | Yes                          | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RT3070 (150Mbps) | Yes                                    | Yes           | 2.4 GHz                                | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RT3072 (300Mbps) | Yes                                    | Yes           | 2.4 GHz                                | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RTL8187 (54Mbps)  | Yes                                    | Yes           | 2.4 GHz (B/G)                          | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RT2770F (150Mbps)| Yes                                    | Yes           | 2.4 GHz                                | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RTL8812AU (1200Mbps) | Yes                                    | No (Driver Required) | 2.4 GHz & 5 GHz               | 20 dBm      | No (Airbase-ng Only)        | No           | No                           | No           | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RT5572 (300Mbps) | Yes                                    | Yes           | 2.4 GHz & 5 GHz                       | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |
| RT3572 (300Mbps) | Yes                                    | Yes           | 2.4 GHz & 5 GHz                       | 30 dBm (Unlocked) | Yes                      | Yes          | Yes                          | Yes          | Need Kernel/firmware/driver<br>For Multiple Adapter need Module Support |



# Wireless Cards and NetHunter

External wireless cards are necessary because Android devices do not support monitor mode on most devices apart from some Qualcomm chips used in modern Snapdragon SOC. There are some devices that can support monitor mode with a modified firmware and kernel such as the Nexus 5, 7 (2012), and Nexus 6P. Right now, only a specially modified version of Nexus 5 supports monitor mode for Nethunter.

A couple of limitations are that Android devices require a USB-OTG cable and the power output is limited. Because of these limitations, not all wireless cards can receive the necessary power output and may not have external power (y-cable) support.

When asking the question “What is the best card for use with NetHunter?”, you need to ask yourself what your use case is. While all cards will likely perform similar at closer ranges, some of them have increased transmit power and antenna attachments which allow them to work at longer distances than small form factor cards. There is also the possibility that your device may only provide 450 or less mA of power over OTG rather than the full USB 500 mA specification. If this is the case, you may want to consider devices with lower transmit power.

source: https://www.kali.org/docs/nethunter/wireless-cards/
