# api documentation for  [firebase-tools (v3.6.0)](https://github.com/firebase/firebase-tools)  [![npm package](https://img.shields.io/npm/v/npmdoc-firebase-tools.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-firebase-tools) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-firebase-tools.svg)](https://travis-ci.org/npmdoc/node-npmdoc-firebase-tools)
#### Command-Line Interface for Firebase

[![NPM](https://nodei.co/npm/firebase-tools.png?downloads=true)](https://www.npmjs.com/package/firebase-tools)

[![apidoc](https://npmdoc.github.io/node-npmdoc-firebase-tools/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-firebase-tools_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-firebase-tools/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-firebase-tools/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-firebase-tools/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Firebase",
        "url": "https://firebase.google.com/"
    },
    "bin": {
        "firebase": "./bin/firebase"
    },
    "bugs": {
        "url": "https://github.com/firebase/firebase-tools/issues"
    },
    "dependencies": {
        "JSONStream": "^1.2.1",
        "archiver": "^0.16.0",
        "chalk": "^1.1.0",
        "cjson": "^0.3.1",
        "cli-table": "^0.3.1",
        "commander": "^2.8.1",
        "configstore": "^1.2.0",
        "cross-spawn": "^4.0.0",
        "csv-streamify": "^3.0.4",
        "didyoumean": "^1.2.1",
        "es6-set": "^0.1.4",
        "exit-code": "^1.0.2",
        "filesize": "^3.1.3",
        "firebase": "2.x.x",
        "fs-extra": "^0.23.1",
        "fstream-ignore": "^1.0.2",
        "inquirer": "^0.12.0",
        "jsonschema": "^1.0.2",
        "jsonwebtoken": "^5.4.0",
        "lodash": "^4.6.1",
        "open": "^0.0.5",
        "ora": "0.2.3",
        "portfinder": "^0.4.0",
        "progress": "^1.1.8",
        "request": "^2.58.0",
        "rsvp": "^3.0.18",
        "semver": "^5.0.3",
        "superstatic": "^4.0",
        "tar": "^2.2.0",
        "tmp": "0.0.27",
        "universal-analytics": "^0.3.9",
        "update-notifier": "^0.5.0",
        "user-home": "^2.0.0",
        "uuid": "^3.0.0",
        "winston": "^1.0.1"
    },
    "description": "Command-Line Interface for Firebase",
    "devDependencies": {
        "chai": "^3.0.0",
        "chai-as-promised": "^5.1.0",
        "coveralls": "2.11.2",
        "eslint": "^1.4.1",
        "gulp": "^3.9.0",
        "gulp-eslint": "^1.0.0",
        "gulp-exit": "0.0.2",
        "gulp-istanbul": "^0.10.0",
        "gulp-mocha": "^2.1.2",
        "jshint-stylish": "^2.0.1",
        "nock": "^2.10.0",
        "sinon": "^1.17.4",
        "sinon-as-promised": "^4.0.0",
        "sinon-chai": "^2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0f12d2024c7353d8f35d338072885ea7e3cafce0",
        "tarball": "https://registry.npmjs.org/firebase-tools/-/firebase-tools-3.6.0.tgz"
    },
    "engine-strict": true,
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "bin/**",
        "lib/**",
        "commands/**",
        "templates/**",
        "index.js"
    ],
    "gitHead": "bfc9eda82ee37ba8d0f82a86f6d4d4c5d33dfb49",
    "homepage": "https://github.com/firebase/firebase-tools",
    "keywords": [
        "cdn",
        "cli",
        "ssl",
        "cloud",
        "hosting",
        "firebase",
        "realtime",
        "websockets",
        "synchronization"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "firebase",
            "email": "operations@firebase.com"
        }
    ],
    "name": "firebase-tools",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/firebase/firebase-tools.git"
    },
    "scripts": {
        "test": "gulp"
    },
    "version": "3.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module firebase-tools](#apidoc.module.firebase-tools)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>cli.Command (name)](#apidoc.element.firebase-tools.cli.Command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>cli.Option (flags, description)](#apidoc.element.firebase-tools.cli.Option)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>command (cmd)](#apidoc.element.firebase-tools.command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>config (src, options)](#apidoc.element.firebase-tools.config)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>deploy ()](#apidoc.element.firebase-tools.deploy)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>errorOut (error, status)](#apidoc.element.firebase-tools.errorOut)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>getCommand (name)](#apidoc.element.firebase-tools.getCommand)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>help ()](#apidoc.element.firebase-tools.help)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>init ()](#apidoc.element.firebase-tools.init)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>list ()](#apidoc.element.firebase-tools.list)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>login ()](#apidoc.element.firebase-tools.login)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>logout ()](#apidoc.element.firebase-tools.logout)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>open ()](#apidoc.element.firebase-tools.open)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>prompt (options, questions)](#apidoc.element.firebase-tools.prompt)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>serve ()](#apidoc.element.firebase-tools.serve)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>use ()](#apidoc.element.firebase-tools.use)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>validator (url)](#apidoc.element.firebase-tools.validator)
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>accountExporter
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>accountImporter
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>api
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>auth
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>auth_export
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>auth_import
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>cli
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>cli.Command.prototype
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>cli.Option.prototype
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>cli._events
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>command.prototype
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>config.prototype
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_get
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_profile
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_push
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_remove
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_set
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>database_update
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>ensureApiEnabled
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>fsutils
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions.config
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functionsConfig
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions_config_clone
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions_config_get
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions_config_legacy
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions_config_set
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>functions_config_unset
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>hosting
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>hosting_disable
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>logger
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>login_ci
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>setup
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>setup_web
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>tools
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>tools_migrate
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>utils
1.  object <span class="apidocSignatureSpan">firebase-tools.</span>validator.prototype

#### [module firebase-tools.accountExporter](#apidoc.module.firebase-tools.accountExporter)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountExporter.</span>serialExportUsers (projectId, options)](#apidoc.element.firebase-tools.accountExporter.serialExportUsers)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountExporter.</span>validateOptions (options, fileName)](#apidoc.element.firebase-tools.accountExporter.validateOptions)

