## Running Locally


```sh-session
git clone https://github.com/mughees936/blogsite.git
cd blogsite
```


Create a `.env` file similar to [`.env.example`](.env.example).

Then install dependencies and run the development server:
```sh-session
pnpm install
pnpm dev
```


## Cloning / Forking

Please remove all of my personal information (projects, images, etc.) before deploying your own version of this site.

## View Counting Setup (Redis)

This project uses [Upstash Redis](https://upstash.com/) to track page views.

1.  **Create Database**: Sign up at [Upstash](https://upstash.com/) and create a new Redis database.
2.  **Get Credentials**: Copy the `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` from the dashboard.
3.  **Configure Environment**:
    - **Locally**: Add these variables to your `.env` file.
    - **Vercel**: Add these variables in your project settings under "Environment Variables".

If these variables are not set, the view counter will gracefully fallback to showing `0` views.
