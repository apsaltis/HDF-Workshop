
# Verifying your environment



### To connect using Putty from Windows laptop

- Right click to download [this ppk key](https://raw.githubusercontent.com/apsaltis/HDF-Workshop/master/hdf-workshop.ppk) > Save link as > save to Downloads folder
- Use putty to connect to the test node using the ppk key:
  - Connection > SSH > Auth > Private key for authentication > Browse... > Select hdf-workshop.ppk
![Image](https://raw.githubusercontent.com/apsaltis/HDF-Workshop/master/putty.png)

- Create a new seession called `hdf-workshop`, please note the IP address for the test instance is: 54.153.16.40.
![Image](https://github.com/apsaltis/HDF-Workshop/raw/master/putty-session.png)


### To connect from Linux/MacOSX laptop

- SSH into your EC2 node using below steps:
- Right click to download [this pem key](https://raw.githubusercontent.com/apsaltis/HDF-Workshop/master/hdf-workshop.pem)  > Save link as > save to Downloads folder
- Copy pem key to ~/.ssh dir and correct permissions
    ```
    cp ~/Downloads/hdf-workshop.pem ~/.ssh/
    chmod 400 ~/.ssh/hdf-workshop.pem
    ```
 - Login to the test ec2 node
    ```
     ssh -i  ~/.ssh/training-keypair.pem ec2-user@54.153.16.40

    ```
