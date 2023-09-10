# A nice colors Helm Chart to demo routes with multiple backends

```YAML
deployment:
# Each object in the array will create it's own deployment and service 
# and will add a new backend in the route
# The Route support up to 3 backend services
    # Name of the Application
  - name: blue 
    # Number of replicas
    replicas: 1
    # Color of the bubbles
    color: blue
    # The weight that will be used in the route
    weight: 5
  - name: green
    replicas: 1
    color: green
    weight: 5
  - name: purple
    replicas: 1
    color: purple
    weight: 5
```