# hs20-js-dev-env

## Editor & Configuration

    - Install VS Code
    - Edit .editorconfig

## Package Manager

<<<<<<< HEAD
* Install Node and set up npm 
    - Install Node & npm through nvm https://github.com/nvm-sh/nvm#installing-and-updating
=======
* Install Node and set up npm
>>>>>>> 8239cf6e4d42e664bee721bd3f626322f02ae73b

    - Install Node & npm through nvm https://github.com/nvm-sh/nvm#installing-and-updating
    - Create package.json

* Set up Security Scaning

    Beginning with npm@6, a new command, npm audit, recursively analyzes your dependency trees to identify specifically what’s insecure, recommend a replacement, or fix it automatically with npm audit fix...

    ~ npm audit
    ~ npm audit --audit-level high
    ~ npm audit fix

## Development Web Server

    * Config express app
    
    * Share work-in-progrss
        - locatunnel
            ~ npm install localtunnel -g
            ~ lt --port 3000 --subdomain humberto

## Task Automation

    * npm scripts
        - Write in "scripts" inside package.json

## Transpiling

    * Babel
        ~ code .babelrc
        - edit npm automated scripts

## Bundling

    * Why Bundle ?
        - Common JS doesn't work in web browsers
        - Package projects into file(s)
        - Improve Node performance
    
    * Webpack
        ~ code .webpack.config.dev.js
        _ Set up development server to serve up webpack bundle
            ~ code buildScripts/srcServer.js

