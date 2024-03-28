# Prerequisites
- Az Admin Exam (Optional)
- Az Fundamental Understading
- Basic Hands-On Experience.
- Scripting languages.

# Sections of Exam
- Develop an instrumentation strategy [5-10%]
- Develop a site reliability Engineerig (SRE) Strategy
- Develop a security and compliance plan
- Manage Source Control
- Facilitate communication and collaboration
- Define and implement continous integration
- Define and implement a continous delivery and release management strategy

# 1. Develop an instrumentation strategy
- Monitor and Measure Performance
- Detect Errors
- Trace Information
- Visibility, Notifications, Cost Efficiency.

### Design and Implement Strategies
- Logging: A log aggregation and query strategy using Azure Monitor.
- Telemetry: Define and measure key metrics, such as CPU, network and disk.
- Alerts: Implement metric alerts to notify team members.

### Azure Monitor
![](AzureMonitor.svg)  
- How various applications are doing and issues that may occur.
- Data Collected
  - Application
  - OS
  - Azure Resources (Such as ExpressRoute)
  - Azure Subscription
  - Azure Tenant
- Collected data flows through Logs and Metrics.
- Metrics
  - Performance of resources
  - Consumption of resources
- Extend Data Collection
  - Enable diagnostics and add an agent
  - Enable monitoring with application insights

 You can go to monitorig by
 -> Select VM -> Overview -> Monitoring;
 -> If above info is not enough we can see more details on monitoring in left pane
 -> Insights, Alert, Metrics, Diagnostic setting, Logs, Connection Monitor, Workbooks are all parts of Monitoring.

## Key Metrics
- Input
  - Azure Resources (CPU, Memory, Disk, Network)
    - Monitoring -> Metrics -> Fill the details like Scope, Metric Namespace (Custom Guest)-> Metric (Logical disk disk writes) -> Aggregation (Average).
  - Applications
  - Virtual Machine Agents
  - Custom Metrics
- Metrics
  - Insights
  - Dashboards
  - Workbooks
  - Metrics Explorer
  - Metric Alerts
    - VM -> Monitoring -> Alert -> Create alert rule (As you have gone here through VM, VM details will be autofilled ->
    - Condition (Add Condition), Outbound(Outbound Flows) , Operator (>) -> Aggregation Average -> Threshold Value (Some Percentage)
    - Action Group -> Create/Add Action Group

# 2. Develop a site reliability Engineerig (SRE) Strategy
- Main benefit of SRE Strategy is it reduces downtime.

## Healthcheck
### Health Check Types
- Contaier liveness and readiness probes
- Startup
- Shutdown

### Azure Container Instances
- Support Readiness Probes
- Depploying container group that involves readiness Probe

    Console
    create readiness-probe.yml file
    

