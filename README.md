osx-proxy
========

**This should work with any remote SSH server!**

Move `proxy` to somewhere in your PATH.
Make proxy executable via `chmod +x proxy`.

Choose between enabling proxy authorization as Environmental Variables or through directly placing credentials in proxy file.

If you choose to place the variables as Env varibles, make sure that file is sourced by your `.bashrc` or `.zshrc`.

Edit settings in `proxy`:

Set PROXY_USER and PROXY_HOST somewhere in sourced path
ie enter following info into .bashrc or .zshrc or a more private auth file

```
export PROXY_USER='user'
export PROXY_HOST='example.com'
```

If choosing not to set credentials as Environmental Variables, replace the values below for $PROXY_USER and $PROXY_HOST with genuine credentials.

```
remoteuser="SSH_USER_HERE"
remoteproxy="IP_OR_HOSTNAME_HERE"
remoteport="22"
```

Run like this:

```
proxy on|off|killall|shutdown|[no_argument]

on = turn proxy on and setup ssh tunnel
off = turn proxy off
killall = kill all ssh tunnels
shutdown = off and killall
no_arg = toggle current state (if on, set as off, if off set as on)
```
