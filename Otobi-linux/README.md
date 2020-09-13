To use <b>Otobi Layout</b> in Linux Distribution OS, follow the following procedures.<br>
You can use IBus (SCIM) or XKB to enable Otobi layout. But <i>Remember that you cannot produce a Bengali ligature like (Ya-Phala) in XKB.</i>
You have to use IBus (SCIM) for this kind of feature.<br>
The reference operating system is Ubuntu19.04.<br>

<h3>IBus (SCIM)</h3>
First perform:<br>
<code>sudo apt update</code><br>
Then install IBus and m17n library for Unijoy layout by following command in terminal:<br>
<code>sudo apt-get install ibus ibus-m17n m17n-db ibus-gtk</code><br>
Copy and replace the bn-unijoy.mim file to /usr/share/m17n folder. To do so you have to open Files as root by following command:<br>
<code>sudo nautilus</code><br>
Or you can copy and replace bn-unijoy.mim from Home folder by this command:<br>
<code>sudo cp -r /home/USERNAME/bn-unijoy.mim /usr/share/m17n</code><br>
After completing this whole process, you have to restart ibus:<br>
<code>ibus restart</code><br>
Then enable Bengali (Unijoy(m17n)) from:<br>
<code>Settings > Region & Language > Add an Input Source > Bangla</code><br>
This will work as Otobi layout.<br><br>

<h3>XKB</h3>
Copy the bangla and evdev.xml file to these folder respectively:<br>
<code>/usr/share/X11/xkb/symbols/</code><br>
<code>/usr/share/X11/xkb/rules/</code><br>
To do it as root user open Files as:<br>
<code>sudo nautilus</code><br>
Or you can copy from Home folder by this command:<br>
<code>sudo cp -r /home/USERNAME/bangla /usr/share/X11/xkb/symbols/</code><br>
<code>sudo cp -r /home/USERNAME/evdev.xml /usr/share/X11/xkb/rules/</code><br>
You might have to restart your system to effect changes.<br>
Then enable বাংলা from:<br>
<code>Settings > Region & Language > Add an Input Source > Bangla</code><br>
This will work as Otobi layout. But you cannot use some ligatures such as Ya-Phala, Ra-Phala, Reph. Use Show keyboard Layout to examine the layout.<br><br>
