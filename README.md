# PyWebserver
Basic webserver for lab testing

The files and instructions assume that you're logging in using user "ubuntu".  Edit the home directories and "ln" command below appropriately if using a different user.

The following steps will:
- Change to the home directory
> cd
- Clone the project into ~/PyWebserver
> git clone https://github.com/dbrown92700/PyWebserver/
- Define a new webserver service
~~~
cd /etc/systemd/system/
sudo ln -s /home/ubuntu/PyWebserver/webserver.service
sudo systemctl daemon-reload
~~~
- Start that service and show the status of it
~~~
sudo systemctl start webserver.service
sudo systemctl status webserver.service
~~~
- You can stop/start the service with the "sudo systemctl [stop/start]" commands

The webserver will be running on port 8080

