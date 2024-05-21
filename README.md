<p align="center"><img src="https://github.com/therealethanklein/Eclipse-/blob/main/whgC3vbJMwyorqhgXGwj--1--26tzz%20(1).jpg" height="200"></p>

<h1 align="center">Eclipse∞-</h1>

The deployable all-in-one bundle for [Eclipse∞](https://github.com/therealethanklein/Eclipse∞), a highly sophisticated proxy used for evading internet censorship or accessing websites in a controlled sandbox using the power of service-workers and more!

## Deployment

[![Run on Replit](https://binbashbanana.github.io/deploy-buttons/buttons/remade/replit.svg)](https://github.com/therealethanklein/Eclipse-/wiki/Run-on-Replit)
[![Deploy on Railway](https://binbashbanana.github.io/deploy-buttons/buttons/remade/railway.svg)](https://github.com/therealethanklein/Eclipse-/wiki/Deploy-on-Railway)
[![Remix on Glitch](https://binbashbanana.github.io/deploy-buttons/buttons/remade/glitch.svg)](https://github.com/therealethanklein/Eclipse-/wiki/Remix-on-Glitch)
[![Deploy to Koyeb](https://binbashbanana.github.io/deploy-buttons/buttons/remade/koyeb.svg)](https://github.com/therealethanklein/Eclipse-/wiki/Deploy-to-Koyeb)

If you are deploying to an alternative service or to a server, refer to [Deploy via terminal](https://github.com/therealethanklein/Eclipse-/wiki/Deploy-via-terminal).

Additional information such as [customizing your frontend](https://github.com/therealethanklein/Eclipse-/wiki/Customizing-your-frontend) can be found on the [wiki](https://github.com/therealethanklein/Eclipse-/wiki).

Support and updates can be found in our [Discord Server](discord.gg/unblock).

> [!IMPORTANT]  
> Until deployed on a domain with a valid SSL certificate, Firefox will not be able to load the site. Use chromium for testing on localhost

### HTTP Transport
The example uses [EpoxyTransport](https://github.com/MercuryWorkshop/EpoxyTransport) to fetch proxied data encrypted. 

You may also want to use [CurlTransport](https://github.com/MercuryWorkshop/CurlTransport), a different way of fetching encrypted data, or [Bare-Client](https://github.com/MercuryWorkshop/Bare-as-module3), the legacy (unencrypted!) transport.

In public/register-sw.js, look for the line `BareMux.SetTransport("EpxMod.EpoxyClient", { wisp: "ws://localhost:8080/wisp" });`, which can be changed to any of the transports. Make sure to `importScripts` the transport's bundle in `public/uv/sw.js` and add a script tag in both `public/404.html` and `public/index.html`. 

See the [bare-mux](https://github.com/MercuryWorkshop/bare-mux) documentation for more information
