## Use Harness expressions. For most settings in Harness pipelines, you can use fixed values, runtime inputs, or expressions.

### For retreiving the secrets value in pipeline. Replace "project.access_token" with secret key id

```
<+secrets.getValue("project.access_token")>
```

### For retreiving the AppName value pipeline variables

```
<+pipeline.variables.AppName>
```

### For retreiving the TargetGroup ARN from output variables of 'Create_Target_Group step' of 'Deploy' Stage

```
<+pipeline.stages.Deploy.spec.provisioner.steps.Create_Target_Group.output.target_group_arn>
```
