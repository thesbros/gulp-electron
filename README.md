# gulp-run-electron
Gulp plugin for starting Electron.

## Usage
```js
var runElectron = require("gulp-run-electron");
gulp.src("app")
	.pipe(runElectron(["--cli-argument", "--another"], {cwd: "path"}));
```

### runElectron(args: array, opts: object)
Runs the electron executable on the src folder with the specified arguments, and
passes the opts object to child_process.spawn.

Both arguments are optional. If you only want to use the opts object, pass an
empty array for args.
