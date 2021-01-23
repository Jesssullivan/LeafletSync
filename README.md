*A ridiculous utility prompt & CLI for fetching private releases & files from GitHub & BitBucket*


```
wget https://raw.githubusercontent.com/Jesssullivan/LeafletSync/main/LeafletSync && chmod +x LeafletSync && ./LeafletSync
```

- Fetch, unpack, extract releases & output files from a private GitHub repo with an api access token
- Fetch specific files from a private BitBucket account with user's git authentication
- Prefill default prompt values with a variety of console flags
- Save & load default prompt values with a file of environment variables; see template [`sampleEnv`](https://github.com/Jesssullivan/LeafletSync/blob/main/sampleEnv)

```
./LeafletSync

LeafletSync: Do you want to load values from a file?

If so, enter one now...:[Nope!]:  

_                 __ _      _     _____                    
| |               / _| |    | |   /  ___|                   
| |     ___  __ _| |_| | ___| |_  \ `--. _   _ _ __   ___  
| |    / _ \/ _` |  _| |/ _ \ __|  `--. \ | | | '_ \ / __|
| |___|  __/ (_| | | | |  __/ |_  /\__/ / |_| | | | | (__   
\_____/\___|\__,_|_| |_|\___|\__| \____/ \__, |_| |_|\___|  
\                      _____________________/ |             
 \ Fetch from Github: /        α wιρ Σ ♥ |_@__Jess          
 /───────────────────/
 \ Your API Token    | -t |  --token | Required | = personal-api-token
  | Your Handle      | -u |  --user  | Required | = You
  | Source Repo      | -r |  --repo  \ Required  \ = RepoName
  | Repository Owner | -a |  --author \ Required  \ = TheOwner
  | Release Version  | -v |  --version | Required | = v0.0.1
 / Output Directory  | -o |  --out    / Optional  / = dist/
/─────────────────────────/
\ Fetch from BitBucket:  /                                     
 \──────────────────────/                                   
  \  Your Handle       / -bu  /  --b-user  / ~Required | = You
   \ Your Passhrase   / -bp  / --b-pass   / ~Required / = personal-api-token
    \ Source Branch  / -bb  / --b-branch / ~Optional / = master
     \ Source File  / -bf  / --b-file   / ~Required / = <FileInBitBucket>
      \────────────/

Your Handle [<You>]:

Source Repo [<RepoName>]:

Repo Owner [<TheOwner>]:

Host: GitHub | BitBucket [GitHub]:

Your Token [<personal-api-token>]:

Release to fetch: [<v0.0.1>]:

Output to fetch (e.g. /dist/*): [<dist/>]:

...

```
