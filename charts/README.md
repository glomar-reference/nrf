# Smoketest

helm upgrade \
  --create-namespace \
  --install \
  --wait \
  --namespace=open5gs \
  "nrf" \
  "$(git rev-parse --show-toplevel)/charts/nrf"