osx-proxy
========

**This should work with any remote SSH server!**

Move `proxy` to somewhere in your PATH.
Make proxy executable via `chmod +x proxy`.

Choose between enabling proxy authorization as Environmental Variables or through directly placing credentials in proxy file.

If you choose to place the variables as Env varibles, make sure that file is sourced by your `.bashrc` or `.zshrc`.

Edit settings in `proxy`:

```
remoteuser="SSH_USER_HERE"
remoteproxy="IP_OR_HOSTNAME_HERE"
remoteport="22"
```

Run like this:

```
proxy on|off|killall
```
