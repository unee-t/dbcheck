We want to capture across our uneet-{dev,demo,prod} accounts:

- [ ] uptime
- [ ] engineversion
- [ ] dbInstanceClass
- [ ] user_group_map count - so we know if there has been any truncation issues
- [X] schema_version - so we know what version of the data structure we are running
- [X] aurora_version - so we know what version of the database we are running
- [ ] snapshot_time (PreferredBackupWindow) - so we know at what time snapshot are being taken
- [ ] BackupRetentionPeriod - so we know how far back we can restore
- [ ] needing_reboot - so we know if all our settings are in affect
- [ ] binlog_time - whether binlogs are enabled and how far they go
- [X] iam_auth - whether IAM auth is enabled
- [X] slow_log - whether slow log is enabled
- [ ] general_log - whether general log is enabled
- [ ] cluster_endpoint - so we know what the cluster endpoint URL is
- [ ] backtrack - if we can back track and what is the window
- [ ] cloudwatch - check whether logs are being output to CloudWatch
- [ ] check [lambda_async](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/AuroraMySQL.Integrating.Lambda.html) is present
- [ ] check triggers are enabled
- [ ] check innodb_file_format

https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_LogAccess.Concepts.MySQL.html
