### Warning
Due to the architecture of Java function app, please ensure the `pom.xml -> project -> properties -> functionAppName`
field matches your Azure Functions name on the cloud when using deployment center GitHub action.

### Intention

1. Check if functions project can be deployed successfully
2. Check if third party library `junit` can be resolved correctly

### Usage

1. Deploy the function app using deployment center
2. Make a GET http request to `/api/HttpTrigger`
3. Should get a 200 status code with `Hello Functions World!` body
