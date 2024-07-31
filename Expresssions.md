## Use Harness expressions. For most settings in Harness pipelines, you can use fixed values, runtime inputs, or expressions.

### For retreiving the secrets value in pipeline

```
<+sercets.getValue("project.access_token")>
```

### For retreiving the pipeline variables

```
<+pipeline.variables.variable_name>
```
