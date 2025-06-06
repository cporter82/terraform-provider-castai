---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "castai_rebalancing_schedule Data Source - terraform-provider-castai"
subcategory: ""
description: |-
  Retrieve Rebalancing Schedule
---

# castai_rebalancing_schedule (Data Source)

Retrieve Rebalancing Schedule



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) Name of the schedule.

### Read-Only

- `id` (String) The ID of this resource.
- `launch_configuration` (List of Object) (see [below for nested schema](#nestedatt--launch_configuration))
- `schedule` (List of Object) (see [below for nested schema](#nestedatt--schedule))
- `trigger_conditions` (List of Object) (see [below for nested schema](#nestedatt--trigger_conditions))

<a id="nestedatt--launch_configuration"></a>
### Nested Schema for `launch_configuration`

Read-Only:

- `aggressive_mode` (Boolean)
- `aggressive_mode_config` (List of Object) (see [below for nested schema](#nestedobjatt--launch_configuration--aggressive_mode_config))
- `execution_conditions` (List of Object) (see [below for nested schema](#nestedobjatt--launch_configuration--execution_conditions))
- `keep_drain_timeout_nodes` (Boolean)
- `node_ttl_seconds` (Number)
- `num_targeted_nodes` (Number)
- `rebalancing_min_nodes` (Number)
- `selector` (String)
- `target_node_selection_algorithm` (String)

<a id="nestedobjatt--launch_configuration--aggressive_mode_config"></a>
### Nested Schema for `launch_configuration.aggressive_mode_config`

Read-Only:

- `ignore_local_persistent_volumes` (Boolean)
- `ignore_problem_job_pods` (Boolean)
- `ignore_problem_pods_without_controller` (Boolean)
- `ignore_problem_removal_disabled_pods` (Boolean)


<a id="nestedobjatt--launch_configuration--execution_conditions"></a>
### Nested Schema for `launch_configuration.execution_conditions`

Read-Only:

- `achieved_savings_percentage` (Number)
- `enabled` (Boolean)



<a id="nestedatt--schedule"></a>
### Nested Schema for `schedule`

Read-Only:

- `cron` (String)


<a id="nestedatt--trigger_conditions"></a>
### Nested Schema for `trigger_conditions`

Read-Only:

- `ignore_savings` (Boolean)
- `savings_percentage` (Number)


