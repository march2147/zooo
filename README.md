# 🦓 Zoo

A playground for comparing AI image models.

## Usage

This is a [Next.js](https://nextjs.org/) app. To run it locally, you'll need to install [Node.js](https://nodejs.org/en/).

Install dependencies:

```console
npm install
```

Then, copy the `.env.example` file, name it `.env.local`, and fill in your credentials.

You'll need a running ngrok server to receive the [webhooks](https://replicate.com/docs/reference/http#predictions.create--webhook) from Replicate.

To do this, [install ngrok](https://ngrok.com/), and run it with `ngrok http 3000`. You'll see two forwarding addresses. Copy the `https` URL and enter it as your `NGROK_URL`

Then, run the development server:

```console
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser.

## Want to add a model?

1. Check out `lib/models.js` and add your model to the MODELS array.
2. Optionally, generate some example predictions by adding some submissions to `lib/seeds.js`.
3. Push your PR!

## Deploying on Vercel

Alternatively, you can [deploy Zoo on Vercel](./doc/deploy_vercel/README.md).
