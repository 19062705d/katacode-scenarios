# Step 6: Grafana Alert
Grafana alerting allows you to attach rules to your dashboard panels. When you save the dashboard, Grafana extracts the alert rules into a separate alert rule storage and schedules them for evaluation.

The alerting engine publishes some internal metrics about itself. You can read more about how Grafana publishes internal metrics. See also, View alert rules and their current state.

#### alerting.alerts
type:  gauge
description: 

#### alerting.alerts
type: gauge<br>
description: How many alerts by state

#### alerting.request_duration_seconds
type: histogram <br>
description: Histogram of requests to the Alerting API

#### alerting.active_configurations
type: gauge<br>
description: The number of active, non default alertmanager configurations for grafana managed alerts

#### alerting.rule_evaluations_total
type: counter<br>
description: The total number of rule evaluations

#### alerting.rule_evaluation_failures_total
type: counter<br>
description: The total number of rule evaluation failures

#### alerting.rule_evaluation_duration_seconds
type: summary<br>
description: The duration for a rule to execute

#### alerting.rule_group_rules
type: gauge<br>
description: The number of rules


