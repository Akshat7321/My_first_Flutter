1	mkdir music
	touch song{1 2 3 4 5 6 7 8 9 10}.mp3
	mv song*.mp3 music
	ln -s music audio
	
2	sudo groupadd -g 1237 sysadmin
	sudo adduser rob(set password to linux123)
	sudo adduser bob(set password to linux123)
	sudo usermod -a -G manager rob
	sudo usermod -a -G manager bob
	sudo adduser max(set password to linux123)

3	sudo chage -E 2018-07-12 max
	sudo chage -d 0 bob
		
4	mkdir /home/manager

5	# useradd -u 4223 gabriel

6	tar cvfj archive.tar.bz2 -P /etc/hosts
	mv archive.tar.bz2 /tmp/var/

7	cd /etc/
	grep -n udp * > udp_services.txt

8	top
	(press Shift+F)
	(choose CPU%(already set as default) from the list and press s)
	
9	alias stat="/bin/uptime" 

10	INSERT
	vim test.html---(press i to insert text)---(press escape to go back)---:w(+Enter to save)
	DELETE
	:sh---rm textfile.xml
	QUIT
	:q

11	query current zone: firewall-cmd --get-active-zone
	sudo firewall-cmd --set-default-zone=dmz
	get all zones: firewall-cmd --get-zones > new.txt
	
12	firewall-cmd --permanent --add-port=8080/tcp
	sudo firewall-cmd --zone=public --list-ports > zones.txt

13	firewall-cmd --permanent --add-forward-port=port=80:proto=tcp:toport=8080
	firewall-cmd --reload

	
	
