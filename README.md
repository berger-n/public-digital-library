# public-digital-library

## Install

It is recommended to use [yarn](https://yarnpkg.com/) to install the app and any other packages. Installation instructions for each platform are on their [website](https://yarnpkg.com/lang/en/docs/install/).

This will install nodejs as well. yarn is similar to npm (which you may have used in the past), but has better performance and more reliable dependency resolution.

After yarn is installed, clone the repo, then simply run

    yarn install

To start the test server:

    yarn start

It should automatically open the test page in Chrome. Otherwise, visit <http://localhost:3000>



## Settings

### URL to lds-pdi

<!--By default, the app will test on startup where lds-pdi is reachable. The first candidate url is `http://localhost:8080`, then it tries `http://localhost:13280` and finally `http://buda1.bdrc.io`.

This automatic setting can be bypassed using a `GET` parameter if needed: `?lds-pdi=...`. For example, `http://localhost:13280?ldspdi=bdrc1.bdrc.io:13280` will use the online `fuseki` server instead of the default `http://localhost:13280`.-->

There is a `config-defauls.json` located in `/public` directory. It contains:
* a list of candidate urls to `lds-pdi`
* an index in the list to use on startup.

Default settings can be overridden using a separate `/public/config.json`.
