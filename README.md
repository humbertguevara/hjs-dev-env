# hs20-js-dev-env

## Editor & Configuration

    - Install VS Code
    - Edit .editorconfig

## Package Manager

* Install Node and set up npm 
    - Install Node & npm through nvm https://github.com/nvm-sh/nvm#installing-and-updating

* Install Node and set up npm

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

    CHECK AGAIN
        ~ code .webpack.config.dev.js
        _ Set up development server to serve up webpack bundle
            ~ code buildScripts/srcServer.js

    Sourcemaps
        - Maps the bundle code back to the original source
        - Could be generate automatic as pasrt of our build proccess
        - Downloaded only if developer tool is open

## Linting

    * Set up and Config ESLint 
        - ESLint Recommended
        - eslint-watch
        ~ code .eslintrc.json
        - add to scripts in package.json:
            "lint": "esw webpack.config.* src buildScripts --color"
            "lint:watch": "npm run lint -- --watch"

## Testing

    1. Pick a framework
        - Mocha (X)
        - Jasmine
        - Tape
        - QUnit
        - AVA
        - Jest (React)

    2. Assertion Library
        Declare what you expect
        - Chai (X)

    3. Helper Libraries
        * JSDOM (X)
            - Simulates the browser's DOM
            - Rum DOM-related tests withput a browser
        * Cheerio
            - jQuery for the server
            - Query virtual DOM using jQuery selectors        

    4. Where to run tests
        * In Browser
        * Headless Browser
            - PhantomJS (run javascript without UI)
        * In-memory DOM (X)
            - JSDOM

    5. Where to place tests
        * Centralized all tests
            - All test in a folder 'tests'
            - Less noise in src folder

        * Alongside (X)
            - Easy imports
            - Clear visibility
            - Convenient to open
            - No recreating fodler structure
            - Easy file moves 

    6. When should run tests    
        - Unit tests => Run upon save

## Continuos Integration (CI)

    - Run utomate build (builds apps automatically)
    - Run test suite
    - Check code coverage
    - Automate deployment
     