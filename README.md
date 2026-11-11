# Vuka × TseboNexus Discovery Brief

Client intake form for leads from the TseboNexus partnership. A lead fills it in, and we use the answers to build a prototype and proposal.

| | |
|---|---|
| Live URL | <https://discovery.tsebo-nexus.co.za> |
| Hosting | GitHub Pages (static HTML, no build step) |
| DNS | GoDaddy (tsebo-nexus.co.za): `CNAME discovery → 0824622148.github.io` |
| Submissions | Web3Forms, sent once per key in `WEB3FORMS_KEYS`: clayton@vukaonline.co.za (main-site key) and thabo.lebina@tsebonexus.co.za (second key) |

Web3Forms is on the free plan: `ccemail` (copying a second address) is Pro-only and makes submissions fail with HTTP 400 if included.

## Sending the link

Add `?ref=Name` to pre-fill the "Who referred you?" field, for example
`https://discovery.tsebo-nexus.co.za/?ref=Thabo`.

## Where the data goes

Each submission arrives as an email titled **"New discovery brief: <business name>"**. It has every answered field plus a plain-text copy of the full brief at the bottom. Reply-to is set to the lead's email address, so you can reply to them directly from the email.

Nothing is stored on this site. The lead's unsent draft is kept only in their own browser, so they can come back to it later, and it's cleared once they send.

## Files

- `index.html`: the whole form (questions are in the `SECTIONS` array near the top of the script)
- `assets/`: Vuka wordmarks (ink and white) and the TseboNexus logo
- `CNAME`: binds the subdomain

## Changing a question

Edit the `SECTIONS` array in `index.html`, check it locally, then commit and push. Pages redeploys in about a minute.
