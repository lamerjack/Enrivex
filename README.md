# Enrivex
simple standalone player for raspberry py


Fare il download della distribuzionedietpi per il modello richiesto
estrarre il file scaricato
caricarlo nella scheda sd attraverso il programma Win32DiskImager
inserire la scheda sd in raspberry, che installerà il software automaticamente
quando avrà finito l'installazione, chiedera il login:    - username =root
                                                          - password =dietpi 
1) entrare nella configurazione
2) aprire option network e deselezionare ipv6
3) display options,risoluzione 1920x1080 (non opengl) cambiare 64 mb attivare hdmi boost
5) security option cambiare l'host name in Envirex
6) cambiare la regione ed inserire roma
7) file server, selezionare samba
8) installare il software con le modifiche apportate
cambiare la password in Matrox12 attraverso il comando passwd, cambiare la password per samba smbpasswd
con il comando apt-get update e poi apt-get upgrade verificare gli aggiornamenti
apt-get install git
aggiungere il programma omx player con il comando apt-get install omxplayer 
git clone https://github.com/lamerjack/Enrivex.git

aggiungere lo script per farlo partire fin da subito nano /etc/rc.local
            /root/Enrivex/videoplayer.sh
            exit 0

