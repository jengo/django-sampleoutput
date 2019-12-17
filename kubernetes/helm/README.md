# In order to deploy this, you will need to create a Kubernetes secret.
# You never want to store credentials in plain text within your repo
# It's recommended that you use a vault store anyway
kubectl -n jolene create secret generic mysecret --from-literal=SECRET_KEY=changeme
