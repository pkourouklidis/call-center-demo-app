# Call Center Demonstration Application

This is an application to demostrate the capabilities of [Panoptes](https://github.com/pkourouklidis/panoptes). The app simulates incoming customers' calls to a call center and requests predictions from an ML model regarding the customers' satisfaction. Various kinds of dataset shift can be added to the simulations to illustrate how Panoptes enables ML model monitoring.

The app is split in two parts:
- Visualisation Dashboard
- Simulation Configuration Dashboard

## Visualisation Dashboard
The visualisation dashboard shows information about each simulation run such as number of calls and customers satisfaction. This component is split into 3 services:

- [User Interface](https://github.com/pkourouklidis/dashboard-user-interface)
- [Dashboard Backend](https://github.com/pkourouklidis/dashboardservice)
- [Data Service](https://github.com/pkourouklidis/dashboard-dataservice)

## Simulation Configuration Dashboard
The simulation configuration dashboard is responsible for starting/stopping call simulations. The simulations can also be configured to include various kinds of dataset shift. This component is spit into 4 services:

- [User Interface](https://github.com/pkourouklidis/digital-twin-user-interface)
- [Simulation Backend](https://github.com/pkourouklidis/digital-twin-adminservice)
- [Load Generator](https://github.com/pkourouklidis/digital-twin-loadgenerator)
- [Worker Agent](https://github.com/pkourouklidis/digital-twin-worker)

## Deployment
Helm charts are provided in this [repo](https://github.com/pkourouklidis/call-center-deployment) for the deployment of the above services on a kubernetes cluster.