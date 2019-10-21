## New chapter requests
- [All open requests](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter)
- [Open requests awaiting repo creation](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter+-label%3Arepo-created) (waiting on maintainer)
- [Open requests with repo already created](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter+label%3Arepo-created) (waiting on chapter organizer to submit PR to add to listings)

## Instructions for chapter repo setup

When a request comes in, vet request and ensure all details needed for chapter setup have been provided.

Follow these steps to create a new chapter repo after a request has been vetted:

### Tell organizer(s) you're getting started
1. Respond to the appropriate [new chapter request](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter) using the appropriate convo template, adding organizer handles where indicated:
  - ["Setting up repo"](convo-templates/01b-setting-up-repo.md) (if all details provided)
  - ["Need CoC details"](convo-templates/01a-need-coc-contact.md)

### Create chapter repo

1. Click to [create a new repo](https://github.com/organizations/ProtoSchool/repositories/new)
2. Under "Repository template," select "ProtoSchool/chapter-repo-template"
3. Fill in repository name, eg `munich` or `san-francisco`
4. Fill in description, eg "ProtoSchool Munich"
5. Leave other settings as is

### Customize template files

Because you started from a repository template, the new repository will already include the following files:
- README.md (requires customization)
- CODE_OF_CONDUCT.md (requires customization)
- LICENSE.md (no updates required)

_To view or update the chapter repository template, visit the [`chapter-repo-template` repo](https://github.com/ProtoSchool/chapter-repo-template)._

#### Update README.md
1. Click pencil icon from homepage.
2. Replace [LOCATION], [NAME], and [HANDLE] fields in readme.
3. Click "preview changes" to ensure formatting comes out correctly (links most likely to have errors)
4. In "commit changes" section, set title and description as "Update location and organizer details"
5. Click "commit changes" to merge (Currently merging directly to master during setup)

#### Update CODE_OF_CONDUCT.md
1. Click "Code" at top left, then select "CODE_OF_CONDUCT.md"
3. Click pencil icon at top right to make edits
4. Replace [LOCATION] with the chapter location.
5. Update [NAME] and [EMAIL] in the reporting section with relevant details, using one of the following formats:

##### Single organizer
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting chapter organizer **NAME** at **[EMAIL](mailto:EMAIL)**.
```

##### Mutliple organizers with individual email addresses
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting chapter organizers **NAME ([EMAIL](mailto:EMAIL))**,
**NAME ([EMAIL](mailto:EMAIL))**, or **NAME ([EMAIL](mailto:EMAIL))**.
```

##### Multiple organizers sharing an email address
```md
Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the chapter organizing team at
**[EMAIL](mailto:EMAIL)**.
```

6. In "commit changes" section, set title and description to  "Update CoC location and reporting contacts"
7. Click "commit changes" to merge (Currently merging directly to master during setup)

### Add default issues
_As of 10/21/19, it's not possible to have issues in a template repo carry over into a new repo built from it, so this step must be done manually._
1. Add ["Personalize README.md & add calls to action"](issue-templates/01-personalize-repo.md) as is (copy title and body separately)
3. Add ["Review Code of Conduct"](issue-templates/02-review-coc.md) (check which version is needed, copy title and body separately)
4. Add ["Add chapter to our listings"](issue-templates/03-add-chapter-listing.md) as is (copy title and body separately)
5. Add "chapter-setup" label to all 3 setup issues


### Set up admins and teams

#### Add repo admins
1. Click "settings" at top right
2. Click "collaborators and teams" at top left
3. Under collaborators, add each co-organizer (don't include @ sign)
4. Set each co-organizer to admin status


#### Create chapter team and add organizer(s) to it
1. While still in Collaborators & Teams within the chapter repo, click "Create new team"
3. Set team name to match repo name
4. Set description as "CITY chapter members"
5. leave remaining settings as is and click "create team"
6. Click plus sign at left and repeat invite process to add all organizers to new team


#### Add organizer(s) to #chapter-organizers team
1. Click to [add member to the `chapter-organizers` team](https://github.com/orgs/ProtoSchool/teams/chapter-organizers/members?add=true)
2. Invite first organizer
3. Click "add a member" to invite additional organizers (repeat until all are added)
4. Continue until all organizers invited

### Watch the chapter repo
1. Visit chapter repo
2. Click watch & be notified of all conversations

### Tell organizer(s) repo is ready
1. Go to list of [new chapter requests](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter)
2. Check box next to correct repo, click "label" and select "repo-created"
3. Open issue
4. Copy ["Repo ready"](convo-templates/02-repo-ready.md) conversation template into new comment in issue and replace [ORGANIZER] and [CHAPTER] placeholders - proof carefully!

_Wait for organizers to submit PR to add chapter to website._

### Review and merge PR to add chapter to the website
1. When organizer submits PR to add to site, first check repo to ensure it has a CoC with contact info and a complete readme. Check their issue queue to make sure all organizers have agreed to the CoC and there's nothing you need to help fix. If it looks okay, merge the PR.
2. Return to [chapter setup request list](https://github.com/ProtoSchool/organizing/issues?q=is%3Aissue+is%3Aopen+label%3Anew-chapter) and select correct setup issue
3. Copy [Added to Website](convo-templates/03-added-to-website.md) conversation template into new comment in issue
4. Click "comment and close"
5. Do the same in the issue within their chapter repo
