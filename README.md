# CEO Command Center — standalone project

This is the same CEO Command Center app, packaged as a normal React project
so it can run on real hosting (Vercel, Netlify, etc.) instead of inside the
chat sandbox. Once deployed here, the automatic silent archive/notify calls
(no tap needed) will actually work, because the sandbox restriction that
required one-tap buttons doesn't exist on real hosting.

## Local development (optional, needs Node.js installed)
```
npm install
npm run dev
```

## Deploy to Vercel (recommended, no local setup needed)
See the deployment guide provided in chat — short version:
1. Push this folder to a new GitHub repository.
2. Go to vercel.com → New Project → Import that repository.
3. Vercel auto-detects Vite and deploys. Done — you get a live URL.

## After deploying
Everything works exactly the same as in the chat preview — Integrations
panel, one-tap buttons, AI-generated answers, file exports. The only
difference is that background archive/notify calls no longer need a click;
they'll fire automatically when `Auto-notify CEO on every completed task`
is on, since real hosting doesn't block outbound requests the way the
chat sandbox does.
