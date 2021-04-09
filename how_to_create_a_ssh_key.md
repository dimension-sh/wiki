### How To Create A SSH Key

An SSH key is required to connect to dimension.sh services securely and for signing up for a user account. 

We recommend **ed25519** keys, but we accept **RSA** and the other OpenSSH supported key types, except **DSA**. 

#### Linux / \*BSD / Most \*nix Systems

You can use OpenSSH that'll most likely be provided by your OS distribution.

1. Access the terminal
2. Run the following command:

    ```
    ssh-keygen -t ed25519 -C "your_email@example.com"
    ```

    This will create two files `id_ed25519` and `id_ed25519.pub` in the folder `~/.ssh`, which will be the `.ssh` folder in your home folder.
3. Take note of the `id_ed25519.pub` file location, as this is your public key, which you'll need to provide during registration for an account.

#### Windows 10

The latest Windows 10 includes a version of OpenSSH that you can use to create a key without extra software.

1. Open a Command Prompt, or Powershell
2. Run the following command:

    ```
    ssh-keygen -t ed25519 -C "your_email@example.com"
    ```

    This will create two files `id_ed25519` and `id_ed25519.pub` in the folder `%USERPROFILE%/.ssh`, which will be the `.ssh` folder in your User folder.
3. Take note of the `id_ed25519.pub` file location, as this is your public key, which you'll need to provide during registration for an account.

#### Windows 10 using PuTTY

If your version of Windows 10 doesn't include OpenSSH and the `ssh-keygen` command doesn't work then you can install and use **PuTTY**.

1. Download PuTTY from the [official site](https://www.chiark.greenend.org.uk/~sgtatham/putty/) and install it. We recommend the MSI installer version to make it easier.
2. Open PuTTYGen from your start menu.
3. Select "ED25519" from the "Parameters" section at the bottom of the window.
4. Click "Generate".
5. After a few seconds, your key will be generated and appear in the Key section, after which click "Save Private Key" and save the file in a memorable location. 
6. Take note of the text in "Pubic Key" text box. This is the public key you'll need to provide when registering for an account.