
# Body-Cam-Meta


**TODO**: Body-Cam-Meta is the only &hellip; that &hellip;


## Install

```bash
# clone the repo
git clone git@github.com:yourname/body-cam-meta.git

# change dir to the cloned repo
cd body-cam-meta

# install dev dependencies
npm install -d

# install gulp cli
npm install -g gulp

# build bower/less files
gulp postinstall
```


## Configuration

Configuration (e.g. database and logging setting per environment) is stored in `boot/config.js`.


## Documentation

[The wiki](https://github.com/niftylettuce/eskimo/wiki) is the main source for additional documentation.

## Usage

### Development

Default:

```bash
node app
```

Debugging:

```bash
DEBUG=* node app
```

#### Gulp tasks:

```bash
# Run 'bower', 'less', and 'jshint' tasks
gulp postinstall

# Runs 'build'
gulp

# Run jshint to check syntax of JavaScript files
gulp jshint

# Runs 'clean', 'bower', 'less', 'copy', 'imagemin', 'usemin-css', 'usemin-js', and 'usemin-jade'
gulp build

# Runs 'watch-noapp', running the app with nodemon and livereload
gulp watch

# Runs 'watch-noreload', and starts a livereload server to automatically refresh your browser when changes are done
gulp watch-noapp

# Watches changes to public assets (images, fonts, less/css, js, and jade files) and runs appropriate tasks ('imagemin', 'less'/'usemin-css', 'usemin-js', 'usemin-jade') to parse them
gulp watch-noreload

# Run less to create CSS files
gulp less

# Optimizes and copies images to 'assets/dist/img'
gulp imagemin

# Adds versions to JS files, copying them later to 'assets/dist/js'
gulp usemin-js

# Adds versions to CSS files, optimizes and parses images and CSS files as well, copying them later to 'assets/dist'
gulp usemin-css

# Adds versions to assets in JADE files, optimizes and parses assets, copying them later to 'assets/dist'
gulp usemin-jade

# Cleans 'assets/dist' and 'bower_components' directories
gulp clean

# Copies some static files (favicon, robots.txt, etc) to 'assets/dist'
gulp copy
```

### Production

> Production environment requires that you have built out the "assets/dist" folder.

Build project with [gulp.js](http://gulpjs.com/):

```bash
gulp build
```

> Now you can proceed to running in production mode with optional `recluster` support.

Default:

```bash
sudo NODE_ENV=production node app
```

[Recluster](https://github.com/doxout/recluster):

```bash
sudo NODE_ENV=production node cluster
# kill -s SIGUSR2 %d
```


## Tests

```bash
npm test
```


## Contributors

See "package.json" for a list of contributors.  Learn how to add contributors using [npm's docs](https://www.npmjs.org/doc/files/package.json.html#people-fields-author-contributors).


## License

**TODO**: [Choose a license](http://choosealicense.com/) and insert it here.
