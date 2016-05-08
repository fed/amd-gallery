# RequireJS + Hogan.js Example

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

To version and tag a release, move to `master` and run the [appropriate command](https://docs.npmjs.com/cli/version):

```
npm version major  # bump major version, eg. 1.0.2 -> 2.0.0
npm version minor  # bump minor version, eg. 0.1.3 -> 0.2.0
npm version patch  # bump patch version, eg. 0.0.1 -> 0.0.2
```

Make sure to push tags:

```
git push --tags origin master
```

## Semantic Versioning

Given a version number `MAJOR.MINOR.PATCH`, increment the:

1. `MAJOR` version when you make incompatible API changes,
2. `MINOR` version when you add functionality in a backwards-compatible manner, and
3. `PATCH` version when you make backwards-compatible bug fixes.

Additional labels for pre-release and build metadata are available as extensions to the `MAJOR.MINOR.PATCH` format.

See the [Semantic Versioning](http://semver.org/) specification for more information.
