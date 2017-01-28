# GeoNode Workshops

## How to run the presentation locally

Install dependencies with [npm](https://www.npmjs.com/) and [bower](https://bower.io/):

```bash
$ npm install
```

and

```bash
$ bower install
```

Serve it locally:

```bash
$ grunt serve
```

Open the browser at [http://localhost:9000](http://localhost:9000)

## How to publish online

Open the gruntfile configuration `Gruntfile.coffee` and change the directory for publishing the current workshop in the `dest` properties:

```coffee
copy:

            dist:
                files: [{
                    expand: true
                    src: [
                        'slides/**'
                        'bower_components/**'
                        'js/**'
                        'css/*.css'
                        'resources/**'
                        'css/img/**'
                        'css/fonts/**'
                    ]
                    dest: 'dist/foss4git2017'
                },{
                    expand: true
                    src: ['index.html']
                    dest: 'dist/foss4git2017'
                    filter: 'isFile'
                }]
```

Run then the build with the command:

```bash
$ grunt dist
```

Deploy on specific folder of github pages:

```bash
$ grunt deploy
```
