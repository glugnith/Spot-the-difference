There are two parts of a commit message: subject and body.
Not every commit message required body; some commits are so simple that a single line is fine.
eg: Fix a typo in README.md

## Separate subject from body with a blank line

Git log prints subject+body
Git log --oneline prints only subject
git shortlog, which groups commits by user, again showing just the subject line for concision.

## Limit the subject line to 50 characters

50 characters is not a hard limit, just a rule of thumb. Keeping subject lines at this length ensures that they are readable, 
and forces the author to think for a moment about the most concise way to explain what’s going on.
And will truncate any subject line longer than 72 characters with an ellipsis, So shoot for 50 characters, but consider 72 the hard limit.

## Capitalize the subject line

## Do not end the subject line with a period

Trailing punctuation is unnecessary in subject lines. Besides, space is precious when you’re trying to keep them to 50 chars or less.

## Use the imperative mood in the subject line

Imperative mood just means “spoken or written as if giving a command or instruction”. A few examples:
Clean your room
Close the door
Take out the trash

Git itself uses the imperative whenever it creates a commit on your behalf.

For example, the default message created when using git merge reads:
Merge branch 'myfeature'

And when using git revert:
Revert "Add the thing with the stuff"
This reverts commit cc87791524aedd593cff5a74532befe7ab69ce9d.

So when you write your commit messages in the imperative, you’re following Git’s own built-in conventions. 
For example:
Refactor subsystem X for readability
Update getting started documentation
Remove deprecated methods
Release version 1.0.0

#### A properly formed Git commit subject line should always be able to complete the following sentence: 

If applied, this commit will your subject line here

For example:
If applied, this commit will refactor subsystem X for readability
If applied, this commit will update getting started documentation

## Wrap the body at 72 characters

Git never wraps text automatically. When you write the body of a commit message, you must mind its right margin, and wrap text manually.
The recommendation is to do this at 72 characters, so that Git has plenty of room to indent text while still keeping everything under 80 characters overall.

## Use the body to explain what and why vs. how

In most cases, you can leave out details about how a change has been made. 
Code is generally self-explanatory in this regard (and if the code is so complex that it needs to be explained in prose, that’s what source comments are for).
Just focus on making clear the reasons why you made the change in the first place—the way things worked before the change (and what was wrong with that), 
the way they work now, and why you decided to solve it the way you did.