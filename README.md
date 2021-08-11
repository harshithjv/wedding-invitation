# Wedding Invitation!

Static website developed for my online wedding invitation
### [Live on netlify](https://harshith-weds-nishitha.netlify.app)

# Files

Simple HTML templates stored and edited on `site` folder. Deployed the same on `netlify site`.

## Steps to deploy.

After forking & cloning:

 - Sign up with your `Github` account on netlify wesbite here: https://app.netlify.com/signup
 - Install `Netlify CLI` on your local node installation:
	 - `npm install netlify-cli -g`
	 - Docs: https://docs.netlify.com/cli/get-started/
 - Login to CLI
	 - `netlify login`
 - On terminal, change to repo directory. Make some changes and then:
	 - `netlify deploy`
     - _Note_: If you make changes to files like `.html` files, please push to github and run the above command. Some static updates locally don't get reflected when there is no build command supplied for the given repo.
 - Test the URL specified in the `Website Draft URL` given by above command output.
 - Once satisfied, can deploy to production URL by suffixing `--prod` option like this:
	 - `netlify deploy --prod`

_Note:_ If your planning to build different project and reading this document for help, then observe the `netlify.toml` file in this project. The file contents are bare minimum:
```
[build]
publish = "site"
```
Here `publish` is set to destination directory. For static and barebones html, css and vanilla JS sites, nothing else is required.

## Why Netlify? And not GitHub pages?

To be honest for this project Github pages is well-suited as it contains only static pages. Does not contain `react` or even `express` implementation.

I'd initially thought I will utilize `functions` and `forms` features provided by `netlify`. Also I scraped the idea of converting these templates to `react` code, since this template depended on `jQuery` and other libraries. Conversion process lead lot of re-works for scroll animations and other parts of the template. On the downside I'd to replicate lot of code across 4 html pages.

Overall `netlify` gave a fresh learning experience. So continued with deploying this on `netlify`. For `GitHub pages`, its preferred to place code in root of the directory or in `docs` directory ideally `gh-pages` where continues deployment is set up automatically once `Github pages` is enabled on the repo.

For `netlify` it was not straight-forward and I'd to `google` a lot as to where the issue occured. Though they advertise that it's very easy using the `netlify`, adding `site` directly from `GitHub` repo does not deploy the website for static pages. It works well if you've set the `command` field to some build job which does not work for static sites like this even if you left the field blank.

So there you've it. I'm not using the `netlify` to utilize its full potential. But it gave me lot of learning experience.
