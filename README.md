# googleCloudAPIGatewayFirst

# Pre-requisites
1. Cloud function

# Intial checkup
Check if you have gcloud setup in your local machine or not
```
https://github.com/madi82/GoogleCloudPlatform_Python/wiki/Google-Cloud-SDK-setup
```

Run below command and command will update component automatically 
```
gcloud components update
```
Set the default project. Replace PROJECT_ID with your Google Cloud Platform (GCP) project ID
```
gcloud config set project PROJECT_ID
```
# Enable required services 

API Gateway requires that you enable the following Google services:

1. apigateway.googleapis.com (_API Gateway API_)
2. servicemanagement.googleapis.com	(_Service Management API_)
3. servicecontrol.googleapis.com (_Service Control API_)

To confirm that the required services are enabled:
```
gcloud services list
```
If you do not see the required services listed, enable them:
```
gcloud services enable apigateway.googleapis.com
gcloud services enable servicemanagement.googleapis.com
gcloud services enable servicecontrol.googleapis.com
```
# Configuring a service account [_pending_]
There are 2 types 
1. Using separate svc account
2. Using default svc account
```
https://cloud.google.com/api-gateway/docs/configure-dev-env#configuring_a_service_account
```

