# RequireJS + Hogan.js + The Intern Example

Building a random image gallery using AMD modules:

![amd-gallery](http://i.imgur.com/H7NSmJG.png)

## Prerequisites

* Node.js (http://nodejs.org/)
* Grunt CLI (http://gruntjs.com/)

Run `npm install` the first time you download the app in order to build the binaries for any node modules.

Grunt CLI can be installed globally for convenience with `npm install -g grunt-cli`, otherwise the binary can be found here: `./node_modules/grunt-cli/bin/grunt`.

## Development Tasks

| Command           | Description                      |
|-------------------|----------------------------------|
| `npm install`     | Fetch dependencies               |
| `grunt`           | Start development server         |
| `grunt build`     | Build all the things!            |
| `grunt js`        | Run all JS-related tasks         |
| `grunt hogan`     | Precompile .mustache files       |
| `grunt requirejs` | Concatenate and minify .js files |
| `grunt jshint`    | Lint .js files                   |
| `grunt css`       | Run all CSS-related tasks        |
| `grunt less`      | Compile .less files              |
| `grunt cssmin`    | Minify .css files                |
| `grunt csslint`   | Lint .css files                  |
| `grunt test`      | Run tests and generate coverage report. [Browser version here.](http://localhost:6789/node_modules/intern/client.html?config=tests/intern) |

## Release Versions

Follow these steps to have your feature branch merged:

1. `git fetch`
2. `git checkout develop && git reset --hard origin/develop`
3. `npm version [<newversion> | major | minor | patch]`
4. `git checkout master && git reset --hard origin/master`
5. `git merge develop`
6. `git push --tags && git push && git checkout develop && git push`

## Semantic Versioning

Given a version number `MAJOR.MINOR.PATCH`, increment the:

1. `MAJOR` version when you make incompatible API changes,
2. `MINOR` version when you add functionality in a backwards-compatible manner, and
3. `PATCH` version when you make backwards-compatible bug fixes.

Additional labels for pre-release and build metadata [are available](https://docs.npmjs.com/cli/version) as extensions to the `MAJOR.MINOR.PATCH` format.

See the [Semantic Versioning](http://semver.org/) specification for more information.
