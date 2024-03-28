

## External Tools

### Messaging Apps
- Teams and Slack
- Create a team
- Install Boards/Repos/Pipelines app or plugin
- Create a channel for


### Creating Alerts in Teams:
- Create Team in Enterprise account.
- Apps> Search-> Azure( Boards/Repos/Pipelines -> Add to Team-> Select Team).

### Messaging: Integrating Azure DevOps Boards.
- Authenticate:
    "@azure boards signin"
    "/azboards signin"
- Link channel to project:
    "@azure boards link <project url>"
    "/azboards link <project url>"
- Setup & manage subscriptions:
    "@azure boards subscriptions"
    "/azboards subscriptions"

### Messaging: Integrating Azure DevOps Repos
- Authenticate:
    "@azure repos signin"
    "/azrepos signin"
- Link channel to project:
    "@azure repos subscribe <project/repo url>"
    "/azrepos subscribe <project/repo url>"
- Setup & manage subscriptions:
    "@azure repos subscriptions"
    "/azrepos subscriptions"

### Messaging: Integrating Azure DevOps Pipelines
- Same as Repos just replace repos with Pipelines.

### Service Hooks
- These subscription can be used to integrate Azure DevOps with third-party services.
- Triggered by a specific Azure DevOps Event
Example: pushing code, build completing, etc.
- You select a specific action a card/listto be performed.
Example: creating in Trello

Webhooks are similar: They run with a trigger and as an action post JSON to HTTP(s) endpoint.
