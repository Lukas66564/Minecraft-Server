# Minecraft-Server

Minecraft-Server zum Testen von Farms und Experimentieren mit Server-Performance und Belastungsgrenzen.

## Hintergrund

Ein Freund und ich haben viel auf dem Minecraft-Server DonutSMP.net gespielt und dort große Farms gebaut. Irgendwann wollte ich einen eigenen Server haben, auf dem wir Farms und andere Redstone-Konstruktionen für DonutSMP testen konnten.

## Einrichtung

Für den Server habe ich auf meinem Proxmox-Server einen LXC-Container erstellt und darin einen Minecraft-Server eingerichtet.

Als Verwaltungsoberfläche habe ich **mcsManager** installiert und darüber einen Paper-Server im Vanilla-Stil erstellt. Der Server lief im Whitelist-Modus, sodass nur freigeschaltete Spieler beitreten konnten.

Damit wir auch von außerhalb unseres Netzwerks auf den Server zugreifen konnten, habe ich in den FRITZ!Box Einstellungen eine Portfreigabe für **TCP-Port 25565** auf den LXC-Container eingerichtet. Zusätzlich habe ich eine DuckDNS-Domain geholt und einen Cronjob erstellt, der die öffentliche IP-Adresse automatisch bei DuckDNS aktualisiert.

## Experimente

Auf dem Server haben wir verschiedene Farms und Traps für DonutSMP ausprobiert.

Später wollten wir herausfinden, wie stark wir den Server belasten können. Dafür haben wir mit Command-Blöcken extrem viele Mobs gespawnt, bis der Server schließlich abgestürzt ist.

Das Projekt war ein Hobbyprojekt, bei dem ich praktische Erfahrungen mit Proxmox, Linux-Containern, Minecraft-Server-Hosting, Netzwerk-Konfiguration und Performance-Tests sammeln konnte.
