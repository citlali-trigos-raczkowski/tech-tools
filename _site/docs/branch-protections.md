## Github Branch Protections 

[Branch Protections](https://docs.github.com/en/enterprise-server@3.0/github/administering-a-repository/managing-a-branch-protection-rule

A great starting point is to require at least one approval before merging to master:
```
> go to your repository 
> Settings
> Branches
    > Type `master` into Branch name pattern
    > Add Rule as shown in screenshot
> Save changes
```
![sample branch rule](./static/branch-rule-sample.png)