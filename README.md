# Skaffold issue #5341

`--default-repo` is not honoured with the `deploy` command. 

See https://github.com/GoogleContainerTools/skaffold/issues/5341 for more info



Checkout this repo and then run:

```
skaffold deploy --default-repo eu.gcr.io/my-registry --images my-image:1.0.0
```

## Expected behaviour

It should deploy the image `eu.gcr.io/my-registry/my-image:1.0.0`

## Actual behaviour

It deploys `my-image:1.0.0`.

