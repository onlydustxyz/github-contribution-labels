# github-contribution-labels

## How to use ?

### Warning

The operation described bellow can be slightly destructive. Please make sure to understand it before running it.  
You can also do `dry-run` by using the `-d` option.

### Install [github-label-sync](https://github.com/Financial-Times/github-label-sync)

```shell
npm install -g github-label-sync
```

### Add the contribution labels to you repository

```shell
GITHUB_ACCESS_TOKEN-""
github-label-sync -a $GITHUB_ACCESS_TOKEN -l ./github-contribution-labels/labels.json -A <organisation>/<repository>
```

## Customization

If some of your already existing labels overlap with the one being added, you can specify them as aliases in `labels.json` and they will be automaticaly converted to their new counterparts.
