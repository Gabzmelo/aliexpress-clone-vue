# AliExpress Clone

An full stack project made using:
- Nuxt 3
- Vue.js
- Tailwind CSS
- Supabase
- Prisma
  
You can access the website in production [here](https://aliexpressclonevue.netlify.app/)

## Setup

```bash
  git clone https://github.com/Gabzmelo/aliexpress-clone-vue.git
```
Create the `.env` file like the example and set the Stripe and Supabse connection keys:

```bash
STRIPE_PK_KEY=(PUBLISHABLE KEY)
STRIPE_SK_KEY=(SECRET KEY)

SUPABASE_URL="(PROJECT URL)"
SUPABASE_KEY="(API KEY)"

DATABASE_URL="(CONNECTION STRING)"
```
After connecting your keys, you'll also need to setup the Auth for Google and GitHub

```bash
https://supabase.com/docs/guides/auth/social-login/auth-google
https://supabase.com/docs/guides/auth/social-login/auth-github
```

Once this is done, install the dependencies and start the server:

```bash
  npm i

  npx prisma generate

  npm run dev
```

And run the command to migrate your database tables and run your seed file.

```bash
  npx prisma migrate dev --name init
```
