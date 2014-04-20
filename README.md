Navigator
=========

[![Build Status](https://travis-ci.org/Team-Sass/navigator.svg?branch=master)](https://travis-ci.org/Team-Sass/navigator)

A Ruby testing framework for Sass with Compass.

## Requirements and Usage

Navigator works through Ruby, so you need to be running Ruby 1.8.7 or greater, and you need [Bundler](http://bundler.io/) installed. In order to use Navigator, drop these files into your project, update the Gemfile for the versions you'd like to test against, then run `bundle install`.

Once you have everything installed, run `bundle exec rake` to run the tests. This will compile all of the files in your `tests/tests` files into CSS files and compare those files to the files in `tests/controls`. If any of your output file from your tests don't line up with your controls, you'll get a `.diff` file generated of the differences and you'll get a failed assertion. If your Sass won't compile, you'll get a failed assertion.

If you're working off of a known set of good output and you'd like to generate your controls quickly, you can run `bundle exec rake compile`.

See the README files in `tests/tests` and `tests/controls` for more on what should go into each of them.

## Travis

If you would like to employ [Travis](https://travis-ci.org/) testing for your projects, enable Travis testing on your [Travis profile page](https://travis-ci.org/profile/). This will set Travis up to run the tests against Ruby 1.8.7 and 2.0.0. If you'd like to add the pretty **build passing** image to your Markdown READMEs, here's the code to use once you've got Travis set up!

`[![Build Status](https://travis-ci.org/{user}/{repo}.svg?branch={branch})](https://travis-ci.org/{user}/{repo})`

## License

(c) Sam Richard, Ian Carrico

Licensed under MIT license.
