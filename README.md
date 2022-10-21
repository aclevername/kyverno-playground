# kyverno-playground

## Installing
Create your kind cluster and then install kyverno:
```bash
./install.sh
```

## Example label enforcing policy

```bash
k apply -f resources/example-label-enforcing-policy.yaml

k apply -f resources/deployment-without-label.yaml
# see error

k apply -f resources/deployment-with-label.yaml
# see success
```
