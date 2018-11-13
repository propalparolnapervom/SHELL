# SHELL-SCRIPTING OVERALL

[Docs #1](https://devhints.io/bash)


## PARAMETERS

### Indirect expansion

[Shell Parameter Expansion](http://www.gnu.org/software/bash/manual/html_node/Shell-Parameter-Expansion.html)

View not Parameter Name, but Parameter Value
```
export NAME=sergii
export FULL_NAME=NAME

echo $FULL_NAME
  
  NAME


echo ${!FULL_NAME}
  
  sergii
```

Replacement of previous approach
```
eval REPLACEMENT=\$$FULL_NAME

echo $REPLACEMENT

  sergii

```


























