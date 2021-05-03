# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

Let's start with the main differences between Azure VM and Azure App Services solutions for my app:

|| Azure Virtual Machines     | Azure App Services |
| ----------- | ----------- | ----------- |
| Service | Iaas | PaaS |
| Control | Control over OS and the Infrastructure  | Control over the application code only |
| Languages | Any programming language can be used as long as the machine is configured accordingly  | A fixed number of languages supported   |
| Pricing |  Costs a bit higher at the basic tier | Cheaper, but has less options |
| Scalability |  Scale Sets and Load Balancers | Vertical and Horizontal Scaling Options |
| Availability |  Azure guarantees high availability (>99.9%)with at least two or more instances deployed | %99.95 availability guarantee for basic tier and upwards |

Therefore, for this application, I chose Azure App Services because;

-With App Services, I only need to work on my application code and languages the app uses are supported by the App Services.

-The application does not have very high performance and optimization standards as it is a blogging site.

-With App Services, I could make simple improvements upon my site, such as adding subtitles, multiple image uploads etc., and deploy it quickly.

-App Services' scaling options would be enough for me in case my app starts to see more traffic.

-I'd want my app to be as cheap as possible as it is a simple blog to record my ideas.

### Assess app changes that would change your decision.

-Overall, if my app's memory or cpu requirements increase substantially, I'd consider converting to VM service. For example, I wanted to include videos, or interactive features, limitations of App services might prevent my app from running smoothly. 

-In case this app was already present and contained extensive data, and I wanted to migrate to cloud. Virtual machines would be a much better choice as I would be able to replicate my server on the cloud.

-If my blog took off and has receiving increasingly more traffic, I could consider converting to VM to not be limited by App Services' compute resources.

-Virtual machines present much better control over the app's security. In case I wanted my app to be more secure about who can access what information, I'd want more control with virtual machines.
