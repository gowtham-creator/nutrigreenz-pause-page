# Nutri Greenz — pause page

Shown on nutrigreenz.farm while the store is paused. The real store lives in
`Nutrigreenz-project` and is untouched.

Every path is answered by `middleware.js` with this page as **HTTP 503 +
Retry-After**, so search engines read the pause as temporary. `vercel.json`
rewrites every path to `index.html` as a fallback.

**To resume the store:** move the `nutrigreenz.farm` and `www` domains back to the
main Nutri Greenz Vercel project, then resume that project. Remove the domains from
this project first. Don't delete them at the account level.
