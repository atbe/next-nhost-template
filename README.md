- [Setup an nhost project](#setup-an-nhost-project)
- [Use Abes nextjs template repo](#use-abes-nextjs-template-repo)
- [Connect our local repo to the nhost project](#connect-our-local-repo-to-the-nhost-project)

<h1>Using this template</h1>

1. Setup an nhost project
2. Use Abes nextjs template repo
3. Connect our local repo to the nhost project
4. Run the nhost project locally
5. Deploy it to vercel

### Setup an nhost project

Create your project at https://app.nhost.io/new

This creates:

1. A postgresql database
2. A hasura graphql server
3. A nhost project
4. A `hasura-auth` server
5. CI/CD pipeline for your hasura metadata + database migrations

### Use Abes nextjs template repo

1. Go to https://github.com/atbe/next-nhost-template
2. Click the button `Use this template` at the top of the page
3. Clone the repo to your computer
4. Run `yarn install` on the template repo

### Connect our local repo to the nhost project

1. Install the nhost cli
   ```bash
   sudo curl -L https://raw.githubusercontent.com/nhost/cli/main/get.sh | bash
   ```
2. Init the project
   ```bash
   	nhost init --remote
   ```
3. Start the nhost server
   ```bash
   nhost up
   ```
4. In another terminal, start the nextjs project
   ```bash
   yarn run dev
   ```
