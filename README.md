# Icee.cc Client

Icee exposes your localhost to the world for easy testing and sharing! No need to mess with DNS or deploy just to have others test out your changes.

## Installation ##

```
npm install -g icee
```

This will install the Icee module globally and add the `icee` client cli tool to your PATH.

## Use ##

Assuming your local server is running on port 8000, just use the `icee` command to start the tunnel.

```
icee --port 8000
```

That's it! It will connect to the tunnel server, setup the tunnel, and tell you what url to use for your testing. This url will remain active for the duration of your session.

You can restart your local server all you want, `icee` is smart enough to detect this and reconnect once it is back.

### Arguments

Below are some common arguments. See `icee --help` for additional arguments.

* `--subdomain` request a named subdomain on the Icee server (default is random characters)
* `--local-host` proxy to a hostname other than localhost

## Server ##

See [obie-ai/icee-server](//github.com/obie-ai/icee-server) for details on the server that powers Icee.

## License ##
MIT
