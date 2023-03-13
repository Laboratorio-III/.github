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

## Invite
```
curl -L   -X POST  \
	-H "Accept: application/vnd.github+json"  \
	-H "Authorization: Bearer $GITTOKEN"  \
	-H "X-GitHub-Api-Version: 2022-11-28"  \
	https://api.github.com/orgs/Laboratorio-III/invitations  \
	-d '{"email":"paulmulberry@gmail.com","role":"direct_member","team_ids":[7504252]}'

```
