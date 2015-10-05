Minimal Nginx Heroku Buildpack
==============================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for
nginx.  A dyno created with this buildpack will assume anything deployed is an
nginx app.  Any of the files in the compile step can be overriden by the deployed
app so that you can define a custom nginx conf.

This is just for serving static files or proxying, check out the other nginx
build packs for proxying via a local socket to a backend started with nginx.

## nginx build

The nginx binary is latest stable verion 1.8.0 built on the heroku cedar-14 stack
using [yappbox/yapp-native-build](https://github.com/yappbox/yapp-native-build).

To update nginx just copy the binary built on heroku following the README
[yappbox/yapp-native-build](https://github.com/yappbox/yapp-native-build)
to `bin/nginx`
