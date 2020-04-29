# Travis Presets

This is a repository for reusable configs for [Travis CI](https://travis-ci.com/),
which can be [imported into your Travis file](https://docs.travis-ci.com/user/build-config-imports/).

## Node.JS Presets

This presets makes sure that:
* all important Node.JS versions are tested
* npm is cached
* `build`, `lint`, `test` scripts are executed
* `coveralls` scripts is executed after success

```yml
import: rubensworks/travis-presets:node.yml@master
# ... other stuff
```

If the script execution is not desired, then `rubensworks/travis-presets:node-base.yml@master` can be imported instead,
which just defines Node.JS versions and caches npm.

## License
This software is written by [Ruben Taelman](http://rubensworks.net/).

This code is released under the [MIT license](http://opensource.org/licenses/MIT).

