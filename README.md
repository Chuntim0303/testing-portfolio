# Build and deploy

Command to build the application. PLease remeber to change the project name and application name
```
gcloud builds submit --tag gcr.io/portfolio-streamlit/portfolio-streamlit-main  --project=portfolio-streamlit
```

Command to deploy the application
```
gcloud run deploy --image gcr.io/portfolio-streamlit/portfolio-streamlit-main --platform managed  --project=portfolio-streamlit --allow-unauthenticated
```