# Reference materials for ProtoSchool project maintainers


## Chapter Setup


### New chapter requests: 
- [All open requests](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter)
- [Open requests awaiting repo creation](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter+-label%3Arepo-created) (waiting on maintainer)
- [Open requests with repo already created](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter+label%3Arepo-created) (waiting on chapter organizer to submit PR to add to listings)

### Instructions for chapter repo setup

Follow these steps to create a new chapter repo after a request has been vetted: 

#### Create chapter repo

1. Go to https://github.com/organizations/ProtoSchool/repositories/new
2. Under "Repository template," select "ProtoSchool/chapter-repo-template"
3. Fill in repository name, eg `munich` or `san-francisco`
4. Fill in description, eg "ProtoSchool Munich"
5. Leave other settings as is

#### Customize template files

Because you started from a repository template, the new repository will already include the following files:
- README.md (requires customization)
- CODE_OF_CONDUCT.md (requires customization)
- LICENSE.md (no updates required)

##### Update README.md
1. Click pencil icon from homepage.
2. Replace [LOCATION], [NAME], and [HANDLE] fields in readme.
3. Click "preview changes" to ensure formatting comes out correctly (links most likely to have errors)
4. In "commit changes" section, set title and description as "Update location and organizer details"
5. Click "commit changes" to merge (Currently merging directly to master during setup)

##### Update CODE_OF_CONDUCT.md
1. Click "Code" at top left, then select "CODE_OF_CONDUCT.md"
3. Click pencil icon at top right to make edits
4. Replace [LOCATION] with the chapter location.
5. Update [NAME] and [EMAIL] in the reporting section with relevant details, using one of the following formats:

###### Single organizer
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting chapter organizer **NAME** at **[EMAIL](mailto:EMAIL)**.
```

###### Mutliple organizers with individual email addresses
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting chapter organizers **NAME ([EMAIL](mailto:EMAIL))**,
**NAME ([EMAIL](mailto:EMAIL))**, or **NAME ([EMAIL](mailto:EMAIL))**.
```

###### Multiple organizers sharing an email address
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the chapter organizing team at
**[EMAIL](mailto:EMAIL)**.
```

6. In "commit changes" section, set title and description to  "Update CoC location and reporting contacts"
7. Click "commit changes" to merge (Currently merging directly to master during setup)

#### Add default issues
1. Add "Personalize README.md & add calls to action" as is (copy title and body separately)
3. Add "Review Code of Conduct" (check which version is needed, copy title and body separately)
4. Add "Add chapter to our listings" as is (copy title and body separately)
5. Add "chapter-setup" label to all 3 setup issues


#### Set up admins and teams

##### Add repo admins
1. Click "settings" at top right
2. Click "collaborators and teams" at top left
3. Under collaborators, add each co-organizer (don't include @ sign)
4. Set each co-organizer to admin status


##### Create chapter team and add organizer(s) to it
1. While still in Collaborators & Teams, click "Create new team" (or visit https://github.com/orgs/ProtoSchool/new-team to add a new team)
3. Set team name to match repo name
4. Set description as "CITY chapter members"
5. leave remaining settings as is and click "create team"
6. Click plus sign at left and repeat invite process to add all organizers to new team
7. Visit https://github.com/ProtoSchool, scroll down and select name of new chapter
10. click "settings" at top right
11. click "collaborators and teams" at top left
12. click "add a team" in middle and select name of new chapter

##### Add organizer(s) to #chapter-organizers team
1. Visit https://github.com/orgs/ProtoSchool/teams/chapter-organizers/members?add=true to add someone to the chapter-organizers team
5. invite first organizer
6. click "add a member"
7. invite another organizer
8. continue until all organizers invited

#### Tell organizer(s) know repo is ready
1. Go to list of new repo requests: https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter
2. Check box next to repo, click "label" and select "repo-created"
3. Open issue
4. Copy "repo_ready" conversation template into new comment in issue and replace [ORGANIZER] and [CHAPTER] placeholders - proof carefully!

_Wait for organizers to submit PR to add chapter to website._

#### Review and merge PR to add chapter to the website
1. When organizer submits PR to add to site, first check repo to ensure it has a CoC with contact info and a complete readme. Check their issue queue to make sure all organizers have agreed to the CoC and there's nothing you need to help fix. If it looks okay, merge the PR.
2. Return to chapter setup request list: https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter
3. Open their chapter setup issue and add a new comment using "added-to-website" conversation template
4. Click "comment and close"
5. Do the same in the issue within their chapter repo

#### Watch the chapter repo
1. Visit chapter repo
2. Click watch & be notified of all conversations
