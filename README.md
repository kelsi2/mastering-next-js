# Mastering Next.JS

This repo follows along with the Next.JS tutorial from Lee Robinson at [masteringjs.com](https://masteringnextjs.com/).

- Next is a framework for building React apps and includes server-side rendering (makes fullstack building much easier, not just for front end)
  - Can also be used for static sites and they will be extremely fast (cached pages and smaller than a regular React app) -> not only good for dynamic sites

* No config needed, easy to build products quickly
* Server-side rendering allows for better SEO than React (if it's on the frontend it's harder for search engines to find the info)
* No need for React Router, can use file-based routing (if the page is in the pages folder routing exists automatically)

## Navigating Between Pages

- Can use built in Link component from next
  - First child MUST be an a tag because this gets appended to the DOM
  * Link uses client-side transitions (very fast!)
    - Next pre-fetches any links on a page so when a user actually navigates there it seems instantaneous!

* Use [] for dynamic routing, e.g. posts/[id] will create a dynamic slug for each post
  - useRouter hook dynamically routes between pages
* getInitialProps is a lifecycle method that allows us to fetch props before the data is rendered

---

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
