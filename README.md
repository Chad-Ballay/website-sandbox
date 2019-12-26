[![Netlify Status](https://api.netlify.com/api/v1/badges/a248f80b-89d3-48b7-854d-f954740a1148/deploy-status)](https://app.netlify.com/sites/quizzical-colden-1f3560/deploys)

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
`git checkout -b new_branch`

`git push --set-upstream origin new_branch`

`hugo new post/title.md`

`hugo server -D`

