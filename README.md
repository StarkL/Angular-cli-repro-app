the step :

```
	ng version
	_                      _                 ____ _     ___
	/ \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
	/ △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
	/ ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
	/_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
	|___/

	Angular CLI: 1.7.1
	Node: 8.9.0
	OS: win32 x64
	Angular:
	...

	starkL@BBen MINGW64 /d/document/IT/pf-Nokia/2-demo/angular-cli
	$ ng new repo-app -style=scss --skip-install
	  create repo-app/e2e/app.e2e-spec.ts (290 bytes)
	  create repo-app/e2e/app.po.ts (208 bytes)
	  create repo-app/e2e/tsconfig.e2e.json (235 bytes)
	  create repo-app/karma.conf.js (923 bytes)
	  create repo-app/package.json (1293 bytes)
	  create repo-app/protractor.conf.js (722 bytes)
	  create repo-app/README.md (1023 bytes)
	  create repo-app/tsconfig.json (363 bytes)
	  create repo-app/tslint.json (3012 bytes)
	  create repo-app/.angular-cli.json (1245 bytes)
	  create repo-app/.editorconfig (245 bytes)
	  create repo-app/.gitignore (544 bytes)
	  create repo-app/src/assets/.gitkeep (0 bytes)
	  create repo-app/src/environments/environment.prod.ts (51 bytes)
	  create repo-app/src/environments/environment.ts (387 bytes)
	  create repo-app/src/favicon.ico (5430 bytes)
	  create repo-app/src/index.html (294 bytes)
	  create repo-app/src/main.ts (370 bytes)
	  create repo-app/src/polyfills.ts (3114 bytes)
	  create repo-app/src/styles.scss (80 bytes)
	  create repo-app/src/test.ts (642 bytes)
	  create repo-app/src/tsconfig.app.json (211 bytes)
	  create repo-app/src/tsconfig.spec.json (283 bytes)
	  create repo-app/src/typings.d.ts (104 bytes)
	  create repo-app/src/app/app.module.ts (316 bytes)
	  create repo-app/src/app/app.component.html (1141 bytes)
	  create repo-app/src/app/app.component.spec.ts (986 bytes)
	  create repo-app/src/app/app.component.ts (208 bytes)
	  create repo-app/src/app/app.component.scss (0 bytes)
	Project 'repo-app' successfully created.

	starkL@BBen MINGW64 /d/document/IT/pf-Nokia/2-demo/angular-cli
	$ cd repro-app/

	starkL@BBen MINGW64 /d/document/IT/pf-Nokia/2-demo/angular-cli/repro-app (master)
	$ cnpm i
	platform unsupported @angular/cli@1.7.1 › @angular-devkit/core@0.3.2 › chokidar@1.7.0 › fsevents@^1.0.0 Package require os(darwin) not compatible with your platform(win32)
	[fsevents@^1.0.0] optional install error: Package require os(darwin) not compatible with your platform(win32)
	[npminstall:get] retry GET http://registry.npm.taobao.org/webpack-dev-server/download/webpack-dev-server-2.11.2.tgz after 100ms, retry left 4, error: ResponseError: socket hang up (req "error"), GET https://cdn.npm.taobao.org/webpack-dev-server/-/webpack-dev-server-2.11.2.tgz -1 (connected: true, keepalive socket: true, agent status: {"createSocketCount":3,"createSocketErrorCount":0,"closeSocketCount":3,"errorSocketCount":0,"timeoutSocketCount":3,"requestCount":10,"freeSockets":{},"sockets":{},"requests":{}})
	headers: {}
	√ Installed 30 packages
	√ Linked 882 latest versions
	Cached binary found at C:\Users\starkL\.npminstall_tarball\node-sass\4.7.2\win32-x64-57_binding.node
	Binary found at D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_node-sass@4.7.2@node-sass\vendor\win32-x64-57\binding.node
	Testing binary
	Binary is fine
	√ Run 3 scripts
	deprecate karma@2.0.0 › log4js@2.5.3 › nodemailer@^2.5.0 All versions below 4.0.1 of Nodemailer are deprecated. See https://nodemailer.com/status/
	deprecate karma@2.0.0 › log4js@2.5.3 › loggly@1.1.1 › request@2.75.0 › node-uuid@~1.4.7 Use uuid module instead
	Recently updated (since 2018-02-21): 50 packages (detail see file D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\.recently_updates.txt)
	  Today:
	    → @angular/cli@1.7.1 › cache-loader@^1.2.0(1.2.2) (05:18:37)
	    → @angular/cli@1.7.1 › cache-loader@1.2.2 › webpack@3.11.0 › yargs@8.0.2 › read-pkg-up@2.0.0 › read-pkg@2.0.0 › normalize-package-data@2.4.0 › validate-npm-package-license@^3.0.1(3.0.3) (02:18:49)
	    → @angular/cli@1.7.1 › cache-loader@1.2.2 › webpack@3.11.0 › yargs@8.0.2 › read-pkg-up@2.0.0 › read-pkg@2.0.0 › normalize-package-data@2.4.0 › validate-npm-package-license@3.0.3 › spdx-correct@^3.0.0(3.0.0) (02:16:36)
	    → karma@2.0.0 › log4js@2.5.3 › redis@2.8.0 › redis-commands@^1.2.0(1.3.5) (11:42:09)
	√ All packages installed (1092 packages installed from npm registry, used 1m, speed 34.26kB/s, json 912(1.88MB), tarball 359.6kB)

	starkL@BBen MINGW64 /d/document/IT/pf-Nokia/2-demo/angular-cli/repro-app (master)
	$ ng build -prod
	Unhandled rejection Error: ENOENT: no such file or directory, open 'D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_@angular_core@5.2.6@@angular\package.json'
	    at Object.fs.openSync (fs.js:646:18)
	    at Object.fs.readFileSync (fs.js:551:33)
	    at LicenseExtractor.readPackageJson (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseExtractor.js:124:23)
	    at LicenseExtractor.parsePackage (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseExtractor.js:21:32)
	    at ModuleProcessor.processPackage (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\ModuleProcessor.js:24:46)
	    at ModuleProcessor.processFile (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\ModuleProcessor.js:21:21)
	    at fileCallback (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseWebpackPlugin.js:80:61)
	    at moduleCallback (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseWebpackPlugin.js:87:21)
	    at Set.forEach (<anonymous>)
	    at Chunk.forEachModule (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_webpack@3.11.0@webpack\lib\Chunk.js:159:17)
	    at D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseWebpackPlugin.js:96:27
	    at Array.forEach (<anonymous>)
	    at Compiler.<anonymous> (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_license-webpack-plugin@1.1.2@license-webpack-plugin\dist\LicenseWebpackPlugin.js:65:32)
	    at next (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_tapable@0.2.8@tapable\lib\Tapable.js:204:14)
	    at D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_html-webpack-plugin@2.30.1@html-webpack-plugin\index.js:204:9
	    at PassThroughHandlerContext.finallyHandler (D:\document\IT\pf-Nokia\2-demo\angular-cli\repro-app\node_modules\_bluebird@3.5.1@bluebird\js\release\finally.js:56:23)

	starkL@BBen MINGW64 /d/document/IT/pf-Nokia/2-demo/angular-cli/repro-app (master)
	$
```
