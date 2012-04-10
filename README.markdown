## Setup

``` bash
rake install
rake preview
```


## Deploying to Heroku

http://jasongarber.com/blog/2012/01/10/deploying-octopress-to-heroku-with-a-custom-buildpack/

``` bash
heroku create --stack cedar --buildpack git://github.com/jgarber/heroku-buildpack-ruby-octopress.git
git push heroku master

$ git push heroku master
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 287 bytes, done.
Total 2 (delta 1), reused 0 (delta 0)

-----> Heroku receiving push
-----> Fetching custom buildpack... done
-----> Octopress app detected
-----> Installing dependencies using Bundler version 1.1.rc.3
       Running: bundle install --without development:test --path vendor/bundle --binstubs bin/ --deployment
       Using rake (0.9.2.2)
       Using RedCloth (4.2.8)
       Using posix-spawn (0.3.6)
       Using albino (1.3.3)
       Using blankslate (2.1.2.4)
       Using chunky_png (1.2.1)
       Using fast-stemmer (1.0.0)
       Using classifier (1.3.3)
       Using fssm (0.2.7)
       Using sass (3.1.5)
       Using compass (0.11.5)
       Using directory_watcher (1.4.0)
       Using ffi (1.0.9)
       Using haml (3.1.2)
       Using kramdown (0.13.3)
       Using liquid (2.2.2)
       Using syntax (1.0.0)
       Using maruku (0.6.0)
       Using jekyll (0.11.0)
       Using rubypython (0.5.1)
       Using pygments.rb (0.1.3)
       Using rack (1.3.2)
       Using rdiscount (1.6.8)
       Using rubypants (0.2.0)
       Using tilt (1.3.2)
       Using sinatra (1.2.6)
       Using stringex (1.3.0)
       Using bundler (1.1.rc.3)
       Your bundle is complete! It was installed into ./vendor/bundle
       Cleaning up the bundler cache.
-----> Building Octopress site
       ## Generating Site with Jekyll
       directory source/stylesheets/
          create source/stylesheets/screen.css
       Configuration from /tmp/build_3o42m2napfrdu/_config.yml
       Building site: source -> public
       Successfully generated site: source -> public
-----> Discovering process types
       Procfile declares types     -> (none)
       Default types for Octopress -> console, rake, web
-----> Compiled slug size is 17.2MB
-----> Launching... done, v5
       http://smooth-mist-1976.herokuapp.com deployed to Heroku

To git@heroku.com:smooth-mist-1976.git
   dc8f977..3fc80c2  master -> master
```


## Twitter Bootstrap Theme

https://github.com/bkutil/bootstrap-theme

## Customize

``` bash
$ vim sass/custom/_styles.scss
```

## License
(The MIT License)

Copyright © 2009-2011 Brandon Mathis

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


#### If you want to be awesome.
- Proudly display the 'Powered by Octopress' credit in the footer.
- Add your site to the Wiki so we can watch the community grow.

