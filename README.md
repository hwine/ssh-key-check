# ssh-key-check
Script to check ssh-keys for strength and pass phrase

This script checks all "likely candidates" for private key files in your
```~/.ssh``` directory. Each private key file is checked for conformance with
guidelines posted in [Mozilla's
wiki](https://wiki.mozilla.org/Security/Guidelines/OpenSSH#Key_generation).

# Operation

Run the script and view the output:
```bash
    ./check-ssh-keys
```

If you don't want the script poking around in your ```~/.ssh```
directory, you can copy the keys to test to a different directory.
Simply add the ```--ssh-dir DIR``` option to specify that directory.

Other options may become available over time. Use the ```-h``` option to
see them. Currently:
```
    $ ./check_ssh_keys --help
    usage: check_ssh_keys [options]
    Check private keys for conformance to EIS Guidelines at
    https://wiki.mozilla.org/Security/Guidelines/OpenSSH#Key_generation

    Options are:
        --ssh-dir   directory to check (default ~/.ssh/)
        -h|--help   this help

```
