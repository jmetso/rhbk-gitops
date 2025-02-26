# Red Hat build of Keycloak GitOps repository

Multi cluster structure to deploy [Red Hat Build of Keycloak](https://access.redhat.com/products/red-hat-build-of-keycloak/). 

Currently only one cluster configured.

Folder structure:

```
 |____bootstrap
 | |____argocd
 |   |____rhds
 |     |____apps         - argocd apps for rhds cluster overlays
 |     |____app-of-apps  - app-of-apps for rhds cluster argocd apps
 |
 |____clusters
 | |____overlays
 |   |____rhds
 |     |____tst          - rhds cluster overlay for tst env config
 |     |____prd          - rhds cluster overlay for prd env config
 |
 |____components
 | |____apps
 |   |____keycloak
 |   | |____base         - keycloak base config
 |   |____keycloak-database
 |   | |____base         - keycloak db base config
 |   |____keycloak-operator
 |     |____base         - keycloak operator base config
 |
 |____environments
   |____overlays
     |____tst            - test env overlay for base config
     |____prd            - prod env overlay for base config

```


Inspired by [https://github.com/gnunn-gitops/standards](https://github.com/gnunn-gitops/standards)