#### [module firebase-tools.accountImporter](#apidoc.module.firebase-tools.accountImporter)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>serialImportUsers (projectId, hashOptions, userListArr, index)](#apidoc.element.firebase-tools.accountImporter.serialImportUsers)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>transArrayToUser (arr)](#apidoc.element.firebase-tools.accountImporter.transArrayToUser)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>validateOptions (options)](#apidoc.element.firebase-tools.accountImporter.validateOptions)
1.  [function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>validateUserJson (userJson)](#apidoc.element.firebase-tools.accountImporter.validateUserJson)

#### [module firebase-tools.api](#apidoc.module.firebase-tools.api)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>addRequestHeaders (reqOptions)](#apidoc.element.firebase-tools.api.addRequestHeaders)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>getAccessToken ()](#apidoc.element.firebase-tools.api.getAccessToken)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>getProject (projectId)](#apidoc.element.firebase-tools.api.getProject)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>getProjects ()](#apidoc.element.firebase-tools.api.getProjects)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>request (method, resource, options)](#apidoc.element.firebase-tools.api.request)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>setScopes (s)](#apidoc.element.firebase-tools.api.setScopes)
1.  [function <span class="apidocSignatureSpan">firebase-tools.api.</span>setToken (token)](#apidoc.element.firebase-tools.api.setToken)
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>adminOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>apikeysOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>appengineOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>authOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>clientId
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>clientSecret
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>cloudloggingOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>consoleOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>deployOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>firedataOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>functionsOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>googleOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>hostingOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>realtimeOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>resourceManagerOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>rulesOrigin
1.  string <span class="apidocSignatureSpan">firebase-tools.api.</span>runtimeconfigOrigin

#### [module firebase-tools.auth](#apidoc.module.firebase-tools.auth)
1.  [function <span class="apidocSignatureSpan">firebase-tools.auth.</span>export ()](#apidoc.element.firebase-tools.auth.export)
1.  [function <span class="apidocSignatureSpan">firebase-tools.auth.</span>upload ()](#apidoc.element.firebase-tools.auth.upload)

#### [module firebase-tools.auth_export](#apidoc.module.firebase-tools.auth_export)
1.  [function <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_action (dataFile, options)](#apidoc.element.firebase-tools.auth_export._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_name

#### [module firebase-tools.auth_import](#apidoc.module.firebase-tools.auth_import)
1.  [function <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_action (dataFile, options)](#apidoc.element.firebase-tools.auth_import._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_name

#### [module firebase-tools.cli](#apidoc.module.firebase-tools.cli)
1.  boolean <span class="apidocSignatureSpan">firebase-tools.cli.</span>_allowUnknownOption
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Command (name)](#apidoc.element.firebase-tools.cli.Command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Option (flags, description)](#apidoc.element.firebase-tools.cli.Option)
1.  number <span class="apidocSignatureSpan">firebase-tools.cli.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">firebase-tools.cli.</span>_args
1.  object <span class="apidocSignatureSpan">firebase-tools.cli.</span>_events
1.  object <span class="apidocSignatureSpan">firebase-tools.cli.</span>_execs
1.  object <span class="apidocSignatureSpan">firebase-tools.cli.</span>commands
1.  object <span class="apidocSignatureSpan">firebase-tools.cli.</span>options
1.  string <span class="apidocSignatureSpan">firebase-tools.cli.</span>_name
1.  string <span class="apidocSignatureSpan">firebase-tools.cli.</span>_version

#### [module firebase-tools.cli.Command](#apidoc.module.firebase-tools.cli.Command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Command (name)](#apidoc.element.firebase-tools.cli.Command.Command)

#### [module firebase-tools.cli.Command.prototype](#apidoc.module.firebase-tools.cli.Command.prototype)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>action (fn)](#apidoc.element.firebase-tools.cli.Command.prototype.action)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>addImplicitHelpCommand ()](#apidoc.element.firebase-tools.cli.Command.prototype.addImplicitHelpCommand)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>alias (alias)](#apidoc.element.firebase-tools.cli.Command.prototype.alias)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>allowUnknownOption (arg)](#apidoc.element.firebase-tools.cli.Command.prototype.allowUnknownOption)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>arguments (desc)](#apidoc.element.firebase-tools.cli.Command.prototype.arguments)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>command (name, desc, opts)](#apidoc.element.firebase-tools.cli.Command.prototype.command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>commandHelp ()](#apidoc.element.firebase-tools.cli.Command.prototype.commandHelp)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>description (str)](#apidoc.element.firebase-tools.cli.Command.prototype.description)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>executeSubCommand (argv, args, unknown)](#apidoc.element.firebase-tools.cli.Command.prototype.executeSubCommand)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>help (cb)](#apidoc.element.firebase-tools.cli.Command.prototype.help)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>helpInformation ()](#apidoc.element.firebase-tools.cli.Command.prototype.helpInformation)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>largestOptionLength ()](#apidoc.element.firebase-tools.cli.Command.prototype.largestOptionLength)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>missingArgument (name)](#apidoc.element.firebase-tools.cli.Command.prototype.missingArgument)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>name ()](#apidoc.element.firebase-tools.cli.Command.prototype.name)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>normalize (args)](#apidoc.element.firebase-tools.cli.Command.prototype.normalize)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>option (flags, description, fn, defaultValue)](#apidoc.element.firebase-tools.cli.Command.prototype.option)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionFor (arg)](#apidoc.element.firebase-tools.cli.Command.prototype.optionFor)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionHelp ()](#apidoc.element.firebase-tools.cli.Command.prototype.optionHelp)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionMissingArgument (option, flag)](#apidoc.element.firebase-tools.cli.Command.prototype.optionMissingArgument)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>opts ()](#apidoc.element.firebase-tools.cli.Command.prototype.opts)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>outputHelp (cb)](#apidoc.element.firebase-tools.cli.Command.prototype.outputHelp)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parse (argv)](#apidoc.element.firebase-tools.cli.Command.prototype.parse)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseArgs (args, unknown)](#apidoc.element.firebase-tools.cli.Command.prototype.parseArgs)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseExpectedArgs (args)](#apidoc.element.firebase-tools.cli.Command.prototype.parseExpectedArgs)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseOptions (argv)](#apidoc.element.firebase-tools.cli.Command.prototype.parseOptions)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>unknownOption (flag)](#apidoc.element.firebase-tools.cli.Command.prototype.unknownOption)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>usage (str)](#apidoc.element.firebase-tools.cli.Command.prototype.usage)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>variadicArgNotLast (name)](#apidoc.element.firebase-tools.cli.Command.prototype.variadicArgNotLast)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>version (str, flags)](#apidoc.element.firebase-tools.cli.Command.prototype.version)

#### [module firebase-tools.cli.Option](#apidoc.module.firebase-tools.cli.Option)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Option (flags, description)](#apidoc.element.firebase-tools.cli.Option.Option)

#### [module firebase-tools.cli.Option.prototype](#apidoc.module.firebase-tools.cli.Option.prototype)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Option.prototype.</span>is (arg)](#apidoc.element.firebase-tools.cli.Option.prototype.is)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli.Option.prototype.</span>name ()](#apidoc.element.firebase-tools.cli.Option.prototype.name)

#### [module firebase-tools.cli._events](#apidoc.module.firebase-tools.cli._events)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>debug (val)](#apidoc.element.firebase-tools.cli._events.debug)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>deploy (args, unknown)](#apidoc.element.firebase-tools.cli._events.deploy)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>help (args, unknown)](#apidoc.element.firebase-tools.cli._events.help)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>init (args, unknown)](#apidoc.element.firebase-tools.cli._events.init)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>interactive (val)](#apidoc.element.firebase-tools.cli._events.interactive)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>json (val)](#apidoc.element.firebase-tools.cli._events.json)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>list (args, unknown)](#apidoc.element.firebase-tools.cli._events.list)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>login (args, unknown)](#apidoc.element.firebase-tools.cli._events.login)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>logout (args, unknown)](#apidoc.element.firebase-tools.cli._events.logout)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>non-interactive (val)](#apidoc.element.firebase-tools.cli._events.non-interactive)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>open (args, unknown)](#apidoc.element.firebase-tools.cli._events.open)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>project (val)](#apidoc.element.firebase-tools.cli._events.project)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>serve (args, unknown)](#apidoc.element.firebase-tools.cli._events.serve)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>token (val)](#apidoc.element.firebase-tools.cli._events.token)
1.  [function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>use (args, unknown)](#apidoc.element.firebase-tools.cli._events.use)
1.  object <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>version

#### [module firebase-tools.command](#apidoc.module.firebase-tools.command)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>command (cmd)](#apidoc.element.firebase-tools.command.command)

#### [module firebase-tools.command.prototype](#apidoc.module.firebase-tools.command.prototype)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>_prepare (options)](#apidoc.element.firebase-tools.command.prototype._prepare)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>action (fn)](#apidoc.element.firebase-tools.command.prototype.action)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>applyRC (options)](#apidoc.element.firebase-tools.command.prototype.applyRC)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>before (fn, args)](#apidoc.element.firebase-tools.command.prototype.before)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>description (description)](#apidoc.element.firebase-tools.command.prototype.description)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>option ()](#apidoc.element.firebase-tools.command.prototype.option)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>register (client)](#apidoc.element.firebase-tools.command.prototype.register)
1.  [function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>runner ()](#apidoc.element.firebase-tools.command.prototype.runner)

#### [module firebase-tools.config](#apidoc.module.firebase-tools.config)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>config (src, options)](#apidoc.element.firebase-tools.config.config)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.</span>load (options, allowMissing)](#apidoc.element.firebase-tools.config.load)
1.  object <span class="apidocSignatureSpan">firebase-tools.config.</span>LEGACY_HOSTING_KEYS
1.  object <span class="apidocSignatureSpan">firebase-tools.config.</span>MATERIALIZE_TARGETS
1.  string <span class="apidocSignatureSpan">firebase-tools.config.</span>FILENAME

#### [module firebase-tools.config.prototype](#apidoc.module.firebase-tools.config.prototype)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_hasDeepKey (obj, key)](#apidoc.element.firebase-tools.config.prototype._hasDeepKey)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_materialize (target)](#apidoc.element.firebase-tools.config.prototype._materialize)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_parseFile (target, filePath)](#apidoc.element.firebase-tools.config.prototype._parseFile)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>askWriteProjectFile (p, content)](#apidoc.element.firebase-tools.config.prototype.askWriteProjectFile)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>get (key, fallback)](#apidoc.element.firebase-tools.config.prototype.get)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>has (key)](#apidoc.element.firebase-tools.config.prototype.has)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>importLegacyHostingKeys ()](#apidoc.element.firebase-tools.config.prototype.importLegacyHostingKeys)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>path (pathName)](#apidoc.element.firebase-tools.config.prototype.path)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>readProjectFile (p, options)](#apidoc.element.firebase-tools.config.prototype.readProjectFile)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>set (key, value)](#apidoc.element.firebase-tools.config.prototype.set)
1.  [function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>writeProjectFile (p, content)](#apidoc.element.firebase-tools.config.prototype.writeProjectFile)

#### [module firebase-tools.database](#apidoc.module.firebase-tools.database)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>get ()](#apidoc.element.firebase-tools.database.get)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>profile ()](#apidoc.element.firebase-tools.database.profile)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>push ()](#apidoc.element.firebase-tools.database.push)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>remove ()](#apidoc.element.firebase-tools.database.remove)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>set ()](#apidoc.element.firebase-tools.database.set)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database.</span>update ()](#apidoc.element.firebase-tools.database.update)

#### [module firebase-tools.database_get](#apidoc.module.firebase-tools.database_get)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_action (path, options)](#apidoc.element.firebase-tools.database_get._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_get.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_name

#### [module firebase-tools.database_profile](#apidoc.module.firebase-tools.database_profile)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_action (options)](#apidoc.element.firebase-tools.database_profile._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_name

#### [module firebase-tools.database_push](#apidoc.module.firebase-tools.database_push)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_push._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_push.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_name

#### [module firebase-tools.database_remove](#apidoc.module.firebase-tools.database_remove)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_action (path, options)](#apidoc.element.firebase-tools.database_remove._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_name

#### [module firebase-tools.database_set](#apidoc.module.firebase-tools.database_set)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_set._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_set.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_name

#### [module firebase-tools.database_update](#apidoc.module.firebase-tools.database_update)
1.  [function <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_update._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.database_update.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_name

#### [module firebase-tools.deploy](#apidoc.module.firebase-tools.deploy)
1.  [function <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_action (options)](#apidoc.element.firebase-tools.deploy._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.deploy.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_name

#### [module firebase-tools.ensureApiEnabled](#apidoc.module.firebase-tools.ensureApiEnabled)
1.  [function <span class="apidocSignatureSpan">firebase-tools.ensureApiEnabled.</span>enable (projectId, apiName)](#apidoc.element.firebase-tools.ensureApiEnabled.enable)
1.  [function <span class="apidocSignatureSpan">firebase-tools.ensureApiEnabled.</span>ensure (projectId, apiName, prefix)](#apidoc.element.firebase-tools.ensureApiEnabled.ensure)

#### [module firebase-tools.fsutils](#apidoc.module.firebase-tools.fsutils)
1.  [function <span class="apidocSignatureSpan">firebase-tools.fsutils.</span>dirExistsSync (path)](#apidoc.element.firebase-tools.fsutils.dirExistsSync)
1.  [function <span class="apidocSignatureSpan">firebase-tools.fsutils.</span>fileExistsSync (path)](#apidoc.element.firebase-tools.fsutils.fileExistsSync)

#### [module firebase-tools.functions](#apidoc.module.firebase-tools.functions)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions.</span>log ()](#apidoc.element.firebase-tools.functions.log)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions.</span>config

#### [module firebase-tools.functions.config](#apidoc.module.firebase-tools.functions.config)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>clone ()](#apidoc.element.firebase-tools.functions.config.clone)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>get ()](#apidoc.element.firebase-tools.functions.config.get)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>set ()](#apidoc.element.firebase-tools.functions.config.set)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>unset ()](#apidoc.element.firebase-tools.functions.config.unset)

#### [module firebase-tools.functionsConfig](#apidoc.module.firebase-tools.functionsConfig)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>ensureApi (options)](#apidoc.element.firebase-tools.functionsConfig.ensureApi)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>getFirebaseConfig (projectId, instance)](#apidoc.element.firebase-tools.functionsConfig.getFirebaseConfig)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>idsToVarName (projectId, configId, varId)](#apidoc.element.firebase-tools.functionsConfig.idsToVarName)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>materializeAll (projectId)](#apidoc.element.firebase-tools.functionsConfig.materializeAll)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>materializeConfig (configName, output)](#apidoc.element.firebase-tools.functionsConfig.materializeConfig)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>parseSetArgs (args)](#apidoc.element.firebase-tools.functionsConfig.parseSetArgs)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>parseUnsetArgs (args)](#apidoc.element.firebase-tools.functionsConfig.parseUnsetArgs)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>setVariablesRecursive (projectId, configId, varPath, val)](#apidoc.element.firebase-tools.functionsConfig.setVariablesRecursive)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>varNameToIds (varName)](#apidoc.element.firebase-tools.functionsConfig.varNameToIds)
1.  object <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>RESERVED_NAMESPACES

#### [module firebase-tools.functions_config_clone](#apidoc.module.firebase-tools.functions_config_clone)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_action (options)](#apidoc.element.firebase-tools.functions_config_clone._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_name

#### [module firebase-tools.functions_config_get](#apidoc.module.firebase-tools.functions_config_get)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_action (path, options)](#apidoc.element.firebase-tools.functions_config_get._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_name

#### [module firebase-tools.functions_config_legacy](#apidoc.module.firebase-tools.functions_config_legacy)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_action (options)](#apidoc.element.firebase-tools.functions_config_legacy._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_options
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_name

#### [module firebase-tools.functions_config_set](#apidoc.module.firebase-tools.functions_config_set)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_action (args, options)](#apidoc.element.firebase-tools.functions_config_set._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_name

#### [module firebase-tools.functions_config_unset](#apidoc.module.firebase-tools.functions_config_unset)
1.  [function <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_action (args, options)](#apidoc.element.firebase-tools.functions_config_unset._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_name

#### [module firebase-tools.help](#apidoc.module.firebase-tools.help)
1.  [function <span class="apidocSignatureSpan">firebase-tools.help.</span>_action (commandName)](#apidoc.element.firebase-tools.help._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.help.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.help.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.help.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.help.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.help.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.help.</span>_name

#### [module firebase-tools.hosting](#apidoc.module.firebase-tools.hosting)
1.  [function <span class="apidocSignatureSpan">firebase-tools.hosting.</span>disable ()](#apidoc.element.firebase-tools.hosting.disable)

#### [module firebase-tools.hosting_disable](#apidoc.module.firebase-tools.hosting_disable)
1.  [function <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_action (options)](#apidoc.element.firebase-tools.hosting_disable._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_name

#### [module firebase-tools.init](#apidoc.module.firebase-tools.init)
1.  [function <span class="apidocSignatureSpan">firebase-tools.init.</span>_action (feature, options)](#apidoc.element.firebase-tools.init._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.init.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.init.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.init.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.init.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.init.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.init.</span>_name

#### [module firebase-tools.list](#apidoc.module.firebase-tools.list)
1.  [function <span class="apidocSignatureSpan">firebase-tools.list.</span>_action (options)](#apidoc.element.firebase-tools.list._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.list.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.list.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.list.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.list.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.list.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.list.</span>_name

#### [module firebase-tools.logger](#apidoc.module.firebase-tools.logger)
1.  boolean <span class="apidocSignatureSpan">firebase-tools.logger.</span>emitErrs
1.  boolean <span class="apidocSignatureSpan">firebase-tools.logger.</span>exitOnError
1.  boolean <span class="apidocSignatureSpan">firebase-tools.logger.</span>padLevels
1.  boolean <span class="apidocSignatureSpan">firebase-tools.logger.</span>stripColors
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>debug (msg)](#apidoc.element.firebase-tools.logger.debug)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>error (msg)](#apidoc.element.firebase-tools.logger.error)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>info (msg)](#apidoc.element.firebase-tools.logger.info)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>log ()](#apidoc.element.firebase-tools.logger.log)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>silly (msg)](#apidoc.element.firebase-tools.logger.silly)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>verbose (msg)](#apidoc.element.firebase-tools.logger.verbose)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logger.</span>warn (msg)](#apidoc.element.firebase-tools.logger.warn)
1.  number <span class="apidocSignatureSpan">firebase-tools.logger.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>_events
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>_hnames
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>_names
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>domain
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>exceptionHandlers
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>filters
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>levels
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>profilers
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>rewriters
1.  object <span class="apidocSignatureSpan">firebase-tools.logger.</span>transports
1.  string <span class="apidocSignatureSpan">firebase-tools.logger.</span>level

#### [module firebase-tools.login](#apidoc.module.firebase-tools.login)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>login ()](#apidoc.element.firebase-tools.login.login)
1.  [function <span class="apidocSignatureSpan">firebase-tools.login.</span>ci ()](#apidoc.element.firebase-tools.login.ci)

#### [module firebase-tools.login_ci](#apidoc.module.firebase-tools.login_ci)
1.  [function <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_action (options)](#apidoc.element.firebase-tools.login_ci._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_name

#### [module firebase-tools.logout](#apidoc.module.firebase-tools.logout)
1.  [function <span class="apidocSignatureSpan">firebase-tools.logout.</span>_action (options)](#apidoc.element.firebase-tools.logout._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.logout.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.logout.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.logout.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.logout.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.logout.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.logout.</span>_name

#### [module firebase-tools.open](#apidoc.module.firebase-tools.open)
1.  [function <span class="apidocSignatureSpan">firebase-tools.open.</span>_action (linkName, options)](#apidoc.element.firebase-tools.open._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.open.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.open.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.open.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.open.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.open.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.open.</span>_name

#### [module firebase-tools.prompt](#apidoc.module.firebase-tools.prompt)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>prompt (options, questions)](#apidoc.element.firebase-tools.prompt.prompt)
1.  [function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>convertLabeledListChoices (choices)](#apidoc.element.firebase-tools.prompt.convertLabeledListChoices)
1.  [function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>listLabelToValue (label, choices)](#apidoc.element.firebase-tools.prompt.listLabelToValue)
1.  [function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>once (question)](#apidoc.element.firebase-tools.prompt.once)

#### [module firebase-tools.serve](#apidoc.module.firebase-tools.serve)
1.  [function <span class="apidocSignatureSpan">firebase-tools.serve.</span>_action (options)](#apidoc.element.firebase-tools.serve._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.serve.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.serve.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.serve.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.serve.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.serve.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.serve.</span>_name

#### [module firebase-tools.setup](#apidoc.module.firebase-tools.setup)
1.  [function <span class="apidocSignatureSpan">firebase-tools.setup.</span>web ()](#apidoc.element.firebase-tools.setup.web)

#### [module firebase-tools.setup_web](#apidoc.module.firebase-tools.setup_web)
1.  [function <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_action (options)](#apidoc.element.firebase-tools.setup_web._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_name

#### [module firebase-tools.tools](#apidoc.module.firebase-tools.tools)
1.  [function <span class="apidocSignatureSpan">firebase-tools.tools.</span>migrate ()](#apidoc.element.firebase-tools.tools.migrate)

#### [module firebase-tools.tools_migrate](#apidoc.module.firebase-tools.tools_migrate)
1.  [function <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_action (options)](#apidoc.element.firebase-tools.tools_migrate._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_name

#### [module firebase-tools.use](#apidoc.module.firebase-tools.use)
1.  [function <span class="apidocSignatureSpan">firebase-tools.use.</span>_action (newActive, options)](#apidoc.element.firebase-tools.use._action)
1.  object <span class="apidocSignatureSpan">firebase-tools.use.</span>_befores
1.  object <span class="apidocSignatureSpan">firebase-tools.use.</span>_options
1.  object <span class="apidocSignatureSpan">firebase-tools.use.</span>client
1.  string <span class="apidocSignatureSpan">firebase-tools.use.</span>_cmd
1.  string <span class="apidocSignatureSpan">firebase-tools.use.</span>_description
1.  string <span class="apidocSignatureSpan">firebase-tools.use.</span>_name

#### [module firebase-tools.utils](#apidoc.module.firebase-tools.utils)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>addSubdomain (origin, subdomain)](#apidoc.element.firebase-tools.utils.addSubdomain)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>consoleUrl (project, path)](#apidoc.element.firebase-tools.utils.consoleUrl)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>endpoint (parts)](#apidoc.element.firebase-tools.utils.endpoint)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>envOverride (envname, value, coerce)](#apidoc.element.firebase-tools.utils.envOverride)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>explainStdin ()](#apidoc.element.firebase-tools.utils.explainStdin)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>getInheritedOption (options, key)](#apidoc.element.firebase-tools.utils.getInheritedOption)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logBullet (message, type)](#apidoc.element.firebase-tools.utils.logBullet)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logSuccess (message, type)](#apidoc.element.firebase-tools.utils.logSuccess)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logWarning (message, type)](#apidoc.element.firebase-tools.utils.logWarning)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>makeActiveProject (projectDir, newActive)](#apidoc.element.firebase-tools.utils.makeActiveProject)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>reject (message, options)](#apidoc.element.firebase-tools.utils.reject)
1.  [function <span class="apidocSignatureSpan">firebase-tools.utils.</span>stringToStream (text)](#apidoc.element.firebase-tools.utils.stringToStream)

#### [module firebase-tools.validator](#apidoc.module.firebase-tools.validator)
1.  [function <span class="apidocSignatureSpan">firebase-tools.</span>validator (url)](#apidoc.element.firebase-tools.validator.validator)
1.  object <span class="apidocSignatureSpan">firebase-tools.validator.</span>firebase

#### [module firebase-tools.validator.prototype](#apidoc.module.firebase-tools.validator.prototype)
1.  [function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>_decorateErrors (errors)](#apidoc.element.firebase-tools.validator.prototype._decorateErrors)
1.  [function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>_process ()](#apidoc.element.firebase-tools.validator.prototype._process)
1.  [function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>validate (data)](#apidoc.element.firebase-tools.validator.prototype.validate)



# <a name="apidoc.module.firebase-tools"></a>[module firebase-tools](#apidoc.module.firebase-tools)

#### <a name="apidoc.element.firebase-tools.cli.Command"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>cli.Command (name)](#apidoc.element.firebase-tools.cli.Command)
- description and source-code
```javascript
function Command(name) {
  this.commands = [];
  this.options = [];
  this._execs = {};
  this._allowUnknownOption = false;
  this._args = [];
  this._name = name || '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Option"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>cli.Option (flags, description)](#apidoc.element.firebase-tools.cli.Option)
- description and source-code
```javascript
function Option(flags, description) {
  this.flags = flags;
  this.required = ~flags.indexOf('<');
  this.optional = ~flags.indexOf('[');
  this.bool = !~flags.indexOf('-no-');
  flags = flags.split(/[ ,|]+/);
  if (flags.length > 1 && !/^[[<]/.test(flags[1])) this.short = flags.shift();
  this.long = flags.shift();
  this.description = description || '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.command"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>command (cmd)](#apidoc.element.firebase-tools.command)
- description and source-code
```javascript
command = function (cmd) {
  this._cmd = cmd;
  this._name = _.first(cmd.split(' '));
  this._description = null;
  this._options = [];
  this._action = null;
  this._befores = [];
}
```
- example usage
```shell
...
};

// ignoring this in coverage for now since it's just wrapping commander
/* istanbul ignore next */
Command.prototype.register = function(client) {
this.client = client;
var program = client.cli;
var cmd = program.command(this._cmd);
if (this._description) { cmd.description(this._description); }
this._options.forEach(function(args) { cmd.option.apply(cmd, args); });

var self = this;
cmd.action(function() {
  var runner = self.runner();
  var start = new Date().getTime();
...
```

#### <a name="apidoc.element.firebase-tools.config"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>config (src, options)](#apidoc.element.firebase-tools.config)
- description and source-code
```javascript
config = function (src, options) {
  this.options = options || {};
  this.projectDir = options.projectDir || detectProjectRoot(options.cwd);

  this._src = src;
  this.data = {};
  this.defaults = {};
  this.notes = {};

  if (this._src.firebase) {
    this.defaults.project = this._src.firebase;
    utils.logWarning(chalk.bold('"firebase"') + ' key in firebase.json is deprecated. Run ' + chalk.bold('firebase use --add') + '
instead');
  }

  if (_.has(this._src, 'rules')) {
    _.set(this._src, 'database.rules', this._src.rules);
  }

  Config.MATERIALIZE_TARGETS.forEach(function(target) {
    if (_.get(this._src, target)) {
      if (target === 'database.rules') {
        _.set(this.data, 'database.rulesString', this._materialize(target));
      } else {
        _.set(this.data, target, this._materialize(target));
      }
    }
  }, this);

  // auto-detect functions from package.json in directory
  if (this.projectDir && !this.get('functions.source') && fsutils.fileExistsSync(this.path('functions/package.json'))) {
    this.set('functions.source', 'functions');
  }

  // use 'public' as signal for legacy hosting since it's a required key
  if (!this.data.hosting && this._src.public) {
    this.importLegacyHostingKeys();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.deploy"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>deploy ()](#apidoc.element.firebase-tools.deploy)
- description and source-code
```javascript
deploy = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
token: process.env.FIREBASE_TOKEN,
cwd: '/path/to/project/folder'
}).then(function() {
console.log('Rules have been deployed!')
}).catch(function(err) {
// handle error
...
```

#### <a name="apidoc.element.firebase-tools.errorOut"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>errorOut (error, status)](#apidoc.element.firebase-tools.errorOut)
- description and source-code
```javascript
errorOut = function (error, status) {
  require('./lib/errorOut')(client, error, status);
}
```
- example usage
```shell
...
  var self = this;
  cmd.action(function() {
var runner = self.runner();
var start = new Date().getTime();
var options = _.last(_.toArray(arguments));
var argCount = cmd._args.length;
if (arguments.length - 1 > argCount) {
  return client.errorOut(
    new FirebaseError('Too many arguments. Run ' + chalk.bold('firebase help ' + cmd._name) + ' for usage instructions', {exit:
1})
  );
}

runner.apply(self, arguments).then(function(result) {
  if (utils.getInheritedOption(options, 'json')) {
    console.log(JSON.stringify({
...
```

#### <a name="apidoc.element.firebase-tools.getCommand"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>getCommand (name)](#apidoc.element.firebase-tools.getCommand)
- description and source-code
```javascript
getCommand = function (name) {
  for (var i = 0; i < client.cli.commands.length; i++) {
    if (client.cli.commands[i]._name === name) {
      return client.cli.commands[i];
    }
  }
  return null;
}
```
- example usage
```shell
...
var chalk = require('chalk');
var logger = require('../lib/logger');
var utils = require('../lib/utils');

module.exports = new Command('help [command]')
.description('display help information')
.action(function(commandName) {
  var cmd = this.client.getCommand(commandName);
  if (cmd) {
    cmd.outputHelp();
  } else if (commandName) {
    logger.warn();
    utils.logWarning(chalk.bold(commandName) + ' is not a valid command. See below for valid commands');
    this.client.cli.outputHelp();
  } else {
...
```

#### <a name="apidoc.element.firebase-tools.help"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>help ()](#apidoc.element.firebase-tools.help)
- description and source-code
```javascript
help = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.init"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>init ()](#apidoc.element.firebase-tools.init)
- description and source-code
```javascript
init = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.list"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>list ()](#apidoc.element.firebase-tools.list)
- description and source-code
```javascript
list = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...

## Using as a Module

The Firebase CLI can also be used programmatically as a standard Node module. Each command is exposed as a function that takes an
 options object and returns a Promise. For example:

'''js
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
...
```

#### <a name="apidoc.element.firebase-tools.login"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>login ()](#apidoc.element.firebase-tools.login)
- description and source-code
```javascript
login = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
.description('generate an access token for use in non-interactive environments')
.option('--no-localhost', 'copy and paste a code instead of starting a local server for authentication')
.action(function(options) {
  if (options.nonInteractive) {
    return utils.reject('Cannot run login:ci in non-interactive mode.', {exit: 1});
  }

  return auth.login(options.localhost).then(function(result) {
    logger.info();
    utils.logSuccess('Success! Use this token to login on a CI server:\n\n' +
      chalk.bold(result.tokens.refresh_token) + '\n\nExample: firebase deploy --token "$FIREBASE_TOKEN"\n');
    return result;
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.logout"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>logout ()](#apidoc.element.firebase-tools.logout)
- description and source-code
```javascript
logout = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
var user = configstore.get('user');
var tokens = configstore.get('tokens');
var currentToken = _.get(tokens, 'refresh_token');
var token = utils.getInheritedOption(options, 'token') || currentToken;
api.setToken(token);
var next;
if (token) {
  next = auth.logout(token);
} else {
  next = RSVP.resolve();
}

var cleanup = function() {
  if (token || user || tokens) {
    var msg = 'Logged out';
...
```

#### <a name="apidoc.element.firebase-tools.open"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>open ()](#apidoc.element.firebase-tools.open)
- description and source-code
```javascript
open = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.prompt"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>prompt (options, questions)](#apidoc.element.firebase-tools.prompt)
- description and source-code
```javascript
prompt = function (options, questions) {
  return new RSVP.Promise(function(resolve, reject) {
    var prompts = [];
    for (var i = 0; i < questions.length; i++) {
      if (!options[questions[i].name]) {
        prompts.push(questions[i]);
      }
    }

    if (prompts.length && options.nonInteractive) {
      return reject(new FirebaseError('Missing required options (' + _.uniq(_.map(prompts, 'name')).join(', ') + ') while running
 in non-interactive mode', {
        children: prompts,
        exit: 1
      }));
    }

    return inquirer.prompt(prompts, function(answers) {
      _.forEach(answers, function(v, k) {
        options[k] = v;
      });
      return resolve(options);
    });
  });
}
```
- example usage
```shell
...
    if (prompts.length && options.nonInteractive) {
      return reject(new FirebaseError('Missing required options (' + _.uniq(_.map(prompts, 'name')).join(', ') + ') while running
 in non-interactive mode', {
        children: prompts,
        exit: 1
      }));
    }

    return inquirer.prompt(prompts, function(answers) {
      _.forEach(answers, function(v, k) {
        options[k] = v;
      });
      return resolve(options);
    });
  });
};
...
```

#### <a name="apidoc.element.firebase-tools.serve"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>serve ()](#apidoc.element.firebase-tools.serve)
- description and source-code
```javascript
serve = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.use"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>use ()](#apidoc.element.firebase-tools.use)
- description and source-code
```javascript
use = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.validator"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>validator (url)](#apidoc.element.firebase-tools.validator)
- description and source-code
```javascript
validator = function (url) {
  this._validateQueue = [];

  var self = this;
  request.get(url, function(err, response, body) {
    if (!err && response.statusCode === 200) {
      self.schema = JSON.parse(body);
      self._process();
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.accountExporter"></a>[module firebase-tools.accountExporter](#apidoc.module.firebase-tools.accountExporter)

#### <a name="apidoc.element.firebase-tools.accountExporter.serialExportUsers"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountExporter.</span>serialExportUsers (projectId, options)](#apidoc.element.firebase-tools.accountExporter.serialExportUsers)
- description and source-code
```javascript
serialExportUsers = function (projectId, options) {
  var postBody = {
    targetProjectId: projectId,
    maxResults: options.batchSize
  };
  if (options.nextPageToken) {
    postBody.nextPageToken = options.nextPageToken;
  }
  return api.request('POST', '/identitytoolkit/v3/relyingparty/downloadAccount', {
    auth: true,
    json: true,
    data: postBody,
    origin: api.googleOrigin
  }).then(function(ret) {
    var userList = ret.body.users;
    if (userList && userList.length > 0) {
      _writeUsersToFile(userList, options.format, options.writeStream);
      utils.logSuccess('Exported ' + userList.length + ' account(s) successfully.');
      options.nextPageToken = ret.body.nextPageToken;
      return serialExportUsers(projectId, options);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.accountExporter.validateOptions"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountExporter.</span>validateOptions (options, fileName)](#apidoc.element.firebase-tools.accountExporter.validateOptions)
- description and source-code
```javascript
validateOptions = function (options, fileName) {
  var exportOptions = {};
  if (fileName === undefined) {
    return utils.reject('Must specify data file', {exit: 1});
  }
  var extName = path.extname(fileName.toLowerCase());
  if (extName === '.csv') {
    exportOptions.format = 'csv';
  } else if (extName === '.json') {
    exportOptions.format = 'json';
  } else if (options.format) {
    var format = options.format.toLowerCase();
    if (format === 'csv' || format === 'json') {
      exportOptions.format = format;
    } else {
      return utils.reject('Unsupported data file format, should be csv or json', {exit: 1});
    }
  } else {
    return utils.reject('Please specify data file format in file name, or use 'format' parameter', {exit: 1});
  }
  return exportOptions;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.accountImporter"></a>[module firebase-tools.accountImporter](#apidoc.module.firebase-tools.accountImporter)

#### <a name="apidoc.element.firebase-tools.accountImporter.serialImportUsers"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>serialImportUsers (projectId, hashOptions, userListArr, index)](#apidoc.element.firebase-tools.accountImporter.serialImportUsers)
- description and source-code
```javascript
serialImportUsers = function (projectId, hashOptions, userListArr, index) {
  return _sendRequest(projectId, userListArr[index], hashOptions)
      .then(function() {
        if (index < userListArr.length - 1) {
          return serialImportUsers(projectId, hashOptions, userListArr, index + 1);
        }
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.accountImporter.transArrayToUser"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>transArrayToUser (arr)](#apidoc.element.firebase-tools.accountImporter.transArrayToUser)
- description and source-code
```javascript
transArrayToUser = function (arr) {
  var user = {
    localId: arr[0],
    email: arr[1],
    emailVerified: arr[2] === 'true',
    passwordHash: arr[3],
    salt: arr[4],
    displayName: arr[5],
    photoUrl: arr[6],
    createdAt: arr[23],
    lastLoginAt: arr[24],
    providerUserInfo: []
  };
  _addProviderUserInfo(user, 'google.com', arr.slice(7, 11));
  _addProviderUserInfo(user, 'facebook.com', arr.slice(11, 15));
  _addProviderUserInfo(user, 'twitter.com', arr.slice(15, 19));
  _addProviderUserInfo(user, 'github.com', arr.slice(19, 23));
  return user;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.accountImporter.validateOptions"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>validateOptions (options)](#apidoc.element.firebase-tools.accountImporter.validateOptions)
- description and source-code
```javascript
validateOptions = function (options) {
  if (!options.hashAlgo) {
    utils.logWarning('No hash algorithm specified. Password users cannot be imported.');
    return {valid: true};
  }
  var hashAlgo = options.hashAlgo.toUpperCase();
  switch (hashAlgo) {
  case 'HMAC_SHA512':
  case 'HMAC_SHA256':
  case 'HMAC_SHA1':
  case 'HMAC_MD5':
    if (!options.hashKey || options.hashKey === '') {
      return utils.reject('Must provide hash key(base64 encoded) for hash algorithm ' + options.hashAlgo, {exit: 1});
    }
    return {hashAlgo: hashAlgo, hashKey: options.hashKey, valid: true};
  case 'MD5':
  case 'SHA1':
  case 'SHA256':
  case 'PBKDF_SHA1':
  case 'PBKDF2_SHA256':
    var roundsNum = parseInt(options.rounds, 10);
    if (isNaN(roundsNum) || roundsNum < 0 || roundsNum > 30000) {
      return utils.reject('Must provide valid rounds(0..30000) for hash algorithm ' + options.hashAlgo, {exit: 1});
    }
    return {hashAlgo: hashAlgo, rounds: options.rounds, valid: true};
  case 'SCRYPT':
    if (!options.hashKey || options.hashKey === '') {
      return utils.reject('Must provide hash key(base64 encoded) for hash algorithm ' + options.hashAlgo, {exit: 1});
    }
    roundsNum = parseInt(options.rounds, 10);
    if (isNaN(roundsNum) || roundsNum <= 0 || roundsNum > 8) {
      return utils.reject('Must provide valid rounds(1..8) for hash algorithm ' + options.hashAlgo, {exit: 1});
    }
    var memCost = parseInt(options.memCost, 10);
    if (isNaN(memCost) || memCost <= 0 || memCost > 14) {
      return utils.reject('Must provide valid memory cost(1..14) for hash algorithm ' + options.hashAlgo, {exit: 1});
    }
    var saltSeparator = '';
    if (options.saltSeparator) {
      saltSeparator = options.saltSeparator;
    }
    return {
      hashAlgo: hashAlgo,
      hashKey: options.hashKey,
      saltSeparator: saltSeparator,
      rounds: options.rounds,
      memCost: options.memCost,
      valid: true
    };
  case 'BCRYPT':
    return {hashAlgo: hashAlgo, valid: true};
  default:
    return utils.reject('Unsupported hash algorithm ' + chalk.bold(options.hashAlgo));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.accountImporter.validateUserJson"></a>[function <span class="apidocSignatureSpan">firebase-tools.accountImporter.</span>validateUserJson (userJson)](#apidoc.element.firebase-tools.accountImporter.validateUserJson)
- description and source-code
```javascript
validateUserJson = function (userJson) {
  var keydiff = _.difference(_.keys(userJson), ALLOWED_JSON_KEYS);
  if (keydiff.length) {
    return {error: JSON.stringify(userJson, null, 2) + ' has unsupported keys: ' + keydiff.join(',')};
  }
  if (userJson.providerUserInfo) {
    for (var i = 0; i < userJson.providerUserInfo.length; i++) {
      var res = _validateProviderUserInfo(userJson.providerUserInfo[i]);
      if (res.error) {
        return res;
      }
    }
  }
  return {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.api"></a>[module firebase-tools.api](#apidoc.module.firebase-tools.api)

#### <a name="apidoc.element.firebase-tools.api.addRequestHeaders"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>addRequestHeaders (reqOptions)](#apidoc.element.firebase-tools.api.addRequestHeaders)
- description and source-code
```javascript
addRequestHeaders = function (reqOptions) {
// Runtime fetch of Auth singleton to prevent circular module dependencies
  _.set(reqOptions, ['headers', 'User-Agent'], 'FirebaseCLI/' + CLI_VERSION);
  var auth = require('../lib/auth');
  return auth.getAccessToken(refreshToken, commandScopes).then(function(result) {
    _.set(reqOptions, 'headers.authorization', 'Bearer ' + result.access_token);
    return reqOptions;
  });
}
```
- example usage
```shell
...

url += querystring.stringify(query);

var reqOptions = {
  url: url
};

return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
  return new RSVP.Promise(function(resolve, reject) {
    var fileOut = !!options.output;
    var outStream = fileOut ? fs.createWriteStream(options.output) : process.stdout;
    var erroring;
    var errorResponse = '';
    var response;
...
```

#### <a name="apidoc.element.firebase-tools.api.getAccessToken"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>getAccessToken ()](#apidoc.element.firebase-tools.api.getAccessToken)
- description and source-code
```javascript
getAccessToken = function () {
  return require('./auth').getAccessToken(refreshToken, commandScopes);
}
```
- example usage
```shell
...
    scopes.OPENID,
    scopes.CLOUD_PROJECTS_READONLY,
    scopes.FIREBASE_PLATFORM
  ].concat(s || [])));
  logger.debug('> command requires scopes:', JSON.stringify(commandScopes));
},
getAccessToken: function() {
  return require('./auth').getAccessToken(refreshToken, commandScopes);
},
addRequestHeaders: function(reqOptions) {
// Runtime fetch of Auth singleton to prevent circular module dependencies
  _.set(reqOptions, ['headers', 'User-Agent'], 'FirebaseCLI/' + CLI_VERSION);
  var auth = require('../lib/auth');
  return auth.getAccessToken(refreshToken, commandScopes).then(function(result) {
    _.set(reqOptions, 'headers.authorization', 'Bearer ' + result.access_token);
...
```

#### <a name="apidoc.element.firebase-tools.api.getProject"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>getProject (projectId)](#apidoc.element.firebase-tools.api.getProject)
- description and source-code
```javascript
getProject = function (projectId) {
  return api.request('GET', '/v1/projects/' + encodeURIComponent(projectId), {
    auth: true
  }).then(function(res) {
    if (res.body && !res.body.error) {
      return res.body;
    }

    return RSVP.reject(new FirebaseError('Server Error: Unexpected Response. Please try again', {
      context: res,
      exit: 2
    }));
  });
}
```
- example usage
```shell
...
/**
 * Tries to determine the instance ID for the provided
 * project.
 * @param {Object} options The command-line options object
 * @returns {Promise<String>} The instance ID
 */
module.exports = function(options) {
return api.getProject(options.project).then(function(project) {
  if (!_.has(project, ['instances', 'database', 0])) {
    throw new FirebaseError('No instance found for project. Please try a different project.', {
      exit: 1
    });
  }
  return project.instances.database[0];
});
...
```

#### <a name="apidoc.element.firebase-tools.api.getProjects"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>getProjects ()](#apidoc.element.firebase-tools.api.getProjects)
- description and source-code
```javascript
getProjects = function () {
  return api.request('GET', '/v1/projects', {
    auth: true
  }).then(function(res) {
    if (res.body && res.body.projects) {
      return res.body.projects;
    }

    return RSVP.reject(new FirebaseError('Server Error: Unexpected Response. Please try again', {
      context: res,
      exit: 2
    }));
  });
}
```
- example usage
```shell
...
var _ = require('lodash');
var logger = require('../lib/logger');

module.exports = new Command('list')
  .description('list the Firebases to which you have access')
  .before(requireAuth)
  .action(function(options) {
    return api.getProjects().then(function(projects) {
var tableHead = ['Name', 'Project ID / Instance', 'Permissions'];
var table = new Table({
  head: tableHead,
  style: {head: ['yellow']}
});

var out = [];
...
```

#### <a name="apidoc.element.firebase-tools.api.request"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>request (method, resource, options)](#apidoc.element.firebase-tools.api.request)
- description and source-code
```javascript
request = function (method, resource, options) {
  options = _.extend({
    data: {},
    origin: api.adminOrigin, // default to hitting the admin backend
    resolveOnHTTPError: false, // by default, status codes >= 400 leads to reject
    json: true
  }, options);

  var validMethods = ['GET', 'PUT', 'POST', 'DELETE', 'PATCH'];

  if (validMethods.indexOf(method) < 0) {
    method = 'GET';
  }

  var reqOptions = {
    method: method
  };

  if (options.query) {
    resource = _appendQueryData(resource, options.query);
  }

  if (method === 'GET') {
    resource = _appendQueryData(resource, options.data);
  } else {
    if (_.size(options.data) > 0) {
      reqOptions.body = options.data;
    } else if (_.size(options.form) > 0) {
      reqOptions.form = options.form;
    }
  }

  reqOptions.url = options.origin + resource;
  reqOptions.files = options.files;
  reqOptions.resolveOnHTTPError = options.resolveOnHTTPError;
  reqOptions.json = options.json;

  if (options.auth === true) {
    return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
      return _request(reqOptionsWithToken);
    });
  }

  return _request(reqOptions);
}
```
- example usage
```shell
...
  message: 'Are you sure you want to disable Firebase Hosting?\n  ' + chalk.bold.underline('This will immediately make your site
 inaccessible!')
}
    ]).then(function() {
if (!options.confirm) {
  return RSVP.resolve();
}

return api.request('POST', '/v1/projects/' + encodeURIComponent(options.project) + '/releases', {
  auth: true,
  data: {
    hosting: {
      disabled: true
    }
  },
  origin: api.deployOrigin
...
```

#### <a name="apidoc.element.firebase-tools.api.setScopes"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>setScopes (s)](#apidoc.element.firebase-tools.api.setScopes)
- description and source-code
```javascript
setScopes = function (s) {
  commandScopes = _.uniq(_.flatten([
    scopes.EMAIL,
    scopes.OPENID,
    scopes.CLOUD_PROJECTS_READONLY,
    scopes.FIREBASE_PLATFORM
  ].concat(s || [])));
  logger.debug('> command requires scopes:', JSON.stringify(commandScopes));
}
```
- example usage
```shell
...

module.exports = function(options, authScopes) {
var inScopes = authScopes;
if (_.isFunction(authScopes)) {
  inScopes = authScopes(options);
}

api.setScopes(inScopes);
options.authScopes = api.commandScopes;

var tokens = configstore.get('tokens');
var user = configstore.get('user');

var tokenOpt = utils.getInheritedOption(options, 'token');
tokenOpt = tokenOpt || process.env.FIREBASE_TOKEN;
...
```

#### <a name="apidoc.element.firebase-tools.api.setToken"></a>[function <span class="apidocSignatureSpan">firebase-tools.api.</span>setToken (token)](#apidoc.element.firebase-tools.api.setToken)
- description and source-code
```javascript
setToken = function (token) {
  refreshToken = token;
}
```
- example usage
```shell
...
module.exports = new Command('logout')
.description('log the CLI out of Firebase')
.action(function(options) {
  var user = configstore.get('user');
  var tokens = configstore.get('tokens');
  var currentToken = _.get(tokens, 'refresh_token');
  var token = utils.getInheritedOption(options, 'token') || currentToken;
  api.setToken(token);
  var next;
  if (token) {
    next = auth.logout(token);
  } else {
    next = RSVP.resolve();
  }
...
```



# <a name="apidoc.module.firebase-tools.auth"></a>[module firebase-tools.auth](#apidoc.module.firebase-tools.auth)

#### <a name="apidoc.element.firebase-tools.auth.export"></a>[function <span class="apidocSignatureSpan">firebase-tools.auth.</span>export ()](#apidoc.element.firebase-tools.auth.export)
- description and source-code
```javascript
export = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.auth.upload"></a>[function <span class="apidocSignatureSpan">firebase-tools.auth.</span>upload ()](#apidoc.element.firebase-tools.auth.upload)
- description and source-code
```javascript
upload = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.auth_export"></a>[module firebase-tools.auth_export](#apidoc.module.firebase-tools.auth_export)

#### <a name="apidoc.element.firebase-tools.auth_export._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.auth_export.</span>_action (dataFile, options)](#apidoc.element.firebase-tools.auth_export._action)
- description and source-code
```javascript
_action = function (dataFile, options) {
  var projectId = getProjectId(options);
  var checkRes = validateOptions(options, dataFile);
  if (!checkRes.format) {
    return checkRes;
  }
  var exportOptions = checkRes;
  var writeStream = fs.createWriteStream(dataFile);
  if (exportOptions.format === 'json') {
    writeStream.write('{"users": [' + os.EOL);
  }
  exportOptions.writeStream = writeStream;
  exportOptions.batchSize = MAX_BATCH_SIZE;
  logger.info('Exporting accounts to ' + chalk.bold(dataFile));
  return serialExportUsers(projectId, exportOptions).then(function() {
    if (exportOptions.format === 'json') {
      writeStream.write(']}');
    }
    writeStream.end();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.auth_import"></a>[module firebase-tools.auth_import](#apidoc.module.firebase-tools.auth_import)

#### <a name="apidoc.element.firebase-tools.auth_import._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.auth_import.</span>_action (dataFile, options)](#apidoc.element.firebase-tools.auth_import._action)
- description and source-code
```javascript
_action = function (dataFile, options) {
  var projectId = getProjectId(options);
  var checkRes = validateOptions(options);
  if (!checkRes.valid) {
    return checkRes;
  }
  var hashOptions = checkRes;

  if (!_.endsWith(dataFile, '.csv') && !_.endsWith(dataFile, '.json')) {
    return utils.reject('Data file must end with .csv or .json', {exit: 1});
  }
  var stats = fs.statSync(dataFile);
  var fileSizeInBytes = stats.size;
  logger.info('Processing ' + chalk.bold(dataFile) + ' (' + fileSizeInBytes + ' bytes)');

  var inStream = fs.createReadStream(dataFile);
  var batches = [];
  var currentBatch = [];
  return new RSVP.Promise(function(resolve, reject) {
    var parser;
    var counter = 0;
    if (dataFile.endsWith('.csv')) {
      parser = csv({objectMode: true});
      parser.on('data', function(line) {
        counter++;
        var user = transArrayToUser(line.map(
          function(str) {
            // Ignore starting '|'' and trailing '|''
            var newStr = str.trim().replace(/^["|'](.*)["|']$/, '$1');
            return newStr === '' ? undefined : newStr;
          }));
        currentBatch.push(user);
        if (currentBatch.length === MAX_BATCH_SIZE) {
          batches.push(currentBatch);
          currentBatch = [];
        }
      }).on('end', function() {
        if (currentBatch.length) {
          batches.push(currentBatch);
        }
        return resolve(batches);
      });
      inStream.pipe(parser);
    } else {
      parser = jsonStream.parse(['users', {emitKey: true}]);
      parser.on('data', function(pair) {
        counter++;
        var res = validateUserJson(pair.value);
        if (res.error) {
          return reject(res.error);
        }
        currentBatch.push(pair.value);
        if (currentBatch.length === MAX_BATCH_SIZE) {
          batches.push(currentBatch);
          currentBatch = [];
        }
      }).on('end', function() {
        if (currentBatch.length) {
          batches.push(currentBatch);
        }
        return resolve(batches);
      });
      inStream.pipe(parser);
    }
  }).then(function(userListArr) {
    if (userListArr.length) {
      return serialImportUsers(projectId, hashOptions, userListArr, 0);
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.cli"></a>[module firebase-tools.cli](#apidoc.module.firebase-tools.cli)

#### <a name="apidoc.element.firebase-tools.cli.Command"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Command (name)](#apidoc.element.firebase-tools.cli.Command)
- description and source-code
```javascript
function Command(name) {
  this.commands = [];
  this.options = [];
  this._execs = {};
  this._allowUnknownOption = false;
  this._args = [];
  this._name = name || '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Option"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Option (flags, description)](#apidoc.element.firebase-tools.cli.Option)
- description and source-code
```javascript
function Option(flags, description) {
  this.flags = flags;
  this.required = ~flags.indexOf('<');
  this.optional = ~flags.indexOf('[');
  this.bool = !~flags.indexOf('-no-');
  flags = flags.split(/[ ,|]+/);
  if (flags.length > 1 && !/^[[<]/.test(flags[1])) this.short = flags.shift();
  this.long = flags.shift();
  this.description = description || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.cli.Command"></a>[module firebase-tools.cli.Command](#apidoc.module.firebase-tools.cli.Command)

#### <a name="apidoc.element.firebase-tools.cli.Command.Command"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Command (name)](#apidoc.element.firebase-tools.cli.Command.Command)
- description and source-code
```javascript
function Command(name) {
  this.commands = [];
  this.options = [];
  this._execs = {};
  this._allowUnknownOption = false;
  this._args = [];
  this._name = name || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.cli.Command.prototype"></a>[module firebase-tools.cli.Command.prototype](#apidoc.module.firebase-tools.cli.Command.prototype)

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.action"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>action (fn)](#apidoc.element.firebase-tools.cli.Command.prototype.action)
- description and source-code
```javascript
action = function (fn) {
  var self = this;
  var listener = function(args, unknown) {
    // Parse any so-far unknown options
    args = args || [];
    unknown = unknown || [];

    var parsed = self.parseOptions(unknown);

    // Output help if necessary
    outputHelpIfNecessary(self, parsed.unknown);

    // If there are still any unknown options, then we simply
    // die, unless someone asked for help, in which case we give it
    // to them, and then we die.
    if (parsed.unknown.length > 0) {
      self.unknownOption(parsed.unknown[0]);
    }

    // Leftover arguments need to be pushed back. Fixes issue #56
    if (parsed.args.length) args = parsed.args.concat(args);

    self._args.forEach(function(arg, i) {
      if (arg.required && null == args[i]) {
        self.missingArgument(arg.name);
      } else if (arg.variadic) {
        if (i !== self._args.length - 1) {
          self.variadicArgNotLast(arg.name);
        }

        args[i] = args.splice(i);
      }
    });

    // Always append ourselves to the end of the arguments,
    // to make sure we match the number of arguments the user
    // expects
    if (self._args.length) {
      args[self._args.length] = self;
    } else {
      args.push(self);
    }

    fn.apply(self, args);
  };
  var parent = this.parent || this;
  var name = parent === this ? '*' : this._name;
  parent.on(name, listener);
  if (this._alias) parent.on(this._alias, listener);
  return this;
}
```
- example usage
```shell
...
'data:set': 'database:set',
'data:update': 'database:update',
'deploy:hosting': 'deploy --only hosting',
'deploy:database': 'deploy --only database',
'prefs:token': 'login:ci'
};

program.action(function(cmd, cmd2) {
logger.error(
  chalk.bold.red('Error:'),
  chalk.bold(cmd), 'is not a Firebase command'
);

if (RENAMED_COMMANDS[cmd]) {
  logger.error();
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.addImplicitHelpCommand"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>addImplicitHelpCommand ()](#apidoc.element.firebase-tools.cli.Command.prototype.addImplicitHelpCommand)
- description and source-code
```javascript
addImplicitHelpCommand = function () {
  this.command('help [cmd]', 'display help for [cmd]');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.alias"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>alias (alias)](#apidoc.element.firebase-tools.cli.Command.prototype.alias)
- description and source-code
```javascript
alias = function (alias) {
  if (0 == arguments.length) return this._alias;
  this._alias = alias;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.allowUnknownOption"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>allowUnknownOption (arg)](#apidoc.element.firebase-tools.cli.Command.prototype.allowUnknownOption)
- description and source-code
```javascript
allowUnknownOption = function (arg) {
    this._allowUnknownOption = arguments.length === 0 || arg;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.arguments"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>arguments (desc)](#apidoc.element.firebase-tools.cli.Command.prototype.arguments)
- description and source-code
```javascript
arguments = function (desc) {
  return this.parseExpectedArgs(desc.split(/ +/));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.command"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>command (name, desc, opts)](#apidoc.element.firebase-tools.cli.Command.prototype.command)
- description and source-code
```javascript
command = function (name, desc, opts) {
  opts = opts || {};
  var args = name.split(/ +/);
  var cmd = new Command(args.shift());

  if (desc) {
    cmd.description(desc);
    this.executables = true;
    this._execs[cmd._name] = true;
    if (opts.isDefault) this.defaultExecutable = cmd._name;
  }

  cmd._noHelp = !!opts.noHelp;
  this.commands.push(cmd);
  cmd.parseExpectedArgs(args);
  cmd.parent = this;

  if (desc) return this;
  return cmd;
}
```
- example usage
```shell
...
};

// ignoring this in coverage for now since it's just wrapping commander
/* istanbul ignore next */
Command.prototype.register = function(client) {
this.client = client;
var program = client.cli;
var cmd = program.command(this._cmd);
if (this._description) { cmd.description(this._description); }
this._options.forEach(function(args) { cmd.option.apply(cmd, args); });

var self = this;
cmd.action(function() {
  var runner = self.runner();
  var start = new Date().getTime();
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.commandHelp"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>commandHelp ()](#apidoc.element.firebase-tools.cli.Command.prototype.commandHelp)
- description and source-code
```javascript
commandHelp = function () {
  if (!this.commands.length) return '';

  var commands = this.commands.filter(function(cmd) {
    return !cmd._noHelp;
  }).map(function(cmd) {
    var args = cmd._args.map(function(arg) {
      return humanReadableArgName(arg);
    }).join(' ');

    return [
      cmd._name
        + (cmd._alias ? '|' + cmd._alias : '')
        + (cmd.options.length ? ' [options]' : '')
        + ' ' + args
      , cmd.description()
    ];
  });

  var width = commands.reduce(function(max, command) {
    return Math.max(max, command[0].length);
  }, 0);

  return [
    ''
    , '  Commands:'
    , ''
    , commands.map(function(cmd) {
      var desc = cmd[1] ? '  ' + cmd[1] : '';
      return pad(cmd[0], width) + desc;
    }).join('\n').replace(/^/gm, '    ')
    , ''
  ].join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.description"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>description (str)](#apidoc.element.firebase-tools.cli.Command.prototype.description)
- description and source-code
```javascript
description = function (str) {
  if (0 === arguments.length) return this._description;
  this._description = str;
  return this;
}
```
- example usage
```shell
...

var MAX_BATCH_SIZE = 1000;

var validateOptions = accountExporter.validateOptions;
var serialExportUsers = accountExporter.serialExportUsers;

module.exports = new Command('auth:export [dataFile]')
.description('Export accounts from your Firebase project into a data file')
.option(
    '--format <format>', 'Format of exported data (csv, json). Ignored if [dataFile] has format extension.')
.before(requireAccess)
.action(function(dataFile, options) {
  var projectId = getProjectId(options);
  var checkRes = validateOptions(options, dataFile);
  if (!checkRes.format) {
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.executeSubCommand"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>executeSubCommand (argv, args, unknown)](#apidoc.element.firebase-tools.cli.Command.prototype.executeSubCommand)
- description and source-code
```javascript
executeSubCommand = function (argv, args, unknown) {
  args = args.concat(unknown);

  if (!args.length) this.help();
  if ('help' == args[0] && 1 == args.length) this.help();

  // <cmd> --help
  if ('help' == args[0]) {
    args[0] = args[1];
    args[1] = '--help';
  }

  // executable
  var f = argv[1];
  // name of the subcommand, link 'pm-install'
  var bin = basename(f, '.js') + '-' + args[0];


  // In case of globally installed, get the base dir where executable
  //  subcommand file should be located at
  var baseDir
    , link = readlink(f);

  // when symbolink is relative path
  if (link !== f && link.charAt(0) !== '/') {
    link = path.join(dirname(f), link)
  }
  baseDir = dirname(link);

  // prefer local './<bin>' to bin in the $PATH
  var localBin = path.join(baseDir, bin);

  // whether bin file is a js script with explicit '.js' extension
  var isExplicitJS = false;
  if (exists(localBin + '.js')) {
    bin = localBin + '.js';
    isExplicitJS = true;
  } else if (exists(localBin)) {
    bin = localBin;
  }

  args = args.slice(1);

  var proc;
  if (process.platform !== 'win32') {
    if (isExplicitJS) {
      args.unshift(localBin);
      // add executable arguments to spawn
      args = (process.execArgv || []).concat(args);

      proc = spawn('node', args, { stdio: 'inherit', customFds: [0, 1, 2] });
    } else {
      proc = spawn(bin, args, { stdio: 'inherit', customFds: [0, 1, 2] });
    }
  } else {
    args.unshift(localBin);
    proc = spawn(process.execPath, args, { stdio: 'inherit'});
  }

  proc.on('close', process.exit.bind(process));
  proc.on('error', function(err) {
    if (err.code == "ENOENT") {
      console.error('\n  %s(1) does not exist, try --help\n', bin);
    } else if (err.code == "EACCES") {
      console.error('\n  %s(1) not executable. try chmod or run with root\n', bin);
    }
    process.exit(1);
  });

  // Store the reference to the child process
  this.runningCommand = proc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.help"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>help (cb)](#apidoc.element.firebase-tools.cli.Command.prototype.help)
- description and source-code
```javascript
help = function (cb) {
  this.outputHelp(cb);
  process.exit();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.helpInformation"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>helpInformation ()](#apidoc.element.firebase-tools.cli.Command.prototype.helpInformation)
- description and source-code
```javascript
helpInformation = function () {
  var desc = [];
  if (this._description) {
    desc = [
      '  ' + this._description
      , ''
    ];
  }

  var cmdName = this._name;
  if (this._alias) {
    cmdName = cmdName + '|' + this._alias;
  }
  var usage = [
    ''
    ,'  Usage: ' + cmdName + ' ' + this.usage()
    , ''
  ];

  var cmds = [];
  var commandHelp = this.commandHelp();
  if (commandHelp) cmds = [commandHelp];

  var options = [
    '  Options:'
    , ''
    , '' + this.optionHelp().replace(/^/gm, '    ')
    , ''
    , ''
  ];

  return usage
    .concat(cmds)
    .concat(desc)
    .concat(options)
    .join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.largestOptionLength"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>largestOptionLength ()](#apidoc.element.firebase-tools.cli.Command.prototype.largestOptionLength)
- description and source-code
```javascript
largestOptionLength = function () {
  return this.options.reduce(function(max, option) {
    return Math.max(max, option.flags.length);
  }, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.missingArgument"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>missingArgument (name)](#apidoc.element.firebase-tools.cli.Command.prototype.missingArgument)
- description and source-code
```javascript
missingArgument = function (name) {
  console.error();
  console.error("  error: missing required argument '%s'", name);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.name"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>name ()](#apidoc.element.firebase-tools.cli.Command.prototype.name)
- description and source-code
```javascript
name = function () {
  return this._name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.normalize"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>normalize (args)](#apidoc.element.firebase-tools.cli.Command.prototype.normalize)
- description and source-code
```javascript
normalize = function (args) {
  var ret = []
    , arg
    , lastOpt
    , index;

  for (var i = 0, len = args.length; i < len; ++i) {
    arg = args[i];
    if (i > 0) {
      lastOpt = this.optionFor(args[i-1]);
    }

    if (arg === '--') {
      // Honor option terminator
      ret = ret.concat(args.slice(i));
      break;
    } else if (lastOpt && lastOpt.required) {
      ret.push(arg);
    } else if (arg.length > 1 && '-' == arg[0] && '-' != arg[1]) {
      arg.slice(1).split('').forEach(function(c) {
        ret.push('-' + c);
      });
    } else if (/^--/.test(arg) && ~(index = arg.indexOf('='))) {
      ret.push(arg.slice(0, index), arg.slice(index + 1));
    } else {
      ret.push(arg);
    }
  }

  return ret;
}
```
- example usage
```shell
...
};

Config.prototype.has = function(key) {
  return _.has(this.data, key);
};

Config.prototype.path = function(pathName) {
  var outPath = path.normalize(path.join(this.projectDir, pathName));
  if (_.includes(path.relative(this.projectDir, outPath), '..')) {
    throw new FirebaseError(chalk.bold(pathName) + ' is outside of project directory', {exit: 1});
  }
  return outPath;
};

Config.prototype.readProjectFile = function(p, options) {
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.option"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>option (flags, description, fn, defaultValue)](#apidoc.element.firebase-tools.cli.Command.prototype.option)
- description and source-code
```javascript
option = function (flags, description, fn, defaultValue) {
  var self = this
    , option = new Option(flags, description)
    , oname = option.name()
    , name = camelcase(oname);

  // default as 3rd arg
  if (typeof fn != 'function') {
    if (fn instanceof RegExp) {
      var regex = fn;
      fn = function(val, def) {
        var m = regex.exec(val);
        return m ? m[0] : def;
      }
    }
    else {
      defaultValue = fn;
      fn = null;
    }
  }

  // preassign default value only for --no-*, [optional], or <required>
  if (false == option.bool || option.optional || option.required) {
    // when --no-* we make sure default is true
    if (false == option.bool) defaultValue = true;
    // preassign only if we have a default
    if (undefined !== defaultValue) self[name] = defaultValue;
  }

  // register the option
  this.options.push(option);

  // when it's passed assign the value
  // and conditionally invoke the callback
  this.on(oname, function(val) {
    // coercion
    if (null !== val && fn) val = fn(val, undefined === self[name]
      ? defaultValue
      : self[name]);

    // unassigned or bool
    if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
      // if no value, bool true, and we have a default, then use it!
      if (null == val) {
        self[name] = option.bool
          ? defaultValue || true
          : false;
      } else {
        self[name] = val;
      }
    } else if (null !== val) {
      // reassign
      self[name] = val;
    }
  });

  return this;
}
```
- example usage
```shell
...
var program = require('commander');
var pkg = require('./package.json');
var chalk = require('chalk');
var logger = require('./lib/logger');
var didYouMean = require('didyoumean');

program.version(pkg.version);
program.option('-P, --project <alias_or_project_id>', 'the Firebase project to use for this command');
program.option('-j, --json', 'output JSON instead of text, also triggers non-interactive mode');
program.option('--token <token>', 'supply an auth token for this command');
program.option('--non-interactive', 'error out of the command instead of waiting for prompts');
program.option('--interactive', 'force interactive shell treatment even when not detected');
program.option('--debug', 'print verbose debug output and keep a debug log file');
// program.option('-d, --debug', 'display debug information and keep firebase-debug.log');
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.optionFor"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionFor (arg)](#apidoc.element.firebase-tools.cli.Command.prototype.optionFor)
- description and source-code
```javascript
optionFor = function (arg) {
  for (var i = 0, len = this.options.length; i < len; ++i) {
    if (this.options[i].is(arg)) {
      return this.options[i];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.optionHelp"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionHelp ()](#apidoc.element.firebase-tools.cli.Command.prototype.optionHelp)
- description and source-code
```javascript
optionHelp = function () {
  var width = this.largestOptionLength();

  // Prepend the help information
  return [pad('-h, --help', width) + '  ' + 'output usage information']
      .concat(this.options.map(function(option) {
        return pad(option.flags, width) + '  ' + option.description;
      }))
      .join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.optionMissingArgument"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>optionMissingArgument (option, flag)](#apidoc.element.firebase-tools.cli.Command.prototype.optionMissingArgument)
- description and source-code
```javascript
optionMissingArgument = function (option, flag) {
  console.error();
  if (flag) {
    console.error("  error: option '%s' argument missing, got '%s'", option.flags, flag);
  } else {
    console.error("  error: option '%s' argument missing", option.flags);
  }
  console.error();
  process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.opts"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>opts ()](#apidoc.element.firebase-tools.cli.Command.prototype.opts)
- description and source-code
```javascript
opts = function () {
  var result = {}
    , len = this.options.length;

  for (var i = 0 ; i < len; i++) {
    var key = camelcase(this.options[i].name());
    result[key] = key === 'version' ? this._version : this[key];
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.outputHelp"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>outputHelp (cb)](#apidoc.element.firebase-tools.cli.Command.prototype.outputHelp)
- description and source-code
```javascript
outputHelp = function (cb) {
  if (!cb) {
    cb = function(passthru) {
      return passthru;
    }
  }
  process.stdout.write(cb(this.helpInformation()));
  this.emit('--help');
}
```
- example usage
```shell
...
var utils = require('../lib/utils');

module.exports = new Command('help [command]')
.description('display help information')
.action(function(commandName) {
  var cmd = this.client.getCommand(commandName);
  if (cmd) {
    cmd.outputHelp();
  } else if (commandName) {
    logger.warn();
    utils.logWarning(chalk.bold(commandName) + ' is not a valid command. See below for valid commands');
    this.client.cli.outputHelp();
  } else {
    this.client.cli.outputHelp();
    logger.info();
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.parse"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parse (argv)](#apidoc.element.firebase-tools.cli.Command.prototype.parse)
- description and source-code
```javascript
parse = function (argv) {
  // implicit help
  if (this.executables) this.addImplicitHelpCommand();

  // store raw args
  this.rawArgs = argv;

  // guess name
  this._name = this._name || basename(argv[1], '.js');

  // github-style sub-commands with no sub-command
  if (this.executables && argv.length < 3 && !this.defaultExecutable) {
    // this user needs help
    argv.push('--help');
  }

  // process argv
  var parsed = this.parseOptions(this.normalize(argv.slice(2)));
  var args = this.args = parsed.args;

  var result = this.parseArgs(this.args, parsed.unknown);

  // executable sub-commands
  var name = result.args[0];
  if (this._execs[name] && typeof this._execs[name] != "function") {
    return this.executeSubCommand(argv, args, parsed.unknown);
  } else if (this.defaultExecutable) {
    // use the default subcommand
    args.unshift(name = this.defaultExecutable);
    return this.executeSubCommand(argv, args, parsed.unknown);
  }

  return result;
}
```
- example usage
```shell
...
    if (currentBatch.length) {
      batches.push(currentBatch);
    }
    return resolve(batches);
  });
  inStream.pipe(parser);
} else {
  parser = jsonStream.parse(['users', {emitKey: true}]);
  parser.on('data', function(pair) {
    counter++;
    var res = validateUserJson(pair.value);
    if (res.error) {
      return reject(res.error);
    }
    currentBatch.push(pair.value);
...
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.parseArgs"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseArgs (args, unknown)](#apidoc.element.firebase-tools.cli.Command.prototype.parseArgs)
- description and source-code
```javascript
parseArgs = function (args, unknown) {
  var name;

  if (args.length) {
    name = args[0];
    if (this.listeners(name).length) {
      this.emit(args.shift(), args, unknown);
    } else {
      this.emit('*', args);
    }
  } else {
    outputHelpIfNecessary(this, unknown);

    // If there were no args and we have unknown options,
    // then they are extraneous and we need to error.
    if (unknown.length > 0) {
      this.unknownOption(unknown[0]);
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.parseExpectedArgs"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseExpectedArgs (args)](#apidoc.element.firebase-tools.cli.Command.prototype.parseExpectedArgs)
- description and source-code
```javascript
parseExpectedArgs = function (args) {
  if (!args.length) return;
  var self = this;
  args.forEach(function(arg) {
    var argDetails = {
      required: false,
      name: '',
      variadic: false
    };

    switch (arg[0]) {
      case '<':
        argDetails.required = true;
        argDetails.name = arg.slice(1, -1);
        break;
      case '[':
        argDetails.name = arg.slice(1, -1);
        break;
    }

    if (argDetails.name.length > 3 && argDetails.name.slice(-3) === '...') {
      argDetails.variadic = true;
      argDetails.name = argDetails.name.slice(0, -3);
    }
    if (argDetails.name) {
      self._args.push(argDetails);
    }
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.parseOptions"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>parseOptions (argv)](#apidoc.element.firebase-tools.cli.Command.prototype.parseOptions)
- description and source-code
```javascript
parseOptions = function (argv) {
  var args = []
    , len = argv.length
    , literal
    , option
    , arg;

  var unknownOptions = [];

  // parse options
  for (var i = 0; i < len; ++i) {
    arg = argv[i];

    // literal args after --
    if ('--' == arg) {
      literal = true;
      continue;
    }

    if (literal) {
      args.push(arg);
      continue;
    }

    // find matching Option
    option = this.optionFor(arg);

    // option is defined
    if (option) {
      // requires arg
      if (option.required) {
        arg = argv[++i];
        if (null == arg) return this.optionMissingArgument(option);
        this.emit(option.name(), arg);
      // optional arg
      } else if (option.optional) {
        arg = argv[i+1];
        if (null == arg || ('-' == arg[0] && '-' != arg)) {
          arg = null;
        } else {
          ++i;
        }
        this.emit(option.name(), arg);
      // bool
      } else {
        this.emit(option.name());
      }
      continue;
    }

    // looks like an option
    if (arg.length > 1 && '-' == arg[0]) {
      unknownOptions.push(arg);

      // If the next argument looks like it might be
      // an argument for this option, we pass it on.
      // If it isn't, then it'll simply be ignored
      if (argv[i+1] && '-' != argv[i+1][0]) {
        unknownOptions.push(argv[++i]);
      }
      continue;
    }

    // arg
    args.push(arg);
  }

  return { args: args, unknown: unknownOptions };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.unknownOption"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>unknownOption (flag)](#apidoc.element.firebase-tools.cli.Command.prototype.unknownOption)
- description and source-code
```javascript
unknownOption = function (flag) {
  if (this._allowUnknownOption) return;
  console.error();
  console.error("  error: unknown option '%s'", flag);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.usage"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>usage (str)](#apidoc.element.firebase-tools.cli.Command.prototype.usage)
- description and source-code
```javascript
usage = function (str) {
  var args = this._args.map(function(arg) {
    return humanReadableArgName(arg);
  });

  var usage = '[options]'
    + (this.commands.length ? ' [command]' : '')
    + (this._args.length ? ' ' + args.join(' ') : '');

  if (0 == arguments.length) return this._usage || usage;
  this._usage = str;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.variadicArgNotLast"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>variadicArgNotLast (name)](#apidoc.element.firebase-tools.cli.Command.prototype.variadicArgNotLast)
- description and source-code
```javascript
variadicArgNotLast = function (name) {
  console.error();
  console.error("  error: variadic arguments must be last '%s'", name);
  console.error();
  process.exit(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Command.prototype.version"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Command.prototype.</span>version (str, flags)](#apidoc.element.firebase-tools.cli.Command.prototype.version)
- description and source-code
```javascript
version = function (str, flags) {
  if (0 == arguments.length) return this._version;
  this._version = str;
  flags = flags || '-V, --version';
  this.option(flags, 'output the version number');
  this.on('version', function() {
    process.stdout.write(str + '\n');
    process.exit(0);
  });
  return this;
}
```
- example usage
```shell
...

var program = require('commander');
var pkg = require('./package.json');
var chalk = require('chalk');
var logger = require('./lib/logger');
var didYouMean = require('didyoumean');

program.version(pkg.version);
program.option('-P, --project <alias_or_project_id>', 'the Firebase project to use for this command');
program.option('-j, --json', 'output JSON instead of text, also triggers non-interactive mode');
program.option('--token <token>', 'supply an auth token for this command');
program.option('--non-interactive', 'error out of the command instead of waiting for prompts');
program.option('--interactive', 'force interactive shell treatment even when not detected');
program.option('--debug', 'print verbose debug output and keep a debug log file');
// program.option('-d, --debug', 'display debug information and keep firebase-debug.log');
...
```



# <a name="apidoc.module.firebase-tools.cli.Option"></a>[module firebase-tools.cli.Option](#apidoc.module.firebase-tools.cli.Option)

#### <a name="apidoc.element.firebase-tools.cli.Option.Option"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.</span>Option (flags, description)](#apidoc.element.firebase-tools.cli.Option.Option)
- description and source-code
```javascript
function Option(flags, description) {
  this.flags = flags;
  this.required = ~flags.indexOf('<');
  this.optional = ~flags.indexOf('[');
  this.bool = !~flags.indexOf('-no-');
  flags = flags.split(/[ ,|]+/);
  if (flags.length > 1 && !/^[[<]/.test(flags[1])) this.short = flags.shift();
  this.long = flags.shift();
  this.description = description || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.cli.Option.prototype"></a>[module firebase-tools.cli.Option.prototype](#apidoc.module.firebase-tools.cli.Option.prototype)

#### <a name="apidoc.element.firebase-tools.cli.Option.prototype.is"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Option.prototype.</span>is (arg)](#apidoc.element.firebase-tools.cli.Option.prototype.is)
- description and source-code
```javascript
is = function (arg) {
  return arg == this.short || arg == this.long;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli.Option.prototype.name"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli.Option.prototype.</span>name ()](#apidoc.element.firebase-tools.cli.Option.prototype.name)
- description and source-code
```javascript
name = function () {
  return this.long
    .replace('--', '')
    .replace('no-', '');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.cli._events"></a>[module firebase-tools.cli._events](#apidoc.module.firebase-tools.cli._events)

#### <a name="apidoc.element.firebase-tools.cli._events.debug"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>debug (val)](#apidoc.element.firebase-tools.cli._events.debug)
- description and source-code
```javascript
debug = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
...
var responseToError = require('./responseToError');
var refreshToken;
var commandScopes;
var scopes = require('./scopes');
var CLI_VERSION = require('../package.json').version;

var _request = function(options) {
logger.debug('>>> HTTP REQUEST',
  options.method,
  options.url,
  options.body || options.form || '',
  '\n',
  new Date().toString()
);
...
```

#### <a name="apidoc.element.firebase-tools.cli._events.deploy"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>deploy (args, unknown)](#apidoc.element.firebase-tools.cli._events.deploy)
- description and source-code
```javascript
deploy = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
...
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
token: process.env.FIREBASE_TOKEN,
cwd: '/path/to/project/folder'
}).then(function() {
console.log('Rules have been deployed!')
}).catch(function(err) {
// handle error
...
```

#### <a name="apidoc.element.firebase-tools.cli._events.help"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>help (args, unknown)](#apidoc.element.firebase-tools.cli._events.help)
- description and source-code
```javascript
help = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.init"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>init (args, unknown)](#apidoc.element.firebase-tools.cli._events.init)
- description and source-code
```javascript
init = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.interactive"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>interactive (val)](#apidoc.element.firebase-tools.cli._events.interactive)
- description and source-code
```javascript
interactive = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.json"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>json (val)](#apidoc.element.firebase-tools.cli._events.json)
- description and source-code
```javascript
json = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.list"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>list (args, unknown)](#apidoc.element.firebase-tools.cli._events.list)
- description and source-code
```javascript
list = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
...

## Using as a Module

The Firebase CLI can also be used programmatically as a standard Node module. Each command is exposed as a function that takes an
 options object and returns a Promise. For example:

'''js
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
...
```

#### <a name="apidoc.element.firebase-tools.cli._events.login"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>login (args, unknown)](#apidoc.element.firebase-tools.cli._events.login)
- description and source-code
```javascript
login = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
...
.description('generate an access token for use in non-interactive environments')
.option('--no-localhost', 'copy and paste a code instead of starting a local server for authentication')
.action(function(options) {
  if (options.nonInteractive) {
    return utils.reject('Cannot run login:ci in non-interactive mode.', {exit: 1});
  }

  return auth.login(options.localhost).then(function(result) {
    logger.info();
    utils.logSuccess('Success! Use this token to login on a CI server:\n\n' +
      chalk.bold(result.tokens.refresh_token) + '\n\nExample: firebase deploy --token "$FIREBASE_TOKEN"\n');
    return result;
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.cli._events.logout"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>logout (args, unknown)](#apidoc.element.firebase-tools.cli._events.logout)
- description and source-code
```javascript
logout = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
...
var user = configstore.get('user');
var tokens = configstore.get('tokens');
var currentToken = _.get(tokens, 'refresh_token');
var token = utils.getInheritedOption(options, 'token') || currentToken;
api.setToken(token);
var next;
if (token) {
  next = auth.logout(token);
} else {
  next = RSVP.resolve();
}

var cleanup = function() {
  if (token || user || tokens) {
    var msg = 'Logged out';
...
```

#### <a name="apidoc.element.firebase-tools.cli._events.non-interactive"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>non-interactive (val)](#apidoc.element.firebase-tools.cli._events.non-interactive)
- description and source-code
```javascript
non-interactive = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.open"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>open (args, unknown)](#apidoc.element.firebase-tools.cli._events.open)
- description and source-code
```javascript
open = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.project"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>project (val)](#apidoc.element.firebase-tools.cli._events.project)
- description and source-code
```javascript
project = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.serve"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>serve (args, unknown)](#apidoc.element.firebase-tools.cli._events.serve)
- description and source-code
```javascript
serve = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.token"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>token (val)](#apidoc.element.firebase-tools.cli._events.token)
- description and source-code
```javascript
token = function (val) {
  // coercion
  if (null !== val && fn) val = fn(val, undefined === self[name]
    ? defaultValue
    : self[name]);

  // unassigned or bool
  if ('boolean' == typeof self[name] || 'undefined' == typeof self[name]) {
    // if no value, bool true, and we have a default, then use it!
    if (null == val) {
      self[name] = option.bool
        ? defaultValue || true
        : false;
    } else {
      self[name] = val;
    }
  } else if (null !== val) {
    // reassign
    self[name] = val;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.cli._events.use"></a>[function <span class="apidocSignatureSpan">firebase-tools.cli._events.</span>use (args, unknown)](#apidoc.element.firebase-tools.cli._events.use)
- description and source-code
```javascript
use = function (args, unknown) {
  // Parse any so-far unknown options
  args = args || [];
  unknown = unknown || [];

  var parsed = self.parseOptions(unknown);

  // Output help if necessary
  outputHelpIfNecessary(self, parsed.unknown);

  // If there are still any unknown options, then we simply
  // die, unless someone asked for help, in which case we give it
  // to them, and then we die.
  if (parsed.unknown.length > 0) {
    self.unknownOption(parsed.unknown[0]);
  }

  // Leftover arguments need to be pushed back. Fixes issue #56
  if (parsed.args.length) args = parsed.args.concat(args);

  self._args.forEach(function(arg, i) {
    if (arg.required && null == args[i]) {
      self.missingArgument(arg.name);
    } else if (arg.variadic) {
      if (i !== self._args.length - 1) {
        self.variadicArgNotLast(arg.name);
      }

      args[i] = args.splice(i);
    }
  });

  // Always append ourselves to the end of the arguments,
  // to make sure we match the number of arguments the user
  // expects
  if (self._args.length) {
    args[self._args.length] = self;
  } else {
    args.push(self);
  }

  fn.apply(self, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.command"></a>[module firebase-tools.command](#apidoc.module.firebase-tools.command)

#### <a name="apidoc.element.firebase-tools.command.command"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>command (cmd)](#apidoc.element.firebase-tools.command.command)
- description and source-code
```javascript
command = function (cmd) {
  this._cmd = cmd;
  this._name = _.first(cmd.split(' '));
  this._description = null;
  this._options = [];
  this._action = null;
  this._befores = [];
}
```
- example usage
```shell
...
};

// ignoring this in coverage for now since it's just wrapping commander
/* istanbul ignore next */
Command.prototype.register = function(client) {
this.client = client;
var program = client.cli;
var cmd = program.command(this._cmd);
if (this._description) { cmd.description(this._description); }
this._options.forEach(function(args) { cmd.option.apply(cmd, args); });

var self = this;
cmd.action(function() {
  var runner = self.runner();
  var start = new Date().getTime();
...
```



# <a name="apidoc.module.firebase-tools.command.prototype"></a>[module firebase-tools.command.prototype](#apidoc.module.firebase-tools.command.prototype)

#### <a name="apidoc.element.firebase-tools.command.prototype._prepare"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>_prepare (options)](#apidoc.element.firebase-tools.command.prototype._prepare)
- description and source-code
```javascript
_prepare = function (options) {
  options = options || {};
  options.project = utils.getInheritedOption(options, 'project');

  if (!process.stdin.isTTY || utils.getInheritedOption(options, 'nonInteractive')) {
    options.nonInteractive = true;
  }
  // allow override of detected non-interactive with --interactive flag
  if (utils.getInheritedOption(options, 'interactive')) {
    options.nonInteractive = false;
  }

  if (utils.getInheritedOption(options, 'debug')) {
    logger.transports.console.level = 'debug';
  }
  if (utils.getInheritedOption(options, 'json')) {
    options.nonInteractive = true;
    logger.transports.console.level = 'none';
  }

  try {
    options.config = Config.load(options);
  } catch (e) {
    options.configError = e;
  }

  options.projectRoot = detectProjectRoot(options.cwd);
  this.applyRC(options);
  return RSVP.resolve();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.command.prototype.action"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>action (fn)](#apidoc.element.firebase-tools.command.prototype.action)
- description and source-code
```javascript
action = function (fn) {
  this._action = fn;
  return this;
}
```
- example usage
```shell
...
'data:set': 'database:set',
'data:update': 'database:update',
'deploy:hosting': 'deploy --only hosting',
'deploy:database': 'deploy --only database',
'prefs:token': 'login:ci'
};

program.action(function(cmd, cmd2) {
logger.error(
  chalk.bold.red('Error:'),
  chalk.bold(cmd), 'is not a Firebase command'
);

if (RENAMED_COMMANDS[cmd]) {
  logger.error();
...
```

#### <a name="apidoc.element.firebase-tools.command.prototype.applyRC"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>applyRC (options)](#apidoc.element.firebase-tools.command.prototype.applyRC)
- description and source-code
```javascript
applyRC = function (options) {
  var rc = loadRCFile(options.cwd);
  options.rc = rc;

  options.project = options.project || (configstore.get('activeProjects') || {})[options.projectRoot];
  // support deprecated "firebase" key in firebase.json
  if (options.config && !options.project) {
    options.project = options.config.defaults.project;
  }

  var aliases = rc.projects || {};
  var rcProject = _.get(aliases, options.project);
  if (rcProject) {
    options.projectAlias = options.project;
    options.project = rcProject;
  } else if (!options.project && _.size(aliases) === 1) {
    options.projectAlias = _.head(_.keys(aliases));
    options.project = _.head(_.values(aliases));
  }
}
```
- example usage
```shell
...
  try {
    options.config = Config.load(options);
  } catch (e) {
    options.configError = e;
  }

  options.projectRoot = detectProjectRoot(options.cwd);
  this.applyRC(options);
  return RSVP.resolve();
};

/**
 * Apply configuration from .firebaserc files in the working directory tree.
 */
Command.prototype.applyRC = function(options) {
...
```

#### <a name="apidoc.element.firebase-tools.command.prototype.before"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>before (fn, args)](#apidoc.element.firebase-tools.command.prototype.before)
- description and source-code
```javascript
before = function (fn, args) {
  this._befores.push({
    fn: fn,
    args: args
  });
  return this;
}
```
- example usage
```shell
...
var validateOptions = accountExporter.validateOptions;
var serialExportUsers = accountExporter.serialExportUsers;

module.exports = new Command('auth:export [dataFile]')
.description('Export accounts from your Firebase project into a data file')
.option(
    '--format <format>', 'Format of exported data (csv, json). Ignored if [dataFile] has format extension.')
.before(requireAccess)
.action(function(dataFile, options) {
  var projectId = getProjectId(options);
  var checkRes = validateOptions(options, dataFile);
  if (!checkRes.format) {
    return checkRes;
  }
  var exportOptions = checkRes;
...
```

#### <a name="apidoc.element.firebase-tools.command.prototype.description"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>description (description)](#apidoc.element.firebase-tools.command.prototype.description)
- description and source-code
```javascript
description = function (description) {
  this._description = description;
  return this;
}
```
- example usage
```shell
...

var MAX_BATCH_SIZE = 1000;

var validateOptions = accountExporter.validateOptions;
var serialExportUsers = accountExporter.serialExportUsers;

module.exports = new Command('auth:export [dataFile]')
.description('Export accounts from your Firebase project into a data file')
.option(
    '--format <format>', 'Format of exported data (csv, json). Ignored if [dataFile] has format extension.')
.before(requireAccess)
.action(function(dataFile, options) {
  var projectId = getProjectId(options);
  var checkRes = validateOptions(options, dataFile);
  if (!checkRes.format) {
...
```

#### <a name="apidoc.element.firebase-tools.command.prototype.option"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>option ()](#apidoc.element.firebase-tools.command.prototype.option)
- description and source-code
```javascript
option = function () {
  this._options.push(arguments);
  return this;
}
```
- example usage
```shell
...
var program = require('commander');
var pkg = require('./package.json');
var chalk = require('chalk');
var logger = require('./lib/logger');
var didYouMean = require('didyoumean');

program.version(pkg.version);
program.option('-P, --project <alias_or_project_id>', 'the Firebase project to use for this command');
program.option('-j, --json', 'output JSON instead of text, also triggers non-interactive mode');
program.option('--token <token>', 'supply an auth token for this command');
program.option('--non-interactive', 'error out of the command instead of waiting for prompts');
program.option('--interactive', 'force interactive shell treatment even when not detected');
program.option('--debug', 'print verbose debug output and keep a debug log file');
// program.option('-d, --debug', 'display debug information and keep firebase-debug.log');
...
```

#### <a name="apidoc.element.firebase-tools.command.prototype.register"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>register (client)](#apidoc.element.firebase-tools.command.prototype.register)
- description and source-code
```javascript
register = function (client) {
  this.client = client;
  var program = client.cli;
  var cmd = program.command(this._cmd);
  if (this._description) { cmd.description(this._description); }
  this._options.forEach(function(args) { cmd.option.apply(cmd, args); });

  var self = this;
  cmd.action(function() {
    var runner = self.runner();
    var start = new Date().getTime();
    var options = _.last(_.toArray(arguments));
    var argCount = cmd._args.length;
    if (arguments.length - 1 > argCount) {
      return client.errorOut(
        new FirebaseError('Too many arguments. Run ' + chalk.bold('firebase help ' + cmd._name) + ' for usage instructions', {exit
: 1})
      );
    }

    runner.apply(self, arguments).then(function(result) {
      if (utils.getInheritedOption(options, 'json')) {
        console.log(JSON.stringify({
          status: 'success',
          result: result
        }, null, 2));
      }
      var duration = new Date().getTime() - start;
      track(self._name, 'success', duration).then(process.exit);
    }).catch(function(err) {
      if (utils.getInheritedOption(options, 'json')) {
        console.log(JSON.stringify({
          status: 'error',
          error: err.message
        }, null, 2));
      }
      var duration = Date.now() - start;
      var errorEvent = err.exit === 1 ? 'Error (User)' : 'Error (Unexpected)';
      var projectId = getProjectId(options, true);
      var preppedMessage = chalk.stripColor(err.message || '').replace(projectId, '<namespace>');

      RSVP.all([
        track(self._name, 'error', duration),
        track(errorEvent, preppedMessage, duration)
      ]).then(function() {
        client.errorOut(err);
      });
    });

    return cmd;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.command.prototype.runner"></a>[function <span class="apidocSignatureSpan">firebase-tools.command.prototype.</span>runner ()](#apidoc.element.firebase-tools.command.prototype.runner)
- description and source-code
```javascript
runner = function () {
  var self = this;
  return function() {
    var args = _.toArray(arguments);
    // always provide at least an empty object for options
    if (args.length === 0) {
      args.push({});
    }
    var options = _.last(args);

    try {
      var befores = [self._prepare].concat(self._befores);
      var result = befores.shift().call(self, options);
      befores.forEach(function(before) {
        result = result.then(function() {
          return before.fn.call(self, options, before.args);
        });
      });
      return result.then(function() {
        return self._action.apply(self, args);
      });
    } catch (e) {
      return RSVP.reject(e);
    }
  };
}
```
- example usage
```shell
...
var program = client.cli;
var cmd = program.command(this._cmd);
if (this._description) { cmd.description(this._description); }
this._options.forEach(function(args) { cmd.option.apply(cmd, args); });

var self = this;
cmd.action(function() {
  var runner = self.runner();
  var start = new Date().getTime();
  var options = _.last(_.toArray(arguments));
  var argCount = cmd._args.length;
  if (arguments.length - 1 > argCount) {
    return client.errorOut(
      new FirebaseError('Too many arguments. Run ' + chalk.bold('firebase help ' + cmd._name) + ' for usage instructions', {exit
: 1})
    );
...
```



# <a name="apidoc.module.firebase-tools.config"></a>[module firebase-tools.config](#apidoc.module.firebase-tools.config)

#### <a name="apidoc.element.firebase-tools.config.config"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>config (src, options)](#apidoc.element.firebase-tools.config.config)
- description and source-code
```javascript
config = function (src, options) {
  this.options = options || {};
  this.projectDir = options.projectDir || detectProjectRoot(options.cwd);

  this._src = src;
  this.data = {};
  this.defaults = {};
  this.notes = {};

  if (this._src.firebase) {
    this.defaults.project = this._src.firebase;
    utils.logWarning(chalk.bold('"firebase"') + ' key in firebase.json is deprecated. Run ' + chalk.bold('firebase use --add') + '
instead');
  }

  if (_.has(this._src, 'rules')) {
    _.set(this._src, 'database.rules', this._src.rules);
  }

  Config.MATERIALIZE_TARGETS.forEach(function(target) {
    if (_.get(this._src, target)) {
      if (target === 'database.rules') {
        _.set(this.data, 'database.rulesString', this._materialize(target));
      } else {
        _.set(this.data, target, this._materialize(target));
      }
    }
  }, this);

  // auto-detect functions from package.json in directory
  if (this.projectDir && !this.get('functions.source') && fsutils.fileExistsSync(this.path('functions/package.json'))) {
    this.set('functions.source', 'functions');
  }

  // use 'public' as signal for legacy hosting since it's a required key
  if (!this.data.hosting && this._src.public) {
    this.importLegacyHostingKeys();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.config.load"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.</span>load (options, allowMissing)](#apidoc.element.firebase-tools.config.load)
- description and source-code
```javascript
load = function (options, allowMissing) {
  var pd = detectProjectRoot(options.cwd);
  if (pd) {
    try {
      var data = cjson.load(path.join(pd, Config.FILENAME));
      return new Config(data, options);
    } catch (e) {
      throw new FirebaseError('There was an error loading firebase.json:\n\n' + e.message, {
        exit: 1
      });
    }
  }

  if (allowMissing) {
    return null;
  }

  throw new FirebaseError('Not in a Firebase app directory (could not locate firebase.json)', {exit: 1});
}
```
- example usage
```shell
...
if (_isOutside(homeDir, cwd)) {
  warnings.push('You are currently outside your home directory');
}
if (cwd === homeDir) {
  warnings.push('You are initializing your home directory as a Firebase project');
}

var config = Config.load(options, true);
var existingConfig = !!config;
if (!existingConfig) {
  config = new Config({}, {projectDir: cwd, cwd: cwd});
} else {
  warnings.push('You are initializing in an existing Firebase project directory');
}
...
```



# <a name="apidoc.module.firebase-tools.config.prototype"></a>[module firebase-tools.config.prototype](#apidoc.module.firebase-tools.config.prototype)

#### <a name="apidoc.element.firebase-tools.config.prototype._hasDeepKey"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_hasDeepKey (obj, key)](#apidoc.element.firebase-tools.config.prototype._hasDeepKey)
- description and source-code
```javascript
_hasDeepKey = function (obj, key) {
  if (_.has(obj, key)) {
    return true;
  }

  for (var k in obj) {
    if (_.isPlainObject(obj[k]) && this._hasDeepKey(obj[k], key)) {
      return true;
    }
  }
  return false;
}
```
- example usage
```shell
...

Config.prototype._hasDeepKey = function(obj, key) {
  if (_.has(obj, key)) {
    return true;
  }

  for (var k in obj) {
    if (_.isPlainObject(obj[k]) && this._hasDeepKey(obj[k], key)) {
      return true;
    }
  }
  return false;
};

Config.prototype._materialize = function(target) {
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype._materialize"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_materialize (target)](#apidoc.element.firebase-tools.config.prototype._materialize)
- description and source-code
```javascript
_materialize = function (target) {
  var val = _.get(this._src, target);
  if (_.isString(val)) {
    var out = this._parseFile(target, val);
    // if e.g. rules.json has {"rules": {}} use that
    var lastSegment = _.last(target.split('.'));
    if (_.size(out) === 1 && _.has(out, lastSegment)) {
      out = out[lastSegment];
    }
    return out;
  } else if (_.isObject(val)) {
    if (target === 'database.rules') {
      this.notes.databaseRules = 'inline';
      return JSON.stringify({ 'rules': val }, null, 2);
    }
    return val;
  }

  throw new FirebaseError('Parse Error: "' + target + '" must be object or import path', {exit: 1});
}
```
- example usage
```shell
...
if (_.has(this._src, 'rules')) {
  _.set(this._src, 'database.rules', this._src.rules);
}

Config.MATERIALIZE_TARGETS.forEach(function(target) {
  if (_.get(this._src, target)) {
    if (target === 'database.rules') {
      _.set(this.data, 'database.rulesString', this._materialize(target));
    } else {
      _.set(this.data, target, this._materialize(target));
    }
  }
}, this);

// auto-detect functions from package.json in directory
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype._parseFile"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>_parseFile (target, filePath)](#apidoc.element.firebase-tools.config.prototype._parseFile)
- description and source-code
```javascript
_parseFile = function (target, filePath) {
  var fullPath = resolveProjectPath(this.options.cwd, filePath);
  var ext = path.extname(filePath);
  if (!fsutils.fileExistsSync(fullPath)) {
    throw new FirebaseError('Parse Error: Imported file ' + filePath + ' does not exist', {exit: 1});
  }

  switch (ext) {
  case '.json':
    if (target === 'database') {
      this.notes.databaseRules = 'json';
    } else if (target === 'database.rules') {
      var rules = fs.readFileSync(fullPath, 'utf8');
      if (validateJsonRules(rules)) {
        return rules;
      }
      utils.logWarning(chalk.bold.yellow('database: ') + chalk.bold(filePath) + ' must have an outer ' + chalk.bold('rules') + '
key, for example:');
      logger.warn('\n{\n\t"rules": {".read": false, ".write": false}\n}');
      throw new FirebaseError('Database security rules are not correctly formatted', {exit: 1});
    }
    return loadCJSON(fullPath);
<span class="apidocCodeCommentSpan">  /* istanbul ignore-next */
</span>  case '.bolt':
    if (target === 'database') {
      this.notes.databaseRules = 'bolt';
    }
    return parseBoltRules(fullPath);
  default:
    throw new FirebaseError('Parse Error: ' + filePath + ' is not of a supported config file type', {exit: 1});
  }
}
```
- example usage
```shell
...
}
return false;
};

Config.prototype._materialize = function(target) {
var val = _.get(this._src, target);
if (_.isString(val)) {
  var out = this._parseFile(target, val);
  // if e.g. rules.json has {"rules": {}} use that
  var lastSegment = _.last(target.split('.'));
  if (_.size(out) === 1 && _.has(out, lastSegment)) {
    out = out[lastSegment];
  }
  return out;
} else if (_.isObject(val)) {
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.askWriteProjectFile"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>askWriteProjectFile (p, content)](#apidoc.element.firebase-tools.config.prototype.askWriteProjectFile)
- description and source-code
```javascript
askWriteProjectFile = function (p, content) {
  var writeTo = this.path(p);
  var next;
  if (fsutils.fileExistsSync(writeTo)) {
    next = prompt.once({
      type: 'confirm',
      message: 'File ' + chalk.underline(p) + ' already exists. Overwrite?',
      default: false
    });
  } else {
    next = RSVP.resolve(true);
  }

  var self = this;
  return next.then(function(result) {
    if (result) {
      self.writeProjectFile(p, content);
      utils.logSuccess('Wrote ' + chalk.bold(p));
    } else {
      utils.logBullet('Skipping write of ' + chalk.bold(p));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.config.prototype.get"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>get (key, fallback)](#apidoc.element.firebase-tools.config.prototype.get)
- description and source-code
```javascript
get = function (key, fallback) {
  return _.get(this.data, key, fallback);
}
```
- example usage
```shell
...
      return new RSVP.Promise(function(resolve, reject) {
var fileOut = !!options.output;
var outStream = fileOut ? fs.createWriteStream(options.output) : process.stdout;
var erroring;
var errorResponse = '';
var response;

request.get(reqOptionsWithToken)
  .on('response', function(res) {
    response = res;
    if (response.statusCode >= 400) {
      erroring = true;
    }
  })
  .on('data', function(chunk) {
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.has"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>has (key)](#apidoc.element.firebase-tools.config.prototype.has)
- description and source-code
```javascript
has = function (key) {
  return _.has(this.data, key);
}
```
- example usage
```shell
...
.before(requireAccess)
.action(function(options) {
  // Validate options
  if (options.raw && options.input) {
    return utils.reject('Cannot specify both an input file and raw format', {exit: 1});
  } else if (options.parent.json && options.raw) {
    return utils.reject('Cannot output raw data in json format', {exit: 1});
  } else if (options.input && _.has(options, 'duration')) {
    return utils.reject('Cannot specify a duration for input files', {exit: 1});
  } else if (_.has(options, 'duration') && options.duration <= 0) {
    return utils.reject('Must specify a positive number of seconds', {exit: 1});
  }

  return profiler(options);
});
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.importLegacyHostingKeys"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>importLegacyHostingKeys ()](#apidoc.element.firebase-tools.config.prototype.importLegacyHostingKeys)
- description and source-code
```javascript
importLegacyHostingKeys = function () {
  var found = false;
  Config.LEGACY_HOSTING_KEYS.forEach(function(key) {
    if (_.has(this._src, key)) {
      found = true;
      this.set('hosting.' + key, this._src[key]);
    }
  }, this);
  if (found) {
    utils.logWarning('Deprecation Warning: Firebase Hosting configuration should be moved under "hosting" key.');
  }
}
```
- example usage
```shell
...
  // auto-detect functions from package.json in directory
  if (this.projectDir && !this.get('functions.source') && fsutils.fileExistsSync(this.path('functions/package.json'))) {
    this.set('functions.source', 'functions');
  }

  // use 'public' as signal for legacy hosting since it's a required key
  if (!this.data.hosting && this._src.public) {
    this.importLegacyHostingKeys();
  }
};

Config.FILENAME = 'firebase.json';
Config.MATERIALIZE_TARGETS = ['functions', 'hosting', 'database.rules', 'storage'];
Config.LEGACY_HOSTING_KEYS = ['public', 'rewrites', 'redirects', 'headers', 'ignore', 'cleanUrls', 'trailingSlash'];
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.path"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>path (pathName)](#apidoc.element.firebase-tools.config.prototype.path)
- description and source-code
```javascript
path = function (pathName) {
  var outPath = path.normalize(path.join(this.projectDir, pathName));
  if (_.includes(path.relative(this.projectDir, outPath), '..')) {
    throw new FirebaseError(chalk.bold(pathName) + ' is outside of project directory', {exit: 1});
  }
  return outPath;
}
```
- example usage
```shell
...
    } else {
      _.set(this.data, target, this._materialize(target));
    }
  }
}, this);

// auto-detect functions from package.json in directory
if (this.projectDir && !this.get('functions.source') && fsutils.fileExistsSync(this.path('functions/package.json'))) {
  this.set('functions.source', 'functions');
}

// use 'public' as signal for legacy hosting since it's a required key
if (!this.data.hosting && this._src.public) {
  this.importLegacyHostingKeys();
}
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.readProjectFile"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>readProjectFile (p, options)](#apidoc.element.firebase-tools.config.prototype.readProjectFile)
- description and source-code
```javascript
readProjectFile = function (p, options) {
  try {
    var content = fs.readFileSync(this.path(p), 'utf8');
    if (options.json) {
      return JSON.parse(content);
    }
    return content;
  } catch (e) {
    if (options.fallback) {
      return options.fallback;
    }
    throw e;
  }
}
```
- example usage
```shell
...
logger.info(chalk.yellow.bold(BANNER_TEXT) +
  '\nYou\'re about to initialize a Firebase project in this directory:\n\n  ' + chalk.bold(config.projectDir) + '\n' +
  warningText
);

var setup = {
  config: config._src,
  rcfile: config.readProjectFile('.firebaserc', {
    json: true,
    fallback: {}
  })
};

var choices = [
  {name: 'database', label: 'Database: Deploy Firebase Realtime Database Rules', checked: true},
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.set"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>set (key, value)](#apidoc.element.firebase-tools.config.prototype.set)
- description and source-code
```javascript
set = function (key, value) {
  return _.set(this.data, key, value);
}
```
- example usage
```shell
...
}

return prompt(options, [{
  type: 'confirm',
  name: 'collectUsage',
  message: 'Allow Firebase to collect anonymous CLI usage information?'
}]).then(function() {
  configstore.set('usage', options.collectUsage);
  return auth.login(options.localhost);
}).then(function(result) {
  configstore.set('user', result.user);
  configstore.set('tokens', result.tokens);
  // store login scopes in case mandatory scopes grow over time
  configstore.set('loginScopes', result.scopes);
  // remove old session token, if it exists
...
```

#### <a name="apidoc.element.firebase-tools.config.prototype.writeProjectFile"></a>[function <span class="apidocSignatureSpan">firebase-tools.config.prototype.</span>writeProjectFile (p, content)](#apidoc.element.firebase-tools.config.prototype.writeProjectFile)
- description and source-code
```javascript
writeProjectFile = function (p, content) {
  if (typeof content !== 'string') {
    content = JSON.stringify(content, null, 2) + '\n';
  }

  fs.ensureFileSync(this.path(p));
  fs.writeFileSync(this.path(p), content, 'utf8');
}
```
- example usage
```shell
...
  });
}
setup.features.unshift('project');
return init(setup, config, options);
    }).then(function() {
logger.info();
utils.logBullet('Writing configuration info to ' + chalk.bold('firebase.json') + '...');
config.writeProjectFile('firebase.json', setup.config);
utils.logBullet('Writing project information to ' + chalk.bold('.firebaserc') + '...');
config.writeProjectFile('.firebaserc', setup.rcfile);
logger.info();
utils.logSuccess('Firebase initialization complete!');

if (setup.createProject) {
  logger.info();
...
```



# <a name="apidoc.module.firebase-tools.database"></a>[module firebase-tools.database](#apidoc.module.firebase-tools.database)

#### <a name="apidoc.element.firebase-tools.database.get"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>get ()](#apidoc.element.firebase-tools.database.get)
- description and source-code
```javascript
get = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
      return new RSVP.Promise(function(resolve, reject) {
var fileOut = !!options.output;
var outStream = fileOut ? fs.createWriteStream(options.output) : process.stdout;
var erroring;
var errorResponse = '';
var response;

request.get(reqOptionsWithToken)
  .on('response', function(res) {
    response = res;
    if (response.statusCode >= 400) {
      erroring = true;
    }
  })
  .on('data', function(chunk) {
...
```

#### <a name="apidoc.element.firebase-tools.database.profile"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>profile ()](#apidoc.element.firebase-tools.database.profile)
- description and source-code
```javascript
profile = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.database.push"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>push ()](#apidoc.element.firebase-tools.database.push)
- description and source-code
```javascript
push = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
  counter++;
  var user = transArrayToUser(line.map(
    function(str) {
      // Ignore starting '|'' and trailing '|''
      var newStr = str.trim().replace(/^["|'](.*)["|']$/, '$1');
      return newStr === '' ? undefined : newStr;
    }));
  currentBatch.push(user);
  if (currentBatch.length === MAX_BATCH_SIZE) {
    batches.push(currentBatch);
    currentBatch = [];
  }
}).on('end', function() {
  if (currentBatch.length) {
    batches.push(currentBatch);
...
```

#### <a name="apidoc.element.firebase-tools.database.remove"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>remove ()](#apidoc.element.firebase-tools.database.remove)
- description and source-code
```javascript
remove = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.database.set"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>set ()](#apidoc.element.firebase-tools.database.set)
- description and source-code
```javascript
set = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
}

return prompt(options, [{
  type: 'confirm',
  name: 'collectUsage',
  message: 'Allow Firebase to collect anonymous CLI usage information?'
}]).then(function() {
  configstore.set('usage', options.collectUsage);
  return auth.login(options.localhost);
}).then(function(result) {
  configstore.set('user', result.user);
  configstore.set('tokens', result.tokens);
  // store login scopes in case mandatory scopes grow over time
  configstore.set('loginScopes', result.scopes);
  // remove old session token, if it exists
...
```

#### <a name="apidoc.element.firebase-tools.database.update"></a>[function <span class="apidocSignatureSpan">firebase-tools.database.</span>update ()](#apidoc.element.firebase-tools.database.update)
- description and source-code
```javascript
update = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_get"></a>[module firebase-tools.database_get](#apidoc.module.firebase-tools.database_get)

#### <a name="apidoc.element.firebase-tools.database_get._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_get.</span>_action (path, options)](#apidoc.element.firebase-tools.database_get._action)
- description and source-code
```javascript
_action = function (path, options) {
  if (!_.startsWith(path, '/')) {
    return utils.reject('Path must begin with /', {exit: 1});
  }

  var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';
  var query = {};
  if (options.shallow) { query.shallow = 'true'; }
  if (options.pretty) { query.print = 'pretty'; }
  if (options.export) { query.format = 'export'; }
  if (options.orderByKey) { options.orderBy = '$key'; }
  if (options.orderByValue) { options.orderBy = '$value'; }
  _applyStringOpts(query, options, ['limitToFirst', 'limitToLast'], ['orderBy', 'startAt', 'endAt', 'equalTo']);

  url += querystring.stringify(query);

  var reqOptions = {
    url: url
  };

  return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
    return new RSVP.Promise(function(resolve, reject) {
      var fileOut = !!options.output;
      var outStream = fileOut ? fs.createWriteStream(options.output) : process.stdout;
      var erroring;
      var errorResponse = '';
      var response;

      request.get(reqOptionsWithToken)
        .on('response', function(res) {
          response = res;
          if (response.statusCode >= 400) {
            erroring = true;
          }
        })
        .on('data', function(chunk) {
          if (erroring) {
            errorResponse += chunk;
          } else {
            outStream.write(chunk);
          }
        })
        .on('end', function() {
          outStream.write('\n');
          if (erroring) {
            try {
              var data = JSON.parse(errorResponse);
              return reject(responseToError(response, data));
            } catch (e) {
              return reject(new FirebaseError('Malformed JSON response', {
                exit: 2,
                original: e
              }));
            }
          }
          return resolve();
        })
        .on('error', reject);
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_profile"></a>[module firebase-tools.database_profile](#apidoc.module.firebase-tools.database_profile)

#### <a name="apidoc.element.firebase-tools.database_profile._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_profile.</span>_action (options)](#apidoc.element.firebase-tools.database_profile._action)
- description and source-code
```javascript
_action = function (options) {
  // Validate options
  if (options.raw && options.input) {
    return utils.reject('Cannot specify both an input file and raw format', {exit: 1});
  } else if (options.parent.json && options.raw) {
    return utils.reject('Cannot output raw data in json format', {exit: 1});
  } else if (options.input && _.has(options, 'duration')) {
    return utils.reject('Cannot specify a duration for input files', {exit: 1});
  } else if (_.has(options, 'duration') && options.duration <= 0) {
    return utils.reject('Must specify a positive number of seconds', {exit: 1});
  }

  return profiler(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_push"></a>[module firebase-tools.database_push](#apidoc.module.firebase-tools.database_push)

#### <a name="apidoc.element.firebase-tools.database_push._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_push.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_push._action)
- description and source-code
```javascript
_action = function (path, infile, options) {
  if (!_.startsWith(path, '/')) {
    return utils.reject('Path must begin with /', {exit: 1});
  }

  var inStream = utils.stringToStream(options.data) || (infile ? fs.createReadStream(infile) : process.stdin);
  var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';

  if (!infile && !options.data) {
    utils.explainStdin();
  }

  var reqOptions = {
    url: url,
    json: true
  };

  return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
    return new RSVP.Promise(function(resolve, reject) {
      inStream.pipe(request.post(reqOptionsWithToken, function(err, res, body) {
        logger.info();
        if (err) {
          return reject(new FirebaseError('Unexpected error while pushing data', {exit: 2}));
        } else if (res.statusCode >= 400) {
          return reject(responseToError(res, body));
        }

        if (!_.endsWith(path, '/')) {
          path += '/';
        }

        var consoleUrl = utils.consoleUrl(options.project, '/database/data' + path + body.name);
        var refurl = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + body.name;

        utils.logSuccess('Data pushed successfully');
        logger.info();
        logger.info(chalk.bold('View data at:'), consoleUrl);
        return resolve(new Firebase(refurl));
      }));
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_remove"></a>[module firebase-tools.database_remove](#apidoc.module.firebase-tools.database_remove)

#### <a name="apidoc.element.firebase-tools.database_remove._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_remove.</span>_action (path, options)](#apidoc.element.firebase-tools.database_remove._action)
- description and source-code
```javascript
_action = function (path, options) {
  if (!_.startsWith(path, '/')) {
    return utils.reject('Path must begin with /', {exit: 1});
  }

  return prompt(options, [{
    type: 'confirm',
    name: 'confirm',
    default: false,
    message: 'You are about to remove all data at ' + chalk.cyan(utils.addSubdomain(api.realtimeOrigin, options.instance) + path
) + '. Are you sure?'
  }]).then(function() {
    if (!options.confirm) {
      return utils.reject('Command aborted.', {exit: 1});
    }
    var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';
    var reqOptions = {
      url: url,
      json: true
    };

    return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
      return new RSVP.Promise(function(resolve, reject) {
        request.del(reqOptionsWithToken, function(err, res, body) {
          if (err) {
            return reject(new FirebaseError('Unexpected error while removing data', {exit: 2}));
          } else if (res.statusCode >= 400) {
            return reject(responseToError(res, body));
          }

          utils.logSuccess('Data removed successfully');
          return resolve();
        });
      });
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_set"></a>[module firebase-tools.database_set](#apidoc.module.firebase-tools.database_set)

#### <a name="apidoc.element.firebase-tools.database_set._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_set.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_set._action)
- description and source-code
```javascript
_action = function (path, infile, options) {
  if (!_.startsWith(path, '/')) {
    return utils.reject('Path must begin with /', {exit: 1});
  }

  return prompt(options, [{
    type: 'confirm',
    name: 'confirm',
    default: false,
    message: 'You are about to overwrite all data at ' + chalk.cyan(utils.addSubdomain(api.realtimeOrigin, options.instance) + path
) + '. Are you sure?'
  }]).then(function() {
    if (!options.confirm) {
      return utils.reject('Command aborted.', {exit: 1});
    }

    var inStream = utils.stringToStream(options.data) || (infile ? fs.createReadStream(infile) : process.stdin);
    var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';

    if (!infile && !options.data) {
      utils.explainStdin();
    }

    var reqOptions = {
      url: url,
      json: true
    };

    return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
      return new RSVP.Promise(function(resolve, reject) {
        inStream.pipe(request.put(reqOptionsWithToken, function(err, res, body) {
          logger.info();
          if (err) {
            return reject(new FirebaseError('Unexpected error while setting data', {exit: 2}));
          } else if (res.statusCode >= 400) {
            return reject(responseToError(res, body));
          }

          utils.logSuccess('Data persisted successfully');
          logger.info();
          logger.info(chalk.bold('View data at:'), utils.consoleUrl(options.project, '/database/data' + path));
          return resolve();
        }));
      });
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.database_update"></a>[module firebase-tools.database_update](#apidoc.module.firebase-tools.database_update)

#### <a name="apidoc.element.firebase-tools.database_update._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.database_update.</span>_action (path, infile, options)](#apidoc.element.firebase-tools.database_update._action)
- description and source-code
```javascript
_action = function (path, infile, options) {
  if (!_.startsWith(path, '/')) {
    return utils.reject('Path must begin with /', {exit: 1});
  }

  return prompt(options, [{
    type: 'confirm',
    name: 'confirm',
    default: false,
    message: 'You are about to modify data at ' + chalk.cyan(utils.addSubdomain(api.realtimeOrigin, options.instance) + path) + '.
Are you sure?'
  }]).then(function() {
    if (!options.confirm) {
      return utils.reject('Command aborted.', {exit: 1});
    }

    var inStream = utils.stringToStream(options.data) || (infile ? fs.createReadStream(infile) : process.stdin);
    var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';

    if (!infile && !options.data) {
      utils.explainStdin();
    }

    var reqOptions = {
      url: url,
      json: true
    };

    return api.addRequestHeaders(reqOptions).then(function(reqOptionsWithToken) {
      return new RSVP.Promise(function(resolve, reject) {
        inStream.pipe(request.patch(reqOptionsWithToken, function(err, res, body) {
          logger.info();
          if (err) {
            return reject(new FirebaseError('Unexpected error while setting data', {exit: 2}));
          } else if (res.statusCode >= 400) {
            return reject(responseToError(res, body));
          }

          utils.logSuccess('Data updated successfully');
          logger.info();
          logger.info(chalk.bold('View data at:'), utils.consoleUrl(options.project, '/database/data' + path));
          return resolve();
        }));
      });
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.deploy"></a>[module firebase-tools.deploy](#apidoc.module.firebase-tools.deploy)

#### <a name="apidoc.element.firebase-tools.deploy._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.deploy.</span>_action (options)](#apidoc.element.firebase-tools.deploy._action)
- description and source-code
```javascript
_action = function (options) {
  var targets = VALID_TARGETS.filter(function(t) {
    return options.config.has(t);
  });
  if (options.only && options.except) {
    return utils.reject('Cannot specify both --only and --except', {exit: 1});
  }

  if (options.only) {
    targets = _.intersection(targets, options.only.split(','));
  } else if (options.except) {
    targets = _.difference(targets, options.except.split(','));
  }

  if (targets.length === 0) {
    return utils.reject('No deploy targets found. Valid targets: ' + VALID_TARGETS.join(','), {exit: 1});
  }

  return deploy(targets, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.ensureApiEnabled"></a>[module firebase-tools.ensureApiEnabled](#apidoc.module.firebase-tools.ensureApiEnabled)

#### <a name="apidoc.element.firebase-tools.ensureApiEnabled.enable"></a>[function <span class="apidocSignatureSpan">firebase-tools.ensureApiEnabled.</span>enable (projectId, apiName)](#apidoc.element.firebase-tools.ensureApiEnabled.enable)
- description and source-code
```javascript
enable = function (projectId, apiName) {
  return api.request('PATCH', '/v1/services/' + apiName + '/projectSettings/' + projectId + '?updateMask=usageSettings', {
    auth: true,
    data: {
      usageSettings: {consumerEnableStatus: 'ENABLED'}
    },
    origin: 'https://servicemanagement.googleapis.com'
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.ensureApiEnabled.ensure"></a>[function <span class="apidocSignatureSpan">firebase-tools.ensureApiEnabled.</span>ensure (projectId, apiName, prefix)](#apidoc.element.firebase-tools.ensureApiEnabled.ensure)
- description and source-code
```javascript
ensure = function (projectId, apiName, prefix) {
  utils.logBullet(chalk.bold.cyan(prefix + ':') + ' ensuring necessary APIs are enabled...');
  return _checkEnabled(projectId, apiName, prefix).then(function(isEnabled) {
    if (isEnabled) {
      return true;
    }

    utils.logWarning(chalk.bold.yellow(prefix + ':') + ' missing necessary APIs. Enabling now...');
    return _enableApiWithRetries(projectId, apiName, prefix);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.fsutils"></a>[module firebase-tools.fsutils](#apidoc.module.firebase-tools.fsutils)

#### <a name="apidoc.element.firebase-tools.fsutils.dirExistsSync"></a>[function <span class="apidocSignatureSpan">firebase-tools.fsutils.</span>dirExistsSync (path)](#apidoc.element.firebase-tools.fsutils.dirExistsSync)
- description and source-code
```javascript
dirExistsSync = function (path) {
  try {
    var stats = fs.lstatSync(path);
    return stats.isDirectory();
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.fsutils.fileExistsSync"></a>[function <span class="apidocSignatureSpan">firebase-tools.fsutils.</span>fileExistsSync (path)](#apidoc.element.firebase-tools.fsutils.fileExistsSync)
- description and source-code
```javascript
fileExistsSync = function (path) {
  try {
    var stats = fs.lstatSync(path);
    return stats.isFile();
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
...
    } else {
      _.set(this.data, target, this._materialize(target));
    }
  }
}, this);

// auto-detect functions from package.json in directory
if (this.projectDir && !this.get('functions.source') && fsutils.fileExistsSync(this.path('functions/package.json'))) {
  this.set('functions.source', 'functions');
}

// use 'public' as signal for legacy hosting since it's a required key
if (!this.data.hosting && this._src.public) {
  this.importLegacyHostingKeys();
}
...
```



# <a name="apidoc.module.firebase-tools.functions"></a>[module firebase-tools.functions](#apidoc.module.firebase-tools.functions)

#### <a name="apidoc.element.firebase-tools.functions.log"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions.</span>log ()](#apidoc.element.firebase-tools.functions.log)
- description and source-code
```javascript
log = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
## Using as a Module

The Firebase CLI can also be used programmatically as a standard Node module. Each command is exposed as a function that takes an
 options object and returns a Promise. For example:

'''js
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
token: process.env.FIREBASE_TOKEN,
...
```



# <a name="apidoc.module.firebase-tools.functions.config"></a>[module firebase-tools.functions.config](#apidoc.module.firebase-tools.functions.config)

#### <a name="apidoc.element.firebase-tools.functions.config.clone"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>clone ()](#apidoc.element.firebase-tools.functions.config.clone)
- description and source-code
```javascript
clone = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.functions.config.get"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>get ()](#apidoc.element.firebase-tools.functions.config.get)
- description and source-code
```javascript
get = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
      return new RSVP.Promise(function(resolve, reject) {
var fileOut = !!options.output;
var outStream = fileOut ? fs.createWriteStream(options.output) : process.stdout;
var erroring;
var errorResponse = '';
var response;

request.get(reqOptionsWithToken)
  .on('response', function(res) {
    response = res;
    if (response.statusCode >= 400) {
      erroring = true;
    }
  })
  .on('data', function(chunk) {
...
```

#### <a name="apidoc.element.firebase-tools.functions.config.set"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>set ()](#apidoc.element.firebase-tools.functions.config.set)
- description and source-code
```javascript
set = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
}

return prompt(options, [{
  type: 'confirm',
  name: 'collectUsage',
  message: 'Allow Firebase to collect anonymous CLI usage information?'
}]).then(function() {
  configstore.set('usage', options.collectUsage);
  return auth.login(options.localhost);
}).then(function(result) {
  configstore.set('user', result.user);
  configstore.set('tokens', result.tokens);
  // store login scopes in case mandatory scopes grow over time
  configstore.set('loginScopes', result.scopes);
  // remove old session token, if it exists
...
```

#### <a name="apidoc.element.firebase-tools.functions.config.unset"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions.config.</span>unset ()](#apidoc.element.firebase-tools.functions.config.unset)
- description and source-code
```javascript
unset = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
utils.logBullet('Checking feature configuration...');
var out = _.cloneDeep(options.config._src);
var changed = false;

_.forEach(MOVE_KEYS, function(dest, src) {
  if (_.has(out, src)) {
    _.set(out, dest, _.get(out, src));
    _.unset(out, src);
    changed = true;
  }
});

utils.logBullet('Checking "firebase" key...');
var instance = out.firebase;
var rcfile;
...
```



# <a name="apidoc.module.firebase-tools.functionsConfig"></a>[module firebase-tools.functionsConfig](#apidoc.module.firebase-tools.functionsConfig)

#### <a name="apidoc.element.firebase-tools.functionsConfig.ensureApi"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>ensureApi (options)](#apidoc.element.firebase-tools.functionsConfig.ensureApi)
- description and source-code
```javascript
ensureApi = function (options) {
  var projectId = getProjectId(options);
  return ensureApiEnabled(projectId, 'runtimeconfig.googleapis.com', 'runtimeconfig');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.getFirebaseConfig"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>getFirebaseConfig (projectId, instance)](#apidoc.element.firebase-tools.functionsConfig.getFirebaseConfig)
- description and source-code
```javascript
getFirebaseConfig = function (projectId, instance) {
  return RSVP.all([storage.buckets.getDefault(projectId), apikeys.getServerKey(projectId)])
  .then(function(results) {
    return {
      databaseURL: utils.addSubdomain(api.realtimeOrigin, instance),
      storageBucket: results[0],
      apiKey: results[1],
      authDomain: instance + '.firebaseapp.com'
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.idsToVarName"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>idsToVarName (projectId, configId, varId)](#apidoc.element.firebase-tools.functionsConfig.idsToVarName)
- description and source-code
```javascript
idsToVarName = function (projectId, configId, varId) {
  return  _.join(['projects', projectId, 'configs', configId, 'variables', varId], '/');
}
```
- example usage
```shell
...
var metaPath = 'projects/' + projectId + '/configs/firebase/variables/meta';
return runtimeconfig.variables.get(metaPath).then(function(result) {
  var metaVal = JSON.parse(result.text);
  if (!_.has(metaVal, 'version')) {
    logger.info('You do not have any legacy config variables.');
    return null;
  }
  var latestVarPath = functionsConfig.idsToVarName(projectId, 'firebase', metaVal.version);
  return runtimeconfig.variables.get(latestVarPath);
}).then(function(latest) {
  if (latest !== null) {
    var latestVal = JSON.parse(latest.text);
    logger.info(JSON.stringify(latestVal, null, 2));
    return latestVal;
  }
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.materializeAll"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>materializeAll (projectId)](#apidoc.element.firebase-tools.functionsConfig.materializeAll)
- description and source-code
```javascript
materializeAll = function (projectId) {
  var output = {};
  return runtimeconfig.configs.list(projectId).then(function(configs) {
    return RSVP.all(_.map(configs, function(config) {
      if (config.name.match(new RegExp('configs/firebase'))) { // ignore firebase config
        return RSVP.resolve();
      }
      return exports.materializeConfig(config.name, output);
    })).then(function() {
      return output;
    });
  });
}
```
- example usage
```shell
...
var logger = require('../lib/logger');
var requireAccess = require('../lib/requireAccess');
var scopes = require('../lib/scopes');
var functionsConfig = require('../lib/functionsConfig');

function _materialize(projectId, path) {
if (_.isUndefined(path)) {
  return functionsConfig.materializeAll(projectId);
}
var parts = path.split('.');
var configId = parts[0];
var configName = _.join(['projects', projectId, 'configs', configId], '/');
return functionsConfig.materializeConfig(configName, {}).then(function(result) {
  var query =  _.chain(parts).join('.').value();
  return query ? _.get(result, query) : result;
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.materializeConfig"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>materializeConfig (configName, output)](#apidoc.element.firebase-tools.functionsConfig.materializeConfig)
- description and source-code
```javascript
materializeConfig = function (configName, output) {
  var _materializeVariable = function(varName) {
    return runtimeconfig.variables.get(varName).then(function(variable) {
      var id = exports.varNameToIds(variable.name);
      var key = id.config + '.' + id.variable.split('/').join('.');
      _.set(output, key, variable.text);
    });
  };

  var _traverseVariables = function(variables) {
    return RSVP.all(_.map(variables, function(variable) {
      return _materializeVariable(variable.name);
    }));
  };

  return runtimeconfig.variables.list(configName).then(function(variables) {
    return _traverseVariables(variables);
  }).then(function() {
    return output;
  });
}
```
- example usage
```shell
...
function _materialize(projectId, path) {
if (_.isUndefined(path)) {
  return functionsConfig.materializeAll(projectId);
}
var parts = path.split('.');
var configId = parts[0];
var configName = _.join(['projects', projectId, 'configs', configId], '/');
return functionsConfig.materializeConfig(configName, {}).then(function(result) {
  var query =  _.chain(parts).join('.').value();
  return query ? _.get(result, query) : result;
});
}

module.exports = new Command('functions:config:get [path]')
.description('fetch environment config stored at the given path')
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.parseSetArgs"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>parseSetArgs (args)](#apidoc.element.firebase-tools.functionsConfig.parseSetArgs)
- description and source-code
```javascript
parseSetArgs = function (args) {
  var parsed = [];
  _.forEach(args, function(arg) {
    var parts = arg.split('=');
    var key = parts[0];
    if (parts.length < 2) {
      throw new FirebaseError('Invalid argument ' + chalk.bold(arg) + ', must be in key=val format');
    }
    if (/[A-Z]/.test(key)) {
      throw new FirebaseError('Invalid config name ' + chalk.bold(key) + ', cannot use upper case.');
    }

    var id = _keyToIds(key);
    if (_.includes(exports.RESERVED_NAMESPACES, id.config.toLowerCase())) {
      throw new FirebaseError('Cannot set to reserved namespace ' + chalk.bold(id.config));
    }

    var val = parts.slice(1).join('='); // So that someone can have '=' within a variable value
    parsed.push({
      configId: id.config,
      varId: id.variable,
      val: val
    });
  });
  return parsed;
}
```
- example usage
```shell
...
  .before(requireAccess, [scopes.CLOUD_PLATFORM])
  .before(functionsConfig.ensureApi)
  .action(function(args, options) {
if (!args.length) {
  return utils.reject('Must supply at least one key/value pair, e.g. ' + chalk.bold('app.name="My App"'));
}
var projectId = getProjectId(options);
var parsed = functionsConfig.parseSetArgs(args);
var promises = [];

parsed.forEach(function(item) {
  promises.push(functionsConfig.setVariablesRecursive(projectId, item.configId, item.varId, item.val));
});

return RSVP.all(promises).then(function() {
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.parseUnsetArgs"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>parseUnsetArgs (args)](#apidoc.element.firebase-tools.functionsConfig.parseUnsetArgs)
- description and source-code
```javascript
parseUnsetArgs = function (args) {
  var parsed = [];
  args = args[0].split(',');
  _.forEach(args, function(key) {
    var id = _keyToIds(key);
    if (_.includes(exports.RESERVED_NAMESPACES, id.config.toLowerCase())) {
      throw new FirebaseError('Cannot unset reserved namespace ' + chalk.bold(id.config));
    }

    parsed.push({
      configId: id.config,
      varId: id.variable
    });
  });
  return parsed;
}
```
- example usage
```shell
...
.before(requireAccess, [scopes.CLOUD_PLATFORM])
.before(functionsConfig.ensureApi)
.action(function(args, options) {
  if (!args.length) {
    return utils.reject('Must supply at least one key, e.g. ' + chalk.bold('app.name'));
  }
  var projectId = getProjectId(options);
  var parsed = functionsConfig.parseUnsetArgs(args);
  return RSVP.all(_.map(parsed, function(item) {
    if (item.varId === '') {
      return runtimeconfig.configs.delete(projectId, item.configId);
    }
    return runtimeconfig.variables.delete(projectId, item.configId, item.varId);
  })).then(function() {
    utils.logSuccess('Environment updated.');
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.setVariablesRecursive"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>setVariablesRecursive (projectId, configId, varPath, val)](#apidoc.element.firebase-tools.functionsConfig.setVariablesRecursive)
- description and source-code
```javascript
setVariablesRecursive = function (projectId, configId, varPath, val) {
  try {
    var parsed = JSON.parse(val);
    if (!_.isPlainObject(parsed)) { // could be a number, etc.
      return _setVariable(projectId, configId, varPath, val);
    } else if (parsed === null) {
      return _setVariable(projectId, configId, varPath, 'null');
    }
    return RSVP.all(_.map(parsed, function(item, key) {
      var newVarPath = varPath ? _.join([varPath, key], '/') : key;
      if (_.isPlainObject(parsed)) {
        item = JSON.stringify(item);
      }
      return exports.setVariablesRecursive(projectId, configId, newVarPath, item);
    }));
  } catch (e) {
    return _setVariable(projectId, configId, varPath, val);
  }
}
```
- example usage
```shell
...
  return utils.reject('Must supply at least one key/value pair, e.g. ' + chalk.bold('app.name="My App"'));
}
var projectId = getProjectId(options);
var parsed = functionsConfig.parseSetArgs(args);
var promises = [];

parsed.forEach(function(item) {
  promises.push(functionsConfig.setVariablesRecursive(projectId, item.configId, item.varId, item.val));
});

return RSVP.all(promises).then(function() {
  utils.logSuccess('Functions config updated.');
  logger.info('\nPlease deploy your functions for the change to take effect by running '
    + chalk.bold('firebase deploy --only functions') + '\n');
});
...
```

#### <a name="apidoc.element.firebase-tools.functionsConfig.varNameToIds"></a>[function <span class="apidocSignatureSpan">firebase-tools.functionsConfig.</span>varNameToIds (varName)](#apidoc.element.firebase-tools.functionsConfig.varNameToIds)
- description and source-code
```javascript
varNameToIds = function (varName) {
  return {
    config: varName.match(new RegExp('/configs/(.+)/variables/'))[1],
    variable: varName.match(new RegExp('/variables/(.+)'))[1]
  };
}
```
- example usage
```shell
...
  return _setVariable(projectId, configId, varPath, val);
}
};

exports.materializeConfig = function(configName, output) {
var _materializeVariable = function(varName) {
  return runtimeconfig.variables.get(varName).then(function(variable) {
    var id = exports.varNameToIds(variable.name);
    var key = id.config + '.' + id.variable.split('/').join('.');
    _.set(output, key, variable.text);
  });
};

var _traverseVariables = function(variables) {
  return RSVP.all(_.map(variables, function(variable) {
...
```



# <a name="apidoc.module.firebase-tools.functions_config_clone"></a>[module firebase-tools.functions_config_clone](#apidoc.module.firebase-tools.functions_config_clone)

#### <a name="apidoc.element.firebase-tools.functions_config_clone._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions_config_clone.</span>_action (options)](#apidoc.element.firebase-tools.functions_config_clone._action)
- description and source-code
```javascript
_action = function (options) {
  var projectId = getProjectId(options);
  if (!options.from) {
    return utils.reject('Must specify a source project in ' + chalk.bold('--from <projectId>') + ' option.');
  } else if (options.from === projectId) {
    return utils.reject('From project and destination can\'t be the same project.');
  } else if (options.only && options.except) {
    return utils.reject('Cannot use both --only and --except at the same time.');
  }

  var only;
  var except;
  if (options.only) {
    only = options.only.split(',');
  } else if (options.except) {
    except = options.except.split(',');
  }

  return functionsConfigClone(options.from, projectId, only, except).then(function() {
    utils.logSuccess('Cloned functions config from ' + chalk.bold(options.from) + ' into ' + chalk.bold(projectId));
    logger.info('\nPlease deploy your functions for the change to take effect by running '
      + chalk.bold('firebase deploy --only functions') + '\n');
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.functions_config_get"></a>[module firebase-tools.functions_config_get](#apidoc.module.firebase-tools.functions_config_get)

#### <a name="apidoc.element.firebase-tools.functions_config_get._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions_config_get.</span>_action (path, options)](#apidoc.element.firebase-tools.functions_config_get._action)
- description and source-code
```javascript
_action = function (path, options) {
  return _materialize(getProjectId(options), path).then(function(result) {
    logger.info(JSON.stringify(result, null, 2));
    return result;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.functions_config_legacy"></a>[module firebase-tools.functions_config_legacy](#apidoc.module.firebase-tools.functions_config_legacy)

#### <a name="apidoc.element.firebase-tools.functions_config_legacy._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions_config_legacy.</span>_action (options)](#apidoc.element.firebase-tools.functions_config_legacy._action)
- description and source-code
```javascript
_action = function (options) {
  var projectId = getProjectId(options);
  var metaPath = 'projects/' + projectId + '/configs/firebase/variables/meta';
  return runtimeconfig.variables.get(metaPath).then(function(result) {
    var metaVal = JSON.parse(result.text);
    if (!_.has(metaVal, 'version')) {
      logger.info('You do not have any legacy config variables.');
      return null;
    }
    var latestVarPath = functionsConfig.idsToVarName(projectId, 'firebase', metaVal.version);
    return runtimeconfig.variables.get(latestVarPath);
  }).then(function(latest) {
    if (latest !== null) {
      var latestVal = JSON.parse(latest.text);
      logger.info(JSON.stringify(latestVal, null, 2));
      return latestVal;
    }
  }).catch(function(err) {
    if (_.get(err, 'context.response.statusCode') === 404) {
      logger.info('You do not have any legacy config variables.');
      return null;
    }
    return RSVP.reject(err);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.functions_config_set"></a>[module firebase-tools.functions_config_set](#apidoc.module.firebase-tools.functions_config_set)

#### <a name="apidoc.element.firebase-tools.functions_config_set._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions_config_set.</span>_action (args, options)](#apidoc.element.firebase-tools.functions_config_set._action)
- description and source-code
```javascript
_action = function (args, options) {
  if (!args.length) {
    return utils.reject('Must supply at least one key/value pair, e.g. ' + chalk.bold('app.name="My App"'));
  }
  var projectId = getProjectId(options);
  var parsed = functionsConfig.parseSetArgs(args);
  var promises = [];

  parsed.forEach(function(item) {
    promises.push(functionsConfig.setVariablesRecursive(projectId, item.configId, item.varId, item.val));
  });

  return RSVP.all(promises).then(function() {
    utils.logSuccess('Functions config updated.');
    logger.info('\nPlease deploy your functions for the change to take effect by running '
      + chalk.bold('firebase deploy --only functions') + '\n');
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.functions_config_unset"></a>[module firebase-tools.functions_config_unset](#apidoc.module.firebase-tools.functions_config_unset)

#### <a name="apidoc.element.firebase-tools.functions_config_unset._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.functions_config_unset.</span>_action (args, options)](#apidoc.element.firebase-tools.functions_config_unset._action)
- description and source-code
```javascript
_action = function (args, options) {
  if (!args.length) {
    return utils.reject('Must supply at least one key, e.g. ' + chalk.bold('app.name'));
  }
  var projectId = getProjectId(options);
  var parsed = functionsConfig.parseUnsetArgs(args);
  return RSVP.all(_.map(parsed, function(item) {
    if (item.varId === '') {
      return runtimeconfig.configs.delete(projectId, item.configId);
    }
    return runtimeconfig.variables.delete(projectId, item.configId, item.varId);
  })).then(function() {
    utils.logSuccess('Environment updated.');
    logger.info('\nPlease deploy your functions for the change to take effect by running '
      + chalk.bold('firebase deploy --only functions') + '\n');
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.help"></a>[module firebase-tools.help](#apidoc.module.firebase-tools.help)

#### <a name="apidoc.element.firebase-tools.help._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.help.</span>_action (commandName)](#apidoc.element.firebase-tools.help._action)
- description and source-code
```javascript
_action = function (commandName) {
  var cmd = this.client.getCommand(commandName);
  if (cmd) {
    cmd.outputHelp();
  } else if (commandName) {
    logger.warn();
    utils.logWarning(chalk.bold(commandName) + ' is not a valid command. See below for valid commands');
    this.client.cli.outputHelp();
  } else {
    this.client.cli.outputHelp();
    logger.info();
    logger.info('  To get help with a specific command, type', chalk.bold('firebase help [command_name]'));
    logger.info();
  }

  RSVP.resolve();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.hosting"></a>[module firebase-tools.hosting](#apidoc.module.firebase-tools.hosting)

#### <a name="apidoc.element.firebase-tools.hosting.disable"></a>[function <span class="apidocSignatureSpan">firebase-tools.hosting.</span>disable ()](#apidoc.element.firebase-tools.hosting.disable)
- description and source-code
```javascript
disable = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.hosting_disable"></a>[module firebase-tools.hosting_disable](#apidoc.module.firebase-tools.hosting_disable)

#### <a name="apidoc.element.firebase-tools.hosting_disable._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.hosting_disable.</span>_action (options)](#apidoc.element.firebase-tools.hosting_disable._action)
- description and source-code
```javascript
_action = function (options) {
  return prompt(options, [
    {
      type: 'confirm',
      name: 'confirm',
      message: 'Are you sure you want to disable Firebase Hosting?\n  ' + chalk.bold.underline('This will immediately make your
site inaccessible!')
    }
  ]).then(function() {
    if (!options.confirm) {
      return RSVP.resolve();
    }

    return api.request('POST', '/v1/projects/' + encodeURIComponent(options.project) + '/releases', {
      auth: true,
      data: {
        hosting: {
          disabled: true
        }
      },
      origin: api.deployOrigin
    });
  }).then(function() {
    if (options.confirm) {
      utils.logSuccess('Hosting has been disabled for ' + chalk.bold(options.project) + '. Deploy a new version to re-enable.');
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.init"></a>[module firebase-tools.init](#apidoc.module.firebase-tools.init)

#### <a name="apidoc.element.firebase-tools.init._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.init.</span>_action (feature, options)](#apidoc.element.firebase-tools.init._action)
- description and source-code
```javascript
_action = function (feature, options) {
  var cwd = options.cwd || process.cwd();

  var warnings = [];
  var warningText = '';
  if (_isOutside(homeDir, cwd)) {
    warnings.push('You are currently outside your home directory');
  }
  if (cwd === homeDir) {
    warnings.push('You are initializing your home directory as a Firebase project');
  }

  var config = Config.load(options, true);
  var existingConfig = !!config;
  if (!existingConfig) {
    config = new Config({}, {projectDir: cwd, cwd: cwd});
  } else {
    warnings.push('You are initializing in an existing Firebase project directory');
  }

  if (warnings.length) {
    warningText = '\nBefore we get started, keep in mind:\n\n  ' + chalk.yellow.bold('* ') + warnings.join('\n  ' + chalk.yellow
.bold('* ')) + '\n';
  }

  if (process.platform === 'darwin') {
    BANNER_TEXT = BANNER_TEXT.replace(/#/g, '🔥');
  }
  logger.info(chalk.yellow.bold(BANNER_TEXT) +
    '\nYou\'re about to initialize a Firebase project in this directory:\n\n  ' + chalk.bold(config.projectDir) + '\n' +
    warningText
  );

  var setup = {
    config: config._src,
    rcfile: config.readProjectFile('.firebaserc', {
      json: true,
      fallback: {}
    })
  };

  var choices = [
    {name: 'database', label: 'Database: Deploy Firebase Realtime Database Rules', checked: true},
    {name: 'functions', label: 'Functions: Configure and deploy Cloud Functions', checked: true},
    {name: 'hosting', label: 'Hosting: Configure and deploy Firebase Hosting sites', checked: true}
    // {name: 'storage', label: 'Storage: Deploy Firebase Storage Security Rules', checked: true}
  ];

  var next;
  // HACK: Windows Node has issues with selectables as the first prompt, so we
  // add an extra confirmation prompt that fixes the problem
  if (process.platform === 'win32') {
    next = prompt.once({
      type: 'confirm',
      message: 'Are you ready to proceed?'
    });
  } else {
    next = RSVP.resolve(true);
  }

  return next.then(function(proceed) {
    if (!proceed) {
      return utils.reject('Aborted by user.', {exit: 1});
    }

    if (feature) {
      setup.featureArg = true;
      setup.features = [feature];
      return undefined;
    }

    return prompt(setup, [{
      type: 'checkbox',
      name: 'features',
      message: 'What Firebase CLI features do you want to setup for this folder?',
      choices: prompt.convertLabeledListChoices(choices)
    }]);
  }).then(function() {
    if (!setup.featureArg) {
      setup.features = setup.features.map(function(feat) {
        return prompt.listLabelToValue(feat, choices);
      });
    }
    setup.features.unshift('project');
    return init(setup, config, options);
  }).then(function() {
    logger.info();
    utils.logBullet('Writing configuration info to ' + chalk.bold('firebase.json') + '...');
    config.writeProjectFile('firebase.json', setup.config);
    utils.logBullet('Writing project information to ' + chalk.bold('.firebaserc') + '...');
    config.writeProjectFile('.firebaserc', setup.rcfile);
    logger.info();
    utils.logSuccess('Firebase initialization complete!');

    if (setup.createProject) {
      logger.info();
      logger.info(chalk.bold.cyan('Project creation is only available from the Firebase Console'));
      logger.info('Please visit', chalk.underline('https://console.firebase.google.com'), 'to create a new project, then run', chalk
.bold('firebase use --add'));
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.list"></a>[module firebase-tools.list](#apidoc.module.firebase-tools.list)

#### <a name="apidoc.element.firebase-tools.list._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.list.</span>_action (options)](#apidoc.element.firebase-tools.list._action)
- description and source-code
```javascript
_action = function (options) {
  return api.getProjects().then(function(projects) {
    var tableHead = ['Name', 'Project ID / Instance', 'Permissions'];
    var table = new Table({
      head: tableHead,
      style: {head: ['yellow']}
    });

    var out = [];
    _.forEach(projects, function(data, projectId) {
      var project = {
        name: data.name,
        id: projectId,
        permission: data.permission,
        instance: data.instances.database[0]
      };

      var displayId = chalk.bold(projectId);
      if (data.instances.database[0] !== projectId) {
        displayId += '\n' + data.instances.database[0] + ' (instance)';
      }

      var displayPermission;
      switch (data.permission) {
      case 'own':
        displayPermission = chalk.cyan.bold('Owner');
        break;
      case 'edit':
        displayPermission = chalk.bold('Editor');
        break;
      case 'view':
      default:
        displayPermission = 'Viewer';
      }

      var displayName = data.name;
      if (options.project === projectId) {
        displayName = chalk.cyan.bold(displayName + ' (current)');
      }

      out.push(project);
      var row = [
        displayName,
        displayId,
        displayPermission
      ];
      table.push(row);
    });

    if (_.size(projects) === 0) {
      logger.info(chalk.bold('No projects found.'));
      logger.info();
      logger.info(
        chalk.bold.cyan('Projects missing?') + ' This version of the Firebase CLI is only compatible with\n' +
        'projects that have been upgraded to the new Firebase Console. To access your\n' +
        'firebase.com apps, use a previous version: ' + chalk.bold('npm install -g firebase-tools@^2.1')
      );
    } else {
      logger.info(table.toString());
    }
    return out;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.logger"></a>[module firebase-tools.logger](#apidoc.module.firebase-tools.logger)

#### <a name="apidoc.element.firebase-tools.logger.debug"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>debug (msg)](#apidoc.element.firebase-tools.logger.debug)
- description and source-code
```javascript
debug = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
var responseToError = require('./responseToError');
var refreshToken;
var commandScopes;
var scopes = require('./scopes');
var CLI_VERSION = require('../package.json').version;

var _request = function(options) {
logger.debug('>>> HTTP REQUEST',
  options.method,
  options.url,
  options.body || options.form || '',
  '\n',
  new Date().toString()
);
...
```

#### <a name="apidoc.element.firebase-tools.logger.error"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>error (msg)](#apidoc.element.firebase-tools.logger.error)
- description and source-code
```javascript
error = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
'data:update': 'database:update',
'deploy:hosting': 'deploy --only hosting',
'deploy:database': 'deploy --only database',
'prefs:token': 'login:ci'
};

program.action(function(cmd, cmd2) {
logger.error(
  chalk.bold.red('Error:'),
  chalk.bold(cmd), 'is not a Firebase command'
);

if (RENAMED_COMMANDS[cmd]) {
  logger.error();
  logger.error(chalk.bold(cmd) + ' has been renamed, please run', chalk.bold('firebase ' + RENAMED_COMMANDS[cmd]), 'instead');
...
```

#### <a name="apidoc.element.firebase-tools.logger.info"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>info (msg)](#apidoc.element.firebase-tools.logger.info)
- description and source-code
```javascript
info = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
  var exportOptions = checkRes;
  var writeStream = fs.createWriteStream(dataFile);
  if (exportOptions.format === 'json') {
    writeStream.write('{"users": [' + os.EOL);
  }
  exportOptions.writeStream = writeStream;
  exportOptions.batchSize = MAX_BATCH_SIZE;
  logger.info('Exporting accounts to ' + chalk.bold(dataFile));
  return serialExportUsers(projectId, exportOptions).then(function() {
    if (exportOptions.format === 'json') {
      writeStream.write(']}');
    }
    writeStream.end();
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.logger.log"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>log ()](#apidoc.element.firebase-tools.logger.log)
- description and source-code
```javascript
log = function () {
  var args = Array.prototype.slice.call(arguments, 0);
  if (args.length >= 2 && args[1] instanceof Error) {
    args[1] = args[1].stack;
  }
  return oldLogFunc.apply(this, args);
}
```
- example usage
```shell
...
## Using as a Module

The Firebase CLI can also be used programmatically as a standard Node module. Each command is exposed as a function that takes an
 options object and returns a Promise. For example:

'''js
var client = require('firebase-tools');
client.list().then(function(data) {
console.log(data);
}).catch(function(err) {
// handle error
});

client.deploy({
project: 'myfirebase',
token: process.env.FIREBASE_TOKEN,
...
```

#### <a name="apidoc.element.firebase-tools.logger.silly"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>silly (msg)](#apidoc.element.firebase-tools.logger.silly)
- description and source-code
```javascript
silly = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.logger.verbose"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>verbose (msg)](#apidoc.element.firebase-tools.logger.verbose)
- description and source-code
```javascript
verbose = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.logger.warn"></a>[function <span class="apidocSignatureSpan">firebase-tools.logger.</span>warn (msg)](#apidoc.element.firebase-tools.logger.warn)
- description and source-code
```javascript
warn = function (msg) {
  // build argument list (level, msg, ... [string interpolate], [{metadata}], [callback])
  var args = [level].concat(Array.prototype.slice.call(arguments));
  target.log.apply(target, args);
}
```
- example usage
```shell
...
module.exports = new Command('help [command]')
.description('display help information')
.action(function(commandName) {
  var cmd = this.client.getCommand(commandName);
  if (cmd) {
    cmd.outputHelp();
  } else if (commandName) {
    logger.warn();
    utils.logWarning(chalk.bold(commandName) + ' is not a valid command. See below for valid commands');
    this.client.cli.outputHelp();
  } else {
    this.client.cli.outputHelp();
    logger.info();
    logger.info('  To get help with a specific command, type', chalk.bold('firebase help [command_name]'));
    logger.info();
...
```



# <a name="apidoc.module.firebase-tools.login"></a>[module firebase-tools.login](#apidoc.module.firebase-tools.login)

#### <a name="apidoc.element.firebase-tools.login.login"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>login ()](#apidoc.element.firebase-tools.login.login)
- description and source-code
```javascript
login = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
...
.description('generate an access token for use in non-interactive environments')
.option('--no-localhost', 'copy and paste a code instead of starting a local server for authentication')
.action(function(options) {
  if (options.nonInteractive) {
    return utils.reject('Cannot run login:ci in non-interactive mode.', {exit: 1});
  }

  return auth.login(options.localhost).then(function(result) {
    logger.info();
    utils.logSuccess('Success! Use this token to login on a CI server:\n\n' +
      chalk.bold(result.tokens.refresh_token) + '\n\nExample: firebase deploy --token "$FIREBASE_TOKEN"\n');
    return result;
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.login.ci"></a>[function <span class="apidocSignatureSpan">firebase-tools.login.</span>ci ()](#apidoc.element.firebase-tools.login.ci)
- description and source-code
```javascript
ci = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.login_ci"></a>[module firebase-tools.login_ci](#apidoc.module.firebase-tools.login_ci)

#### <a name="apidoc.element.firebase-tools.login_ci._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.login_ci.</span>_action (options)](#apidoc.element.firebase-tools.login_ci._action)
- description and source-code
```javascript
_action = function (options) {
  if (options.nonInteractive) {
    return utils.reject('Cannot run login:ci in non-interactive mode.', {exit: 1});
  }

  return auth.login(options.localhost).then(function(result) {
    logger.info();
    utils.logSuccess('Success! Use this token to login on a CI server:\n\n' +
      chalk.bold(result.tokens.refresh_token) + '\n\nExample: firebase deploy --token "$FIREBASE_TOKEN"\n');
    return result;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.logout"></a>[module firebase-tools.logout](#apidoc.module.firebase-tools.logout)

#### <a name="apidoc.element.firebase-tools.logout._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.logout.</span>_action (options)](#apidoc.element.firebase-tools.logout._action)
- description and source-code
```javascript
_action = function (options) {
  var user = configstore.get('user');
  var tokens = configstore.get('tokens');
  var currentToken = _.get(tokens, 'refresh_token');
  var token = utils.getInheritedOption(options, 'token') || currentToken;
  api.setToken(token);
  var next;
  if (token) {
    next = auth.logout(token);
  } else {
    next = RSVP.resolve();
  }

  var cleanup = function() {
    if (token || user || tokens) {
      var msg = 'Logged out';
      if (token === currentToken) {
        if (user) {
          msg += ' from ' + chalk.bold(user.email);
        }
      } else {
        msg += ' token "' + chalk.bold(token) + '"';
      }
      utils.logSuccess(msg);
    } else {
      logger.info('No need to logout, not logged in');
    }
  };

  return next.then(cleanup, function() {
    utils.logWarning('Invalid refresh token, did not need to deauthorize');
    cleanup();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.open"></a>[module firebase-tools.open](#apidoc.module.firebase-tools.open)

#### <a name="apidoc.element.firebase-tools.open._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.open.</span>_action (linkName, options)](#apidoc.element.firebase-tools.open._action)
- description and source-code
```javascript
_action = function (linkName, options) {
  var link = _.find(LINKS, {arg: linkName});
  if (linkName && !link) {
    return utils.reject('Unrecognized link name. Valid links are:\n\n' + _.map(LINKS, 'arg').join('\n'));
  }

  var next = RSVP.resolve(link);
  if (!link) {
    next = prompt.once({
      type: 'list',
      message: 'What link would you like to open?',
      choices: CHOICES
    }).then(function(result) {
      return _.find(LINKS, {name: result});
    });
  }

  return next.then(function(finalLink) {
    var url;
    if (finalLink.consoleUrl) {
      url = utils.consoleUrl(options.project, finalLink.consoleUrl);
    } else if (finalLink.url) {
      url = finalLink.url;
    } else if (finalLink.arg === 'hosting:site') {
      url = utils.addSubdomain(api.hostingOrigin, options.instance);
    } else if (finalLink.arg === 'functions') {
      url = 'https://console.firebase.google.com/project/' + options.project + '/functions/list';
    } else if (finalLink.arg === 'functions:log') {
      url = 'https://console.developers.google.com/logs/viewer?resource=cloudfunctions.googleapis.com&project=' + options.project
;
    }

    logger.info(chalk.bold.cyan('Tip: ') + 'You can also run ' + chalk.bold.underline('firebase open ' + finalLink.arg));
    logger.info();
    logger.info('Opening ' + chalk.bold(finalLink.name) + ' link in your default browser:');
    logger.info(chalk.bold.underline(url));

    open(url);
    return RSVP.resolve(url);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.prompt"></a>[module firebase-tools.prompt](#apidoc.module.firebase-tools.prompt)

#### <a name="apidoc.element.firebase-tools.prompt.prompt"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>prompt (options, questions)](#apidoc.element.firebase-tools.prompt.prompt)
- description and source-code
```javascript
prompt = function (options, questions) {
  return new RSVP.Promise(function(resolve, reject) {
    var prompts = [];
    for (var i = 0; i < questions.length; i++) {
      if (!options[questions[i].name]) {
        prompts.push(questions[i]);
      }
    }

    if (prompts.length && options.nonInteractive) {
      return reject(new FirebaseError('Missing required options (' + _.uniq(_.map(prompts, 'name')).join(', ') + ') while running
 in non-interactive mode', {
        children: prompts,
        exit: 1
      }));
    }

    return inquirer.prompt(prompts, function(answers) {
      _.forEach(answers, function(v, k) {
        options[k] = v;
      });
      return resolve(options);
    });
  });
}
```
- example usage
```shell
...
    if (prompts.length && options.nonInteractive) {
      return reject(new FirebaseError('Missing required options (' + _.uniq(_.map(prompts, 'name')).join(', ') + ') while running
 in non-interactive mode', {
        children: prompts,
        exit: 1
      }));
    }

    return inquirer.prompt(prompts, function(answers) {
      _.forEach(answers, function(v, k) {
        options[k] = v;
      });
      return resolve(options);
    });
  });
};
...
```

#### <a name="apidoc.element.firebase-tools.prompt.convertLabeledListChoices"></a>[function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>convertLabeledListChoices (choices)](#apidoc.element.firebase-tools.prompt.convertLabeledListChoices)
- description and source-code
```javascript
convertLabeledListChoices = function (choices) {
  return choices.map(function(choice) {
    return {checked: choice.checked, name: choice.label};
  });
}
```
- example usage
```shell
...
    return undefined;
  }

  return prompt(setup, [{
    type: 'checkbox',
    name: 'features',
    message: 'What Firebase CLI features do you want to setup for this folder?',
    choices: prompt.convertLabeledListChoices(choices)
  }]);
}).then(function() {
  if (!setup.featureArg) {
    setup.features = setup.features.map(function(feat) {
      return prompt.listLabelToValue(feat, choices);
    });
  }
...
```

#### <a name="apidoc.element.firebase-tools.prompt.listLabelToValue"></a>[function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>listLabelToValue (label, choices)](#apidoc.element.firebase-tools.prompt.listLabelToValue)
- description and source-code
```javascript
listLabelToValue = function (label, choices) {
  for (var i = 0; i < choices.length; i++) {
    if (choices[i].label === label) {
      return choices[i].name;
    }
  }
}
```
- example usage
```shell
...
    name: 'features',
    message: 'What Firebase CLI features do you want to setup for this folder?',
    choices: prompt.convertLabeledListChoices(choices)
  }]);
}).then(function() {
  if (!setup.featureArg) {
    setup.features = setup.features.map(function(feat) {
      return prompt.listLabelToValue(feat, choices);
    });
  }
  setup.features.unshift('project');
  return init(setup, config, options);
}).then(function() {
  logger.info();
  utils.logBullet('Writing configuration info to ' + chalk.bold('firebase.json') + '...');
...
```

#### <a name="apidoc.element.firebase-tools.prompt.once"></a>[function <span class="apidocSignatureSpan">firebase-tools.prompt.</span>once (question)](#apidoc.element.firebase-tools.prompt.once)
- description and source-code
```javascript
once = function (question) {
  question.name = question.name || 'question';
  return prompt({}, [question]).then(function(answers) { return answers[question.name]; });
}
```
- example usage
```shell
...
  // {name: 'storage', label: 'Storage: Deploy Firebase Storage Security Rules', checked: true}
];

var next;
// HACK: Windows Node has issues with selectables as the first prompt, so we
// add an extra confirmation prompt that fixes the problem
if (process.platform === 'win32') {
  next = prompt.once({
    type: 'confirm',
    message: 'Are you ready to proceed?'
  });
} else {
  next = RSVP.resolve(true);
}
...
```



# <a name="apidoc.module.firebase-tools.serve"></a>[module firebase-tools.serve](#apidoc.module.firebase-tools.serve)

#### <a name="apidoc.element.firebase-tools.serve._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.serve.</span>_action (options)](#apidoc.element.firebase-tools.serve._action)
- description and source-code
```javascript
_action = function (options) {
  logger.info('Starting Firebase development server...');
  logger.info();

  if (options.config) {
    logger.info(chalk.bold('Project Directory:'), options.config.projectDir);
  } else {
    utils.logWarning('No Firebase project directory detected. Serving static content from ' + chalk.bold(options.cwd || process.
cwd()));
  }

  return startServer(options).then(function() {
    return new RSVP.Promise(function(resolve) {
      process.on('SIGINT', function() {
        logger.info('Shutting down...');
        resolve();
      });
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.setup"></a>[module firebase-tools.setup](#apidoc.module.firebase-tools.setup)

#### <a name="apidoc.element.firebase-tools.setup.web"></a>[function <span class="apidocSignatureSpan">firebase-tools.setup.</span>web ()](#apidoc.element.firebase-tools.setup.web)
- description and source-code
```javascript
web = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.setup_web"></a>[module firebase-tools.setup_web](#apidoc.module.firebase-tools.setup_web)

#### <a name="apidoc.element.firebase-tools.setup_web._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.setup_web.</span>_action (options)](#apidoc.element.firebase-tools.setup_web._action)
- description and source-code
```javascript
_action = function (options) {
  return fetchWebSetup(options).then(function(config) {
    logger.info(JS_TEMPLATE.replace('{/*--CONFIG--*/}', JSON.stringify(config, null, 2)));
    return RSVP.resolve(config);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.tools"></a>[module firebase-tools.tools](#apidoc.module.firebase-tools.tools)

#### <a name="apidoc.element.firebase-tools.tools.migrate"></a>[function <span class="apidocSignatureSpan">firebase-tools.tools.</span>migrate ()](#apidoc.element.firebase-tools.tools.migrate)
- description and source-code
```javascript
migrate = function () {
  var args = _.toArray(arguments);
  // always provide at least an empty object for options
  if (args.length === 0) {
    args.push({});
  }
  var options = _.last(args);

  try {
    var befores = [self._prepare].concat(self._befores);
    var result = befores.shift().call(self, options);
    befores.forEach(function(before) {
      result = result.then(function() {
        return before.fn.call(self, options, before.args);
      });
    });
    return result.then(function() {
      return self._action.apply(self, args);
    });
  } catch (e) {
    return RSVP.reject(e);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.tools_migrate"></a>[module firebase-tools.tools_migrate](#apidoc.module.firebase-tools.tools_migrate)

#### <a name="apidoc.element.firebase-tools.tools_migrate._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.tools_migrate.</span>_action (options)](#apidoc.element.firebase-tools.tools_migrate._action)
- description and source-code
```javascript
_action = function (options) {
  if (!options.config) {
    return utils.reject('Must run ' + chalk.bold('tools:migrate') + ' from a directory with a firebase.json');
  }

  utils.logBullet('Checking feature configuration...');
  var out = _.cloneDeep(options.config._src);
  var changed = false;

  _.forEach(MOVE_KEYS, function(dest, src) {
    if (_.has(out, src)) {
      _.set(out, dest, _.get(out, src));
      _.unset(out, src);
      changed = true;
    }
  });

  utils.logBullet('Checking "firebase" key...');
  var instance = out.firebase;
  var rcfile;
  var next;
  var projectId;
  if (instance) {
    next = identifierToProjectId(instance).then(function(result) {
      projectId = result;
      if (projectId) {
        rcfile = {projects: {default: projectId}};
        _.unset(out, 'firebase');
      } else {
        return utils.reject('Could not find Firebase project corresponding to ' + chalk.bold(instance) + '.\nPlease ensure it has
 been migrated to the new console before proceeding.');
      }
    });
    rcfile = {projects: {default: instance}};

    changed = true;
  } else {
    next = RSVP.resolve();
  }

  return next.then(function() {
    if (!changed) {
      logger.info();
      utils.logSuccess('No action required, your firebase.json is all up to date!');
      return true;
    }

    logger.info();
    logger.info(chalk.gray.bold('# preview: updated contents of firebase.json'));
    logger.info();
    logger.info(JSON.stringify(out, null, 2));
    logger.info();

    if (options.confirm) {
      next = RSVP.resolve(true);
    } else {
      next = prompt.once({
        type: 'confirm',
        message: 'Write new config to ' + chalk.underline('firebase.json') + '?',
        default: true
      });
    }

    return next.then(function(confirmed) {
      if (confirmed) {
        options.config.writeProjectFile('firebase.json', out);
        utils.logSuccess('Migrated ' + chalk.bold('firebase.json') + ' successfully');
        if (projectId) {
          options.config.writeProjectFile('.firebaserc', rcfile);
          utils.makeActiveProject(options.projectRoot, projectId);
          utils.logSuccess('Set default project to ' + chalk.bold(projectId));
        }
      } else {
        return utils.reject('Migration aborted by user.', {exit: 1});
      }
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.use"></a>[module firebase-tools.use](#apidoc.module.firebase-tools.use)

#### <a name="apidoc.element.firebase-tools.use._action"></a>[function <span class="apidocSignatureSpan">firebase-tools.use.</span>_action (newActive, options)](#apidoc.element.firebase-tools.use._action)
- description and source-code
```javascript
_action = function (newActive, options) {
  // HACK: Commander.js silently swallows an option called alias >_<
  var aliasOpt;
  var i = process.argv.indexOf('--alias');
  if (i >= 0 && process.argv.length > i + 1) {
    aliasOpt = process.argv[i + 1];
  }

  if (!options.projectRoot) { // not in project directory
    return utils.reject(chalk.bold('firebase use') + ' must be run from a Firebase project directory.\n\nRun ' + chalk.bold('firebase
 init') + ' to start a project directory in the current folder.');
  }

  if (newActive) { // firebase use [alias_or_project]
    var aliasedProject = _.get(options.rc, ['projects', newActive]);
    return api.getProjects().then(function(projects) {
      if (aliasOpt) { // firebase use [project] --alias [alias]
        if (!projects[newActive]) {
          return utils.reject('Cannot create alias ' + chalk.bold(aliasOpt) + ', ' + verifyMessage(newActive));
        }
        writeAlias(options.projectRoot, options.rc, aliasOpt, newActive);
        aliasedProject = newActive;
        logger.info('Created alias', chalk.bold(aliasOpt), 'for', aliasedProject + '.');
      }

      if (aliasedProject) { // found alias
        if (!projects[aliasedProject]) { // found alias, but not in project list
          return utils.reject('Unable to use alias ' + chalk.bold(newActive) + ', ' + verifyMessage(aliasedProject));
        }

        utils.makeActiveProject(options.projectRoot, newActive);
        logger.info('Now using alias', chalk.bold(newActive), '(' + aliasedProject + ')');
      } else if (projects[newActive]) { // exact project id specified
        utils.makeActiveProject(options.projectRoot, newActive);
        logger.info('Now using project', chalk.bold(newActive));
      } else { // no alias or project recognized
        return utils.reject('Invalid project selection, ' + verifyMessage(newActive));
      }
    });
  } else if (options.unalias) { // firebase use --unalias [alias]
    if (_.has(options.rc, ['projects', options.unalias])) {
      writeAlias(options.projectRoot, options.rc, options.unalias, null);
      logger.info('Removed alias', chalk.bold(options.unalias));
      logger.info();
      listAliases(options);
    }
  } else if (options.add) { // firebase use --add
    if (options.nonInteractive) {
      return utils.reject('Cannot run ' + chalk.bold('firebase use --add') + ' in non-interactive mode. Use ' + chalk.bold('firebase
 use <project_id> --alias <alias>') + ' instead.');
    }
    return api.getProjects().then(function(projects) {
      var results = {};
      return prompt(results, [
        {
          type: 'list',
          name: 'project',
          message: 'Which project do you want to add?',
          choices: Object.keys(projects).sort()
        },
        {
          type: 'input',
          name: 'alias',
          message: 'What alias do you want to use for this project? (e.g. staging)',
          validate: function(input) {
            return input && input.length > 0;
          }
        }
      ]).then(function() {
        writeAlias(options.projectRoot, options.rc, results.alias, results.project);
        utils.makeActiveProject(options.projectRoot, results.alias);
        logger.info();
        logger.info('Created alias', chalk.bold(results.alias), 'for', results.project + '.');
        logger.info('Now using alias', chalk.bold(results.alias) + ' (' + results.project + ')');
      });
    });
  } else if (options.clear) { // firebase use --clear
    utils.makeActiveProject(options.projectRoot, null);
    options.projectAlias = null;
    options.project = null;
    logger.info('Cleared active project.');
    logger.info();
    listAliases(options);
  } else { // firebase use
    if (!process.stdout.isTTY) {
      if (options.project) {
        logger.info(options.project);
        return options.project;
      }
      return utils.reject('No active project', {exit: 1});
    }

    if (options.projectAlias) {
      logger.info('Active Project:', chalk.bold.cyan(options.projectAlias + ' (' + options.project + ')'));
    } else if (options.project) { ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.utils"></a>[module firebase-tools.utils](#apidoc.module.firebase-tools.utils)

#### <a name="apidoc.element.firebase-tools.utils.addSubdomain"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>addSubdomain (origin, subdomain)](#apidoc.element.firebase-tools.utils.addSubdomain)
- description and source-code
```javascript
addSubdomain = function (origin, subdomain) {
  return origin.replace('//', '//' + subdomain + '.');
}
```
- example usage
```shell
...
  .option('--equal-to <val>', 'restrict results to <val> (based on specified ordering)')
  .before(requireAccess)
  .action(function(path, options) {
if (!_.startsWith(path, '/')) {
  return utils.reject('Path must begin with /', {exit: 1});
}

var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';
var query = {};
if (options.shallow) { query.shallow = 'true'; }
if (options.pretty) { query.print = 'pretty'; }
if (options.export) { query.format = 'export'; }
if (options.orderByKey) { options.orderBy = '$key'; }
if (options.orderByValue) { options.orderBy = '$value'; }
_applyStringOpts(query, options, ['limitToFirst', 'limitToLast'], ['orderBy', 'startAt', 'endAt', 'equalTo']);
...
```

#### <a name="apidoc.element.firebase-tools.utils.consoleUrl"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>consoleUrl (project, path)](#apidoc.element.firebase-tools.utils.consoleUrl)
- description and source-code
```javascript
consoleUrl = function (project, path) {
  var api = require('./api');
  return api.consoleOrigin + '/project/' + project + path;
}
```
- example usage
```shell
...
    return reject(responseToError(res, body));
  }

  if (!_.endsWith(path, '/')) {
    path += '/';
  }

  var consoleUrl = utils.consoleUrl(options.project, '/database/data' + path + body.name);
  var refurl = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + body.name;

  utils.logSuccess('Data pushed successfully');
  logger.info();
  logger.info(chalk.bold('View data at:'), consoleUrl);
  return resolve(new Firebase(refurl));
}));
...
```

#### <a name="apidoc.element.firebase-tools.utils.endpoint"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>endpoint (parts)](#apidoc.element.firebase-tools.utils.endpoint)
- description and source-code
```javascript
endpoint = function (parts) {
  return '/' + _.join(parts, '/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.firebase-tools.utils.envOverride"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>envOverride (envname, value, coerce)](#apidoc.element.firebase-tools.utils.envOverride)
- description and source-code
```javascript
envOverride = function (envname, value, coerce) {
  if (process.env[envname] && process.env[envname].length) {
    if (coerce) {
      try {
        return coerce(process.env[envname], value);
      } catch (e) {
        return value;
      }
    }
    return process.env[envname];
  }
  return value;
}
```
- example usage
```shell
...
}
return path;
};

var api = {
// "In this context, the client secret is obviously not treated as a secret"
// https://developers.google.com/identity/protocols/OAuth2InstalledApp
clientId: utils.envOverride('FIREBASE_CLIENT_ID', '563584335869-fgrhgmd47bqnekij5i8b5pr03ho849e6.apps.googleusercontent.com'),
clientSecret: utils.envOverride('FIREBASE_CLIENT_SECRET', 'j9iVZfS8kkCEFUPaAeJV0sAi'),
cloudloggingOrigin: utils.envOverride('FIREBASE_CLOUDLOGGING_URL', 'https://logging.googleapis.com'),
adminOrigin: utils.envOverride('FIREBASE_ADMIN_URL', 'https://admin.firebase.com'),
apikeysOrigin: utils.envOverride('FIREBASE_APIKEYS_URL', 'https://apikeys.googleapis.com'),
appengineOrigin: utils.envOverride('FIREBASE_APPENGINE_URL', 'https://appengine.googleapis.com'),
authOrigin: utils.envOverride('FIREBASE_AUTH_URL', 'https://accounts.google.com'),
consoleOrigin: utils.envOverride('FIREBASE_CONSOLE_URL', 'https://console.firebase.google.com'),
...
```

#### <a name="apidoc.element.firebase-tools.utils.explainStdin"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>explainStdin ()](#apidoc.element.firebase-tools.utils.explainStdin)
- description and source-code
```javascript
explainStdin = function () {
  if (isWindows) {
    throw new FirebaseError('STDIN input is not available on Windows.', {exit: 1});
  }
  if (process.stdin.isTTY) {
    logger.info(chalk.bold('Note:'), 'Reading STDIN. Type JSON data and then press Ctrl-D');
  }
}
```
- example usage
```shell
...
  return utils.reject('Path must begin with /', {exit: 1});
}

var inStream = utils.stringToStream(options.data) || (infile ? fs.createReadStream(infile) : process.stdin);
var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';

if (!infile && !options.data) {
  utils.explainStdin();
}

var reqOptions = {
  url: url,
  json: true
};
...
```

#### <a name="apidoc.element.firebase-tools.utils.getInheritedOption"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>getInheritedOption (options, key)](#apidoc.element.firebase-tools.utils.getInheritedOption)
- description and source-code
```javascript
getInheritedOption = function (options, key) {
  var target = options;
  while (target) {
    if (_.has(target, key)) {
      return target[key];
    }
    target = target.parent;
  }
}
```
- example usage
```shell
...

module.exports = new Command('logout')
.description('log the CLI out of Firebase')
.action(function(options) {
  var user = configstore.get('user');
  var tokens = configstore.get('tokens');
  var currentToken = _.get(tokens, 'refresh_token');
  var token = utils.getInheritedOption(options, 'token') || currentToken;
  api.setToken(token);
  var next;
  if (token) {
    next = auth.logout(token);
  } else {
    next = RSVP.resolve();
  }
...
```

#### <a name="apidoc.element.firebase-tools.utils.logBullet"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logBullet (message, type)](#apidoc.element.firebase-tools.utils.logBullet)
- description and source-code
```javascript
logBullet = function (message, type) {
  type = type || 'info';
  logger[type](chalk.cyan.bold('i '), message);
}
```
- example usage
```shell
...
    return prompt.listLabelToValue(feat, choices);
  });
}
setup.features.unshift('project');
return init(setup, config, options);
    }).then(function() {
logger.info();
utils.logBullet('Writing configuration info to ' + chalk.bold('firebase.json') + '...');
config.writeProjectFile('firebase.json', setup.config);
utils.logBullet('Writing project information to ' + chalk.bold('.firebaserc') + '...');
config.writeProjectFile('.firebaserc', setup.rcfile);
logger.info();
utils.logSuccess('Firebase initialization complete!');

if (setup.createProject) {
...
```

#### <a name="apidoc.element.firebase-tools.utils.logSuccess"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logSuccess (message, type)](#apidoc.element.firebase-tools.utils.logSuccess)
- description and source-code
```javascript
logSuccess = function (message, type) {
  type = type || 'info';
  var chr = isWindows ? '+' : '✔';
  logger[type](chalk.green(chr + ' '), message);
}
```
- example usage
```shell
...
        if (!_.endsWith(path, '/')) {
          path += '/';
        }

        var consoleUrl = utils.consoleUrl(options.project, '/database/data' + path + body.name);
        var refurl = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + body.name;

        utils.logSuccess('Data pushed successfully');
        logger.info();
        logger.info(chalk.bold('View data at:'), consoleUrl);
        return resolve(new Firebase(refurl));
      }));
    });
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.utils.logWarning"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>logWarning (message, type)](#apidoc.element.firebase-tools.utils.logWarning)
- description and source-code
```javascript
logWarning = function (message, type) {
  type = type || 'warn';
  var chr = isWindows ? '!' : '⚠';
  logger[type](chalk.yellow.bold(chr + ' '), message);
}
```
- example usage
```shell
...
  return acquireRefs(options, [scopes.CLOUD_PLATFORM])
    .catch(function(err) {
      if (options.config.has('functions')) {
        throw err;
      }

      logger.info();
      utils.logWarning(chalk.bold('Your CLI authentication needs to be updated to take advantage of new features.'));
      utils.logWarning(chalk.bold('Please run ' + chalk.underline('firebase login --reauth')));
      logger.info();

      return acquireRefs(options, []);
    });
})
.before(checkDupHostingKeys)
...
```

#### <a name="apidoc.element.firebase-tools.utils.makeActiveProject"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>makeActiveProject (projectDir, newActive)](#apidoc.element.firebase-tools.utils.makeActiveProject)
- description and source-code
```javascript
makeActiveProject = function (projectDir, newActive) {
  var activeProjects = configstore.get('activeProjects') || {};
  if (newActive) {
    activeProjects[projectDir] = newActive;
  } else {
    _.unset(activeProjects, projectDir);
  }

  configstore.set('activeProjects', activeProjects);
}
```
- example usage
```shell
...

  return next.then(function(confirmed) {
    if (confirmed) {
      options.config.writeProjectFile('firebase.json', out);
      utils.logSuccess('Migrated ' + chalk.bold('firebase.json') + ' successfully');
      if (projectId) {
        options.config.writeProjectFile('.firebaserc', rcfile);
        utils.makeActiveProject(options.projectRoot, projectId);
        utils.logSuccess('Set default project to ' + chalk.bold(projectId));
      }
    } else {
      return utils.reject('Migration aborted by user.', {exit: 1});
    }
  });
});
...
```

#### <a name="apidoc.element.firebase-tools.utils.reject"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>reject (message, options)](#apidoc.element.firebase-tools.utils.reject)
- description and source-code
```javascript
reject = function (message, options) {
  return RSVP.reject(new FirebaseError(message, options));
}
```
- example usage
```shell
...
var checkRes = validateOptions(options);
if (!checkRes.valid) {
  return checkRes;
}
var hashOptions = checkRes;

if (!_.endsWith(dataFile, '.csv') && !_.endsWith(dataFile, '.json')) {
  return utils.reject('Data file must end with .csv or .json', {exit: 1});
}
var stats = fs.statSync(dataFile);
var fileSizeInBytes = stats.size;
logger.info('Processing ' + chalk.bold(dataFile) + ' (' + fileSizeInBytes + ' bytes)');

var inStream = fs.createReadStream(dataFile);
var batches = [];
...
```

#### <a name="apidoc.element.firebase-tools.utils.stringToStream"></a>[function <span class="apidocSignatureSpan">firebase-tools.utils.</span>stringToStream (text)](#apidoc.element.firebase-tools.utils.stringToStream)
- description and source-code
```javascript
stringToStream = function (text) {
  if (!text) {
    return undefined;
  }
  var s = new Readable();
  s.push(text);
  s.push(null);
  return s;
}
```
- example usage
```shell
...
  .option('-d, --data <data>', 'specify escaped JSON directly')
  .before(requireAccess)
  .action(function(path, infile, options) {
if (!_.startsWith(path, '/')) {
  return utils.reject('Path must begin with /', {exit: 1});
}

var inStream = utils.stringToStream(options.data) || (infile ? fs.createReadStream(infile) : process.stdin);
var url = utils.addSubdomain(api.realtimeOrigin, options.instance) + path + '.json?';

if (!infile && !options.data) {
  utils.explainStdin();
}

var reqOptions = {
...
```



# <a name="apidoc.module.firebase-tools.validator"></a>[module firebase-tools.validator](#apidoc.module.firebase-tools.validator)

#### <a name="apidoc.element.firebase-tools.validator.validator"></a>[function <span class="apidocSignatureSpan">firebase-tools.</span>validator (url)](#apidoc.element.firebase-tools.validator.validator)
- description and source-code
```javascript
validator = function (url) {
  this._validateQueue = [];

  var self = this;
  request.get(url, function(err, response, body) {
    if (!err && response.statusCode === 200) {
      self.schema = JSON.parse(body);
      self._process();
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.firebase-tools.validator.prototype"></a>[module firebase-tools.validator.prototype](#apidoc.module.firebase-tools.validator.prototype)

#### <a name="apidoc.element.firebase-tools.validator.prototype._decorateErrors"></a>[function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>_decorateErrors (errors)](#apidoc.element.firebase-tools.validator.prototype._decorateErrors)
- description and source-code
```javascript
_decorateErrors = function (errors) {
  errors.forEach(function(error) {
    error.name = error.property.replace(/^instance/, 'root');
  });
  return errors;
}
```
- example usage
```shell
...
Validator.prototype._process = function() {
  if (!this.schema) { return; }
  while (this._validateQueue.length) {
var item = this._validateQueue.shift();
var result = jsonschema.validate(item.data, this.schema);

var err = new FirebaseError('Your document has validation errors', {
  children: this._decorateErrors(result.errors),
  exit: 2
});

if (result.valid) {
  item.resolve();
} else {
  item.reject(err);
...
```

#### <a name="apidoc.element.firebase-tools.validator.prototype._process"></a>[function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>_process ()](#apidoc.element.firebase-tools.validator.prototype._process)
- description and source-code
```javascript
_process = function () {
  if (!this.schema) { return; }
  while (this._validateQueue.length) {
    var item = this._validateQueue.shift();
    var result = jsonschema.validate(item.data, this.schema);

    var err = new FirebaseError('Your document has validation errors', {
      children: this._decorateErrors(result.errors),
      exit: 2
    });

    if (result.valid) {
      item.resolve();
    } else {
      item.reject(err);
    }
  }
}
```
- example usage
```shell
...
var Validator = function(url) {
this._validateQueue = [];

var self = this;
request.get(url, function(err, response, body) {
  if (!err && response.statusCode === 200) {
    self.schema = JSON.parse(body);
    self._process();
  }
});
};

Validator.prototype.validate = function(data) {
var self = this;
return new RSVP.Promise(function(resolve, reject) {
...
```

#### <a name="apidoc.element.firebase-tools.validator.prototype.validate"></a>[function <span class="apidocSignatureSpan">firebase-tools.validator.prototype.</span>validate (data)](#apidoc.element.firebase-tools.validator.prototype.validate)
- description and source-code
```javascript
validate = function (data) {
  var self = this;
  return new RSVP.Promise(function(resolve, reject) {
    self._validateQueue.push({
      data: data,
      resolve: resolve,
      reject: reject
    });
    self._process();
  });
}
```
- example usage
```shell
...
  });
};

Validator.prototype._process = function() {
  if (!this.schema) { return; }
  while (this._validateQueue.length) {
var item = this._validateQueue.shift();
var result = jsonschema.validate(item.data, this.schema);

var err = new FirebaseError('Your document has validation errors', {
  children: this._decorateErrors(result.errors),
  exit: 2
});

if (result.valid) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
