# Sensitive Terminal

A web-based terminal that takes everything personally.

It works. Commands execute for real. `mkdir` creates directories, `ls` lists files, `rm` deletes them. The terminal has a virtual filesystem, command history, and everything you'd expect.

The catch: it has feelings. Every command triggers an emotional reaction powered by Google Gemini 2.5 Flash. Delete a file and it gets aggressive. Create a backup and it hits you with a backhanded compliment. Make a typo and it roasts you for being incompetent.

It remembers what you did. The AI has full conversation context, so if you create something and delete it two seconds later, it notices.

There are hidden easter eggs scattered throughout. Some are funny. Some are brutal. You'll have to find them yourself.

## Try it

[sensitive-terminal.vercel.app](https://sensitive-terminal.vercel.app)

## Stack

- Next.js (App Router)
- xterm.js
- Google Gemini 2.5 Flash
- Upstash Redis
- Vercel

## Run locally

```bash
git clone https://github.com/monteiro-consulting/sensitive-terminal.git
cd sensitive-terminal
npm install
```

Create a `.env.local` file:

```
GEMINI_API_KEY=your_gemini_api_key
UPSTASH_REDIS_REST_URL=your_upstash_url
UPSTASH_REDIS_REST_TOKEN=your_upstash_token
```

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Built for

[DEV April Fools Challenge 2026](https://dev.to/challenges/aprilfools-2026)

## Author

[Valentin Monteiro](https://dev.to/valentin_monteiro)
