# SSH

Use an key to SSH into your machine without a password.

## Generate a key

Follow Github's instructions on generating a key pair (you can also add them
to your Github account if you wish to use Git).

## Add to authorized_keys

Add your public key (`~/.ssh/id_rsa.pub`) to `~/.ssh/authorized_keys`, creating
the file if necessary. Make sure that `authorized_keys` has file permission `600`.

## Copy to another machine

Copy `~/.ssh/id_rsa` (the private key) to the machine you wish to SSH in from.

Try to SSH in using the key:

`ssh -i path/to/id_rsa pi@raspberrypi.local`

If this was successful, you should have been logged in without a password prompt
(other than the password on the key itself, which your OS can save for you).

## Add to your SSH agent

Add the key to your SSH agent so that you don't have to specify it in future:

`ssh-add path/to/key`

You should now be able to SSH in with `ssh pi@raspberrypi.local` without being
asked for a password.

It's recommended that you now change the Raspberry Pi's password to something
very strong, using the key as your main means of entry.
