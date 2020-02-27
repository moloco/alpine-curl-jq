# E2E script runtime

This docker image is FROM [appropriate/curl][curl], and just adds
[`jq`][jq] and bash on top.

This docker image is to facilitate the curl-based e2e script development. 

# To use it from your cloud build script

You can build this image for your project in the following way:

```
gcloud builds submit --tag=gcr.io/$PROJECT_ID/alpine-curl-jq .
```

[curl]: https://hub.docker.com/r/appropriate/curl/
[jq]: https://stedolan.github.io/jq/
