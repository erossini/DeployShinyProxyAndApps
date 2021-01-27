# Deploy ShinyApps with Azure and Docker
In this new post, I explain how to deploy in an [Azure](https://www.puresourcecode.com/category/tools/azure-tools/) WebApp a [ShinyApps](https://www.puresourcecode.com/tag/shiny-apps) created with [RStudio](https://www.puresourcecode.com/programming-languages/getting-started-with-r) using Azure [DevOps](https://www.puresourcecode.com/?s=devops) as repository and [Docker](https://www.puresourcecode.com/?s=docker) as container. I wrote another post about [dockerize Shiny Apps with command line](https://www.puresourcecode.com/programming-languages/r/deploying-dockerized-r-shiny-apps-on-microsoft-azure/).

For data scientists, ShinyApps offer the possibility to quickly create cute web applications also for prototyping. ShinyApps don't have security integrated. So, we have to find another way to add a security layer to our Shiny applications.

So, we will use [ShinyProxy](https://shinyproxy.io/) to add a security layer. This makes the deployment a bit harder but we will take advantage of that. The pipeline in Azure DevOps for ShinyProxy will be similar to the pipeline for a ShinyApp. I will show in this post how to create a Docker container for ShinyProxy and ShinyProxy.

This repository is related to the post "Deploy ShinyApps with Azure and Docker" on my blog [PureSourceCode](https://www.puresourcecode.com).
