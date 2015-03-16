# nodejs-bower-grunt

This Dockerfile extends the `dockerfile/nodejs-bower-grunt` and adds sass, compass, and libraries that are required for some builds. It is intended to be used for building the assets in your project.

The workdir is set to `/app`.

# Example uses

```
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-grunt npm install
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-grunt bower install
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-grunt grunt build
```

