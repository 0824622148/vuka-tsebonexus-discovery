# Vuka × TseboNexus Discovery Brief

Client intake form for leads from the TseboNexus partnership. A lead fills it in, and we use the answers to build a prototype and proposal.

| | |
|---|---|
| Live URL | <https://tsebo-nexus.vukaonline.co.za> |
| Hosting | GitHub Pages (static HTML, no build step) |
| DNS | Afrihost: `CNAME tsebo-nexus → 0824622148.github.io` |
| Submissions | Web3Forms (same key as vukaonline.co.za), emailed to clayton@vukaonline.co.za, CC thabo.lebina@tsebonexus.co.za |

To change who gets copied, edit `CC_EMAILS` in `index.html` (separate several addresses with `; `). CC is a Web3Forms Pro feature, and each address must be a verified linked email on the account.

## Sending the link

Add `?ref=Name` to pre-fill the "Who referred you?" field, for example
`https://tsebo-nexus.vukaonline.co.za/?ref=Thabo`.

## Where the data goes

Each submission arrives as an email titled **"New discovery brief: <business name>"**. It has every answered field plus a plain-text copy of the full brief at the bottom. Reply-to is set to the lead's email address, so you can reply to them directly from the email.

Nothing is stored on this site. The lead's unsent draft is kept only in their own browser, so they can come back to it later, and it's cleared once they send.

## Files

- `index.html`: the whole form (questions are in the `SECTIONS` array near the top of the script)
- `assets/`: Vuka wordmarks (ink and white) and the TseboNexus logo
- `CNAME`: binds the subdomain

## Changing a question

Edit the `SECTIONS` array in `index.html`, check it locally, then commit and push. Pages redeploys in about a minute.
