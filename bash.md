# Bash tips and tricks

## Is variable empty or unset?

```bash
if [ -z "${MY_VAR}" ]; then
  echo "It's empty or unset"
fi
```

## Default values
```bash
${MY_VAR-default} # If MY_VAR is defined, use it; otherwise default
```
For variations on the theme, see e.g. [Bash FAQ](http://mywiki.wooledge.org/BashFAQ/073)