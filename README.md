# Building-a-static-website-with-Microsoft-Azure
A static website consists of pre-built files (HTML, CSS, JS) served directly to users without server-side processing, resulting in high speed, enhanced security, and low-cost hosting. Ideal for portfolios or landing pages, they deliver identical, fixed content to all visitors.

Static website hosting on Azure provides scalable, cost-effective solutions for serving HTML, CSS, JavaScript, and other static content. Let me walk you through the key aspects comprehensively.
Azure Storage Static Websites is the most popular choice for pure static content. You enable this feature on a standard Azure Storage Account (GPv2), which creates a special $web container. This approach is remarkably cost-effective, charging only for storage and bandwidth, typically pennies per month for small to medium sites. The storage account automatically serves your index.html as the default document and handles 404 errors with a custom error page.
When setting up static website hosting on Azure Storage, you create a storage account in your preferred region, then enable the static website feature through the Azure Portal, CLI, or ARM templates. This generates a primary endpoint URL like https://mystorageaccount.z13.web.core.windows.net. You upload your files to the $web container using tools like Azure Storage Explorer, AzCopy, or directly through CI/CD pipelines.
Azure App Service can also host static sites but is generally overkill unless you need server-side capabilities. 
Limitations
Static hosting doesn't support server-side rendering, dynamic content generation, or complex URL rewriting. Single-page applications work well but require client-side routing. Security headers must be configured at the CDN level.
When to Choose What
Use Azure Storage for simple static sites where cost is paramount. Choose Azure Static Web Apps for modern web applications needing CI/CD, authentication, or serverless APIs. Both scale effortlessly from hobby projects to enterprise applications serving global audiences.
Here is the link to my static website below:

https://enyex100.z1.web.core.windows.net/

Thanks for reading. 

Skills: Cloud Computing • Technical Assistance • Cloud Consulting • Account Management • Microsoft Azure • Azure Data Lake • Troubleshooting Skills: Cloud Computing • Technical Assistance • Cloud Consulting • Account Management • Microsoft Azure • Azure Data Lake • Troubleshooting

o	
 
My Azure Static Website


