 # Rest

## Get all members 
```bash
curl -L   \ 
 	-H "Accept: application/vnd.github+json" \
	-H "Authorization: Bearer $GITTOKEN" \
	-H "X-GitHub-Api-Version: 2022-11-28" \
	https://api.github.com/orgs/Laboratorio-III/members
````

## Get all Teams
```bash
curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer $GITTOKEN"\
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/Laboratorio-III/teams
```
