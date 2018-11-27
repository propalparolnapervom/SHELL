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

## REDIRECTION

Put few lines in the file
```
cat <<EOF > /etc/yum.repos.d/kubernetes.repo
[kubernetes]
name=Kubernetes
baseurl=https://packages.cloud.google.com/yum/repos/kubernetes-el7-x86_64
enabled=1
gpgcheck=1
repo_gpgcheck=1
gpgkey=https://packages.cloud.google.com/yum/doc/yum-key.gpg https://packages.cloud.google.com/yum/doc/rpm-package-key.gpg
exclude=kube*
EOF
```

























