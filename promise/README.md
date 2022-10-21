This example uses a KRM function to interpolate into the `promise.yaml` the contents of a helm release.

To run within this directory:
```bash
kustomize build --enable-alpha-plugins --enable-exec .
```

To apply the output to your cluster:
```
kustomize build --enable-alpha-plugins --enable-exec . > output.yaml | k apply -f -
```
