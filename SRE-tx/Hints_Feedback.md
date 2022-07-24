## Challenge Hints and Feedback:
I personally added these tasks to make the project awesome and not just a normal assessment:

- Documentation should be structured and lean. 
- An API could be built instead of a webpage (e.g. a REST API)
- Programming, IaC and Ci/CD skills demonstrated should be made with production in view (noy jus)
- App should work for any page (`endpoint that receives a path from Wikipedia` which could be a querystring parameter, i.e. `localhost?page=Portugal`).
- API versioning implemented
- Data normalization implemented
- Health check endpoint
- Containers should be read-only (if needed, a volume should be used) with non-root user enforcement
- Logging could use different log levels and should go to stdout or stderr
- requirements.txt could have fixed version
- Prometheus metrics could be added with the use of, e.g., Prometheus Flask Exporter package

# Task 2
- AWS and EKS roles integration!
- Using public TF modules can help but can also bring unnecessary complexity (too many layered modules)
- Using null resource is a practice Hashicorp recommends as a last resource and should be avoided (Helm chart could be used on a pipeline, for instance)
- Automae the installation of Prometheus wth Helm
- Deploy artifact to private repo

# Task 3
- Trigger branch to main (PR's should be opened targeting main, not develop)
- Sleeps should be avoid (use wait=true when available)

## Technical Interview
### Technical questions summary
- What would you have implemented to make your project better?
- How would uou have implemented each of them (explain the approach, tool and why that implementation)
- How would you deploy the application and infrastructure for production and what support techniques would you implement?
- How do you manage deployed applications and what case scenarios would you implement for proactive responses?

### Team culture fit:
Tell me about your previous work experience with the following:
- the type of teams you've worked with in the past 
- the types of projects you've built, 
- the SDLC methodology, you're experienced with
- the approach you've had towards solving problems as a team
- etc.