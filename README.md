Minimal Nginx Heroku Buildpack
==============================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for
nginx.  A dyno created with this buildpack will assume anything deployed is an
nginx app.  Any of the files in the compile step can be overriden by the deployed
app so that you can define a custom nginx conf.
