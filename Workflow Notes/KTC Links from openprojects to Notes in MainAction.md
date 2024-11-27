## Overview of KTC Standards
Use name of vault on same filesystem
- `obsidian://open?vault=my%20vault`
	- obsidian://open?vault=MainAction
		- [Open MainAction](obsidian://open?vault=MainAction)
Use name of vault and file, with "file" the path from the vault root
- `obsidian://open?vault=my%20vault&file=my%20note`
- obsidian://open?vault=MainAction&file=Organizations%2FKenya%2FKTC-Standards
	-  [Open KTC-Standards](obsidian://open?vault=MainAction&file=Organizations%2FKenya%2FKTC-Standards)
	- [Open Kibera Town Centre](obsidian://open?vault=MainAction&file=Organizations%2FKenya%2FKibera%20Town%20Centre%20KTC)
	- [Open KTC Evaluations](obsidian://open?vault=MainAction&file=Action%2FKTC%20Evaluations)
	- [Open KTC Kibera Town Centre](obsidian://open?vault=MainAction&file=Roam%2FNetDay%2FKTC%20Kibera%20Town%20Centre)
	- [Open KTC RR Plan](obsidian://open?vault=MainAction&file=Roam%2FNetDay%2FKTC.RR%20Plan)

Absolute path:
- `obsidian://open?path=%2Fhome%2Fuser%2Fmy%20vault%2Fpath%2Fto%2Fmy%20note`
	- '/Users/johngage/Obsidian.in.JG/MainAction/Roam/NetDay/KTC Slack.md'
	- [Content KTC Slack with pathname](obsidian://content?path=%2FUsers%2Fjohngage%2FObsidian.in.JG%2FMainAction%2FRoam%2FNetDay%2FKTC Slack)
		- doesn't embed
	- [Open KTC Slack with pathname](obsidian://open?path=%2FUsers%2Fjohngage%2FObsidian.in.JG%2FMainAction%2FRoam%2FNetDay%2FKTC Slack)
	- works
Try obsidian :// vault
-  `obsidian://vault/my vault/my note` is equivalent to `obsidian://open?vault=my%20vault&file=my%20note`.
	- [try obsidian://vault](obsidian://vault/MainAction/Roam/NetDay/KTC Slack)
		- works
	- 
obsidian: and two slashes and url without .md works
- `obsidian:///absolute/path/to/my note` is equivalent to `obsidian://open?path=%2Fabsolute%2Fpath%2Fto%2Fmy%20note`.

- [Try 3 slashes and slashes](obsidian:///Users/johngage/Obsidian.in.JG/MainAction/Roam/NetDay/KTC Slack)
	- works