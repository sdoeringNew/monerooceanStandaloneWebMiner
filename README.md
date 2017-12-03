# Moneroocean standalone web miner

[moneroocean.stream](https://moneroocean.stream/) is a [Monero](https://getmonero.org/) mining pool. It offers the possibility of web mining hashes.
  
The moneroocean standalone web miner offers a simple possibility to include the web miner into your homepage.

Just add a JavaScript and an element containing the mining wallet to your page and you are done.

Look [https://sdoeringnew.github.io/](https://sdoeringnew.github.io/) for an example. 

# How to

The stand alone web miner depends on [jQuery](https://jquery.com/) v1.4.4 or higher.  
The web miner code itself can be found [here](web_miner.js).

```html
<script type="text/javascript" src="jquery.min.js"></script>
<script type="text/javascript" src="web_miner.js"></script>
```

Additionally place this to the page.

```html
<div id="moneroocean-web-miner" data-login="YOUR_MONERO_WALLET_HERE"></div>
```

That's it.

The rest will be created dynamically once the script has been loaded.

# Configuration

* login
  * the mandatory Monero wallet ID to mine for
* statsInterval
  * the interval the mining statistics will be updated in milliseconds
  * default: ```2500```
* threads
  * the number of threads to mine with
  * default: ```1```
* autostart
  * ìf set to ```true``` the mining will start automatically once the page has been loaded
  * default: ```false```
