# gatekeeper-demo


## How to install on minikube?

`kubectl apply -f gatekeeper.yaml`

## Apply template

Template defines that given resource should have labels:

`k apply -f required_labels_template.yaml`

## Apply that config maps have to have team label:

`k apply -f team_config_map_constraint.yaml`

## Try to apply config maps

`k apply -f bad-config-map.yaml` - should be unsuccessful

`k apply -f good-config-map.yaml`