# Commands Project

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

Simple project shows a [command_job.rb](app/jobs/command_job.rb) class that allows you to run any command remotely on AWS Lambda.

This could be used to do maintenance things like migrate the database if you only have access to the database within Lambda: [How do I Migrate the Database?](https://community.rubyonjets.com/t/how-do-i-migrate-the-database/22/3)

There is a general `execute` method where you and specific the command in the event payload, example:

```json
{
  command: "whoami"
}
```

## More Examples

[tongueroo/jets-examples](https://github.com/tongueroo/jets-examples)
