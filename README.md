# run_agent

#### Table of Contents

1. [Description](#description)
2. [Usage - Configuration options and additional functionality](#usage)
3. [Reference](#reference)

## Description

A Bolt task to run the Puppet agent on a number of nodes until there are no changes; specifically, until `--detailed-exitcodes` returns 0.

## Usage

```
bolt task run --nodes <node-name> run_agent::run_agent retries=<value> wait_time=<value>
```

## Reference

### run_agent::run_agent

#### Parameters

##### retries

The number of times to retry the agent run before failing.

Default: 5

#### wait_time

The time in seconds to wait for a running agent lock to finish.

Default: 300
