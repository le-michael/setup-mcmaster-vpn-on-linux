# Setup McMaster VPN on Linux

## 1. Download VPN

Download the linux version of the vpn from the following website:
https://www.mcmaster.ca/uts/network/vpn/

## 2. Extract file

Once the download is complete you should have a file called `anyconnect-linux64-4.6.04056-predeploy-k9.tar.gz`. You will need
to extract the file. Use the following command.

`tar xfv anyconnect-linux64-4.6.04056-predeploy-k9.tar.gz`

This will extract the tar file into the current directory. Once complete you should have a new folder called `anyconnect-linux64-4.6.04056`.

## 3. Install VPN

In the directory where you extracter the tar file `cd` into the vpn folder and run `vpn_install.sh`.

```
cd anyconnect-linux64-4.6.04056/vpn
./vpn_install.sh
```

## 4. Connect to VPN

### Using terminal

Once the installation is complete you can run the vpn binary in the vpn folder.

```
./vpn
```

This will open the anyconnect CLI. Run the following command in the CLI to connect to the McMaster servers 

```
connect sslvpn.mcmaster.ca
```

Enter your credentials and you are now connected. You can disconnect by typing `disconnect` within the CLI.


### Using ui

Once the installation is complete you can run the vpnui binary in the vpn folder. 

```
./vpnui
```

Enter your credentials into the input boxes and press connect. You can disconnect by pressing the connection tab and pressing disconnect.
