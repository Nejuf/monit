## Fedora 15 Monit ##

This Monit repository has been modified because the fedora package was outdated and modifications had to be made to the HTML to fit the UI.

## Installation - Fedora ##
1. cd into repository.
2. Run the below, which will ovewrite the binary at /usr/bin/monit

```
./bootstrap
./configure --without-pam --prefix=/usr
make
sudo make install
```

3. Make sure /etc/monit.conf is set as desired, or copy over monitrc
4. Start the monit server with:
```
sudo service monit restart
```

5. Check the status of the service with:
```
sudo monit status
```

6. View the status page as html at <http://localhost:2812>

