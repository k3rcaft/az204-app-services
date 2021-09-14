# az204-app-services

## What is Azure App Service

Azure App Service (PaaS) is a fully managed web application hosting platform. Where :

- You just focus on designing and building your app.
- Azure takes care of the infrastructure to run and scale your applications.

## App Service plans

It is a set of virtual server resources that run App Service apps.
App Service plans are the unit of billing for App Service.
A single App Service plan can host multiple App Service web apps.

Each App Service plan defines:

- Region (West US, East US, and so on)
- Number of VM instances
- Size of VM instances (small, medium, large)
- Pricing tier (Free, Shared, Basic, Standard, Premium, Premium V2, Isolated)

### Select a region

Typically, you would choose a region geographically close to your expected customers.

### Pricing and reliability levels

Shared compute: Free and Shared, these tier will be shared resources for multiple App Services apps, and the resources cannot scale-out.

Dedicated compute:

- The Basic, Standard, Premium, and Premium V2, only apps in the same App Service plan share the same compute resources and we can scale number of its vm.

- Isolated: This tier runs dedicated Azure VMs on dedicated Azure virtual networks (it reaches highest levels of security and performance).

Isolate your app into a new App Service plan when:

- The app is resource-intensive.
- You want to scale the app independently from the other apps in the existing plan.
- The app needs resources in a different geographical region.
