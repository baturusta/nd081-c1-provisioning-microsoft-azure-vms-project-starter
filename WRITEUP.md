# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

Let's start with the main differences between Azure VM and Azure App Services solutions for my app:

| Azure Virtual Machines     | Azure App Services |
| ----------- | ----------- |
| Iaas     | PaaS     |
| Control over OS and the Infrastructure  | Control over the application code only      |
| Any programming language can be used as long as the machine is configured accordingly  | A fixed number of languages supported   |
|   |    |


Therefore, for this application, I chose Azure App Services because;

-With App Services, I only need to work on my application code and languages the app uses are supported by the App Services.
-The application does not have very high performance and optimization standards as it is a blogging site.
-With App Services, I could make simple improvements upon my site, such as adding subtitles, multiple image uploads etc., and deploy it quickly.
-And while I'd want my app to have high availability, I don't care about scaling as much.
-I'd want my app to be as cheap as possible as it is a simple blog to record my ideas.

### Assess app changes that would change your decision.

-Overall, if my app's memory or cpu requirements increase substantially, I'd consider converting to VM service. For example, I wanted to include videos, or interactive features, limitations of App services might prevent my app from running smoothly. 
-In case this app was already present and contained extensive data, and I wanted to migrate to cloud. Virtual machines would be a much better choice as I would be able to replicate my server on the cloud.
-If my blog took off and has receiving increasingly more traffic, I could consider converting to VM to not be limited by App Services' compute resources.

