# Hosting the platform

**Recommendation: buy `supportshaurya.in`, host on GitHub Pages, from a separate public
repo.** Total cost under **₹1,500 a year**. Vercel adds nothing for this.

---

## The domain is not the optional part

The instinct is to start free and add a domain later if it works. For this campaign that is
backwards.

The site's entire job is to be **the trustworthy place** — one combined total, one set of
facts, both campaign links, the documents. It will be printed on flyers, read out, pasted
into WhatsApp forwards by strangers, and sent to CSR heads and a Chief Minister's office.

`supportshaurya.in` reads as a campaign.
`curioler.github.io/support-shaurya` reads as someone's side project.
`support-shaurya-xk3f.vercel.app` reads as a phishing link.

For a family asking the public for ₹26 crore, where the only asset is trust, that difference
converts. The domain is roughly **₹1,000 a year** — less than the cost of reprinting the
flyers once. It is the cheapest credibility available.

And there is a lesson three days old: **the campaign lost WhatsApp overnight because that
channel belonged to someone else.** A domain the family controls cannot be taken away, and
the site behind it can move hosts without a single flyer becoming wrong.

## Hosting: GitHub Pages

| | GitHub Pages | Vercel (Hobby) |
|---|---|---|
| Cost | Free | Free |
| Custom domain + HTTPS | Free | Free |
| Content already there | **Yes — the repo and the markdown exist** | Would need setting up |
| Renders markdown natively | Yes | Needs a framework |
| Serverless functions, SSR | No | Yes |
| Build-minute / bandwidth ceilings | Effectively none at this scale | Hobby-tier limits |
| Commercial-use ambiguity | Static charity site — fine | Hobby tier is for non-commercial use; a donation page sits closer to that line |

**Vercel's advantages are all things this site does not need.** Server-side rendering,
serverless functions, edge middleware — none of that applies to a page showing a total and
some links. Pick it later if the platform ever grows a backend. Today it is extra moving
parts and one more account that can be suspended.

GitHub Pages wins mainly because **the content is already in a GitHub repo in markdown**.
Turning it on is a settings toggle.

## One thing to get right: split the repos

`Curioler/support-shaurya` is **public and contains Shaurya's medical records** — the
MedGenome genetic report, prescriptions, the CPK report. Right now those are public but
obscure: nothing links to them and search engines have no reason to crawl them.

**Publishing a Pages site from that repo would change that.** A live site invites crawlers,
and a public repo behind a linked domain can surface the PDFs in search results for years.
The family agreed to a public repo; they did not agree to a searchable medical file.

So:

- **`support-shaurya`** (this repo) — working documents, sources, analysis. Keep as is, or
  make private. **Do not enable Pages on it.**
- **`supportshaurya-site`** (new) — only what is meant to be public: the combined total,
  the story, both campaign links, contact, and whichever documents the family explicitly
  clears. Pages enabled, domain pointed here.

That also keeps the two jobs separate. The working repo is allowed to be messy and blunt.
The public site is not.

## Costs, honestly

Indian registrars vary and run first-year promotions, so treat these as ranges to check, not
quotes:

| Item | First year | Renewal |
|---|---|---|
| `.in` domain | ~₹500–900 | ~₹800–1,200/yr |
| `.org` domain | ~₹1,000–1,600 | ~₹1,000–1,600/yr |
| GitHub Pages hosting | ₹0 | ₹0 |
| HTTPS certificate | ₹0 (automatic) | ₹0 |

**`.in` or `.org`?** `.in` is cheaper and reads as local, which suits Indian donors, CSR
teams and government correspondence — the audiences that matter most. `.org` reads as
charitable and travels better internationally, which matters if Prakriti opens a diaspora
channel. If the budget stretches, register both and redirect one to the other; the second is
another ₹1,000 or so.

**Buy 2–3 years upfront and turn on auto-renew.** A lapsed domain does not just take the
site down — it makes every printed flyer and QR poster point at nothing, and expired
fundraising domains get bought by opportunists. This campaign may run for years.

**Register it in a name that will still be around**, with contact details someone monitors.
If Bhavin registers it, agree in writing that it belongs to the family, and make sure Gaurang
has the login. Do not let the domain become a single point of failure the way the WhatsApp
number did.

## What to build first

Resist building a platform. Build **one page**:

- The combined total across ImpactGuru and Ketto, with the date it was last updated
- Both donate links, side by side, clearly labelled as the same campaign
- Shaurya's story in the Ketto wording — accurate, no "cure"
- Dr Mathew's attributed line about the therapy working better if given earlier
- A working contact
- A short, honest "where the money goes"

Updating the total is a one-line edit, a commit, and it redeploys itself. No backend, no
database, no automation until the manual version has proved it gets used.

Everything else — document library, contact log, trial tracker — can follow once that page
exists and is being shared.
