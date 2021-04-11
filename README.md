# PAM Tools Workshop

A set of guided labs to get you up started on how to:
- Create business projects using the maven archetype
- Author decisions using VSCode Extension
- Test decisions using Scenario Simulation Tool
- Deploy the project in KIE Server
- Try out the same project in Business Central

### Running locally

Have docker or podman running locally:

```````
docker run -it --rm -p 8080:8080 -v $(pwd):/app-data -e CONTENT_URL_PREFIX="file:///app-data" -e WORKSHOPS_URLS="file:///app-data/_tooling_workshop.yml" -e LOG_TO_STDOUT=true quay.io/osevg/workshopper
```````

### Running on ocp

Login on ocp and:

````
oc create -f support/ocp-provisioning.yml
````
