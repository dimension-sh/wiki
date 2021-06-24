# Account Management

## Changing your password

To change your password, all you need to do is run the `passwd` command, and provide your current and new passwords.

```
[nikdoof@s1 ~]$ passwd
Changing password for user nikdoof.
Current password:
New password:
Retype new password:
passwd: all authentication tokens updated successfully.
[nikdoof@s1 ~]$
```

## Changing your default shell

By default, every new account is set to use `bash` as the login shell, but this can be quickly changed using the `chsh` command. Passing the argument `--list-shells` will show you all the shells you can switch to on the system.

```
[nikdoof@s1 ~]$ chsh --list-shells
/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
/usr/bin/tmux
/bin/tmux
/usr/bin/zsh
/bin/zsh
/bin/csh
/bin/tcsh
/usr/bin/csh
/usr/bin/tcsh
```

Once you've decided on a shell, you can run `chsh` without arguments to switch to the new one, to confirm you'll need to provide your password.

```
[nikdoof@s1 ~]$ chsh
Changing shell for nikdoof.
New shell [/bin/bash]
/bin/zsh
Password:
Shell changed.
[nikdoof@s1 ~]$
```


