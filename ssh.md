
# How To Connect Your Other Machine Using SSH

1. Setup SSH host
    - Install the ssh openssh on the server (machine #1 that is hosting information and connecting to the other machine)
- On Linux:
    ``` bash
    sudo apt-get install openssh-server
    ```
- On Windows: [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)

- On Mac: Comes pre-installed

2. Connect to a remote host/computer2
    - Enter the following command in the client terminal, making sure to replace the username with the host machine's \<username> and the \<hostname> with the ip address for that host machine.
    ``` bash
    ssh <username>@<hostname>
    ```
    You will be prompted to verify the ECDSA key fingerprint, enter **yes** if it is correct.
    
3. Once your terminal connects to the host machine, the username and hostname will be in the terminal. You can access all of the files via the terminal and edit the files via Vim, nano or transfer it to the device.


# Terminology
- Host
- Terminal
- Vim
- SSH
