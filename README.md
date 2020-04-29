# Travis Presets

This is a repository for reusable configs for [Travis CI](https://travis-ci.com/),
which can be [imported into your Travis file](https://docs.travis-ci.com/user/build-config-imports/).

## Node.JS Presets

### [`node-base.yml`](https://github.com/rubensworks/travis-presets/blob/master/node-base.yml)

This preset defines a testing matrix with all major LTS Node versions, and enables npm caching.

**`travis.yml`:**

```yml
import: rubensworks/travis-presets:node-base.yml@master
# ... other stuff
```

### [`node.yml`](https://github.com/rubensworks/travis-presets/blob/master/node.yml)

This preset extends from `node-base.yml`,
and additionally executes `build`, `lint`, `test` scripts,
and runs the `coveralls` script after success.

**`travis.yml`:**

```yml
import: rubensworks/travis-presets:node.yml@master
# ... other stuff
```

## License
This software is written by [Ruben Taelman](http://rubensworks.net/).

This code is released under the [MIT license](http://opensource.org/licenses/MIT).

