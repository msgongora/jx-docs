---
date: 2019-01-25T17:16:08Z
title: "jx get build log"
slug: jx_get_build_log
url: /commands/jx_get_build_log/
---
## jx get build log

Display a build log

### Synopsis

Display a build log

```
jx get build log [flags]
```

### Examples

```
  # Display a build log - with the user choosing which repo + build to view
  jx get build log
  
  # Pick a build to view the log based on the repo cheese
  jx get build log --repo cheese
  
  # Pick a pending knative build to view the log based
  jx get build log -p
  
  # Pick a pending knative build to view the log based on the repo cheese
  jx get build log --repo cheese -p
  
  # Pick a knative build for the 1234 Pull Request on the repo cheese
  jx get build log --repo cheese --branch PR-1234
```

### Options

```
      --branch string            Filters the branch
  -b, --build string             The build number to view
  -c, --current                  Display logs using current folder as repo name, and parent folder as owner
  -f, --filter string            Filters all the available jobs by those that contain the given text
  -h, --help                     help for log
  -o, --owner string             Filters the owner (person/organisation) of the repository
  -p, --pending                  Only display logs which are currently pending to choose from if no build name is supplied
  -r, --repo string              Filters the build repository
  -t, --tail                     Tails the build log to the current terminal (default true)
  -w, --wait                     Waits for the build to start before failing
  -d, --wait-duration duration   Timeout period waiting for the given pipeline to be created (default 5m0s)
```

### SEE ALSO

* [jx get build](/commands/jx_get_build/)	 - Display one or more build resources

###### Auto generated by spf13/cobra on 25-Jan-2019
