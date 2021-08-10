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
 - Test the URL specified in the `Website Draft URL` given by above command output.
 - Once satisfied, can deploy to production URL by suffixing `--prod` option like this:
	 - `netlify deploy --prod`

