Personal website.  Slowly adding more automation to it but this is more of a sandbox than a porfolio

# Current TODO
1. Set up drone.io build
	Not gonna do at this point.
2. Shift to pushing to netlify directly
	My netlify setup works but there is no error checking or piloting.
3. GCP CI/CD setup?
4. Require PR review?
	Weird setup where the `publish` branch is what pushes to prod. 
5. Swtich from gitlab to github


# Shortcuts
`
mkdir themes
cd themes
git clone https://github.com/jrutheiser/hugo-lithium-theme
`

`git checkout -b new_branch`

`git push --set-upstream origin new_branch`

`hugo new post/title.md`

`hugo server -D`

