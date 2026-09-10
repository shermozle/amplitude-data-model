# The Amplitude data model

Interactive teaching material on how the Amplitude data model works, written for
people who know Adobe Analytics well. Seven tools covering the event, scope,
identity, cohorts and arrays.

Examples use a fictional broadband and mobile retailer. Nothing here is drawn from
any particular implementation, and Adobe appears throughout as the reference frame
rather than the subject.

```
index.html              hub page
data-model-tools.html   the seven tools
user-profile.png        screenshot used in tool 04
.nojekyll               stops GitHub running Jekyll over the files
```

Plain HTML, no build step. Open `index.html` directly or serve the directory.

## Editing

Everything lives in `data-model-tools.html` — styles, markup and behaviour in one
file. Content for the interactive panels is in the data structures at the top of
each tool's script block (`JOURNEY`, `J2`, `IDROWS`, `SCENARIOS`, `COHORTS`,
`TERMS`), so most changes are edits to those rather than to markup.

Fonts load from Google Fonts and fall back to system fonts if that's blocked.
There are no other external requests and no absolute paths, so it works from a
project subpath as well as a domain root.
