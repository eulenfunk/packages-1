##### Hintergrund
Alle Einstellungen aus der Datei "site.conf" sind nicht Upgrade-fest!<br>
Leider sind da auch die verwendeten WLAN-Kanaele (2,4MHz u. 5MHz) mit dabei.<br>
<br>
Durch dieses Gluon-Package wird sichergestellt, dass evtl. veränderte Radio-Kanal-Einstellungen nach einem Sysupgrade automatisch wieder hergestellt werden. 
Unabhängig, vom Inhalt der Datei ‚site.conf‘.<br>
<br>
##### Vorgehensweise
Nach einem Sysupgrade, jedoch vor dem ersten Reboot, werden Upgrade-Skripte automatisch abgearbeitet.<br>
Die Skripte dieses Packages hängen sich in die Skript-Abarbeitung ein<br>
(siehe http://gluon.readthedocs.org/en/latest/dev/upgrade.html).<br>
<br>
Das Skript **110-backup-wireless-channel** sicher alte Kanal-Einstellungen.<br>
Das Skript **201-restore-wireless-channel** stellt sie wieder her.<br>
<br>
<br>
