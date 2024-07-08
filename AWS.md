<style>
td, th {
   border: none!important;
}
</style>

# AWS

* Get branch environment variables

```
aws amplify get-branch --app-id <> --branch-name <> --query branch.environmentVaraibles 
```

* Update branch environment variables

```
aws amplify update-branch --app-id <> --branch-name <> --environment-variables "$(cat <<EOF
{
   VAR1: 'test',
   VAR2: "test2"
}
EOF
)"
```

