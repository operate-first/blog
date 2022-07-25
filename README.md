# ARCHIVED

Blog posts are included in the main website.
Create PRs to https://github.com/operate-first/operate-first.github.io/tree/main/content/posts

# [Operate First Blog](https://www.operate-first.cloud/blog/)

This is based on https://github.com/LekoArts/gatsby-starter-minimal-blog - please read the documentation before you continue!

### Previewing your changes on GitHub pages

We use Netlify to preview PR changes. Each PR will show a Netlify check that can be used to access a dynamically generated build and deployment of that PR.

### Manual Site Deployment (Production GitHub Pages)

CI will deploy to GitHub pages automatically on every push to default branch as well on daily schedule. You can trigger a new build manually if you have _write_ permissions on this repo by simply clicking **Run workflow** button on the [CI workflow details screen here](https://github.com/operate-first/blog/actions/workflows/build_job.yaml).

Fully manual build is possible by issuing following commands (requires _write_ access to the repo):

```sh
npm install
npm deploy
```
