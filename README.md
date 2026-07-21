# danielhorne.com

Daniel Horne's personal site. One page, static HTML, no build system, no
dependencies, and no analytics. `index.html` is the whole site.

Two typefaces ship with the repo in `fonts/`: Instrument Serif (display) and
Inter (body), both under the SIL Open Font License. They are SELF-HOSTED on
purpose. Do not swap them for a Google Fonts or other CDN link: the point is
that loading the page makes no third-party request, so no one else learns that
a visitor was here. That property is asserted in the Whole Yield privacy
policy, so breaking it here would make that document false.

## Its look is deliberately NOT the Whole Yield look

This site and `Whole-Yield/wholeyield-site` are meant to diverge. Daniel asked
for that explicitly on 2026-07-21: "both, not matching each other."

This page is art-directed editorial, built to the register of locomotive.ca,
theoutline.com and palmer-dinnerware.com: a large Instrument Serif display face
at weight 400, a persimmon accent, uppercase mono labels, hairline rules, no
cards and no shadows. Whole Yield is the opposite register, modern product
marketing in Inter with pill buttons and rounded cards.

An earlier version of this file said "same visual system as wholeyield-site".
That is now wrong, and it was actively harmful: an agent read that line, treated
the shared style as evidence of Daniel's taste, and proposed a restyle that
preserved a look he did not actually want. If these two sites ever converge
again, it should be because he asked, not because a README said they matched.

## How it publishes

GitHub Pages serves `main` / root. Pushing republishes. `CNAME` holds the apex
domain and must stay at the repo root.

The repo is **public** because a Pages site published from a private repo needs a
GitHub login to view.

## Link discipline

Every outbound link on this page was verified to resolve before it shipped. If
you add one, check it first. Notes on the ones that are deliberately absent:

- **No GitHub link.** github.com/danielahorne is a real account but shows **0
  public repositories** and no bio, because everything lives private under the
  Whole-Yield org. Linking it from a credibility page argues against the page.
- **No Manna link.** Manna has no public URL. It is served tailnet-only over
  Tailscale, so a link would be dead for everyone and would publish a private
  tailnet hostname. The card says "In private beta" instead.
- **No Lucentcast link.** Its marketing site is built but not published yet
  (Pages is not enabled on `Whole-Yield/postprod-service`, pending the live
  Stripe link swap). Card says "Launching soon."
- **No writing link.** No public writing was found. Do not invent one.
- **LinkedIn** returns HTTP 999 to command-line clients. That is LinkedIn's
  anti-bot wall, not a broken link.
- **wholeyield.com** will 404 until its own DNS is pointed. Expected.

## Copy rules

- **Do not name the day-job employer.** It is described as "a large enterprise
  software company" on purpose. Daniel's call, 2026-07-16. Do not "helpfully"
  restore the name. Naming the pre-acquisition company instead leaks the same
  fact, since the acquisition is public, so that is not a workaround either.
  This README is itself published, so do not write the name here to explain the
  rule.
- **The AWS certs are EXPIRED** (earned Feb 2023, Associate certs run 3 years,
  lapsed 2026). The year column reads "Expired 2026", NOT a range. Daniel chose
  this over "2023 to 2026" on 2026-07-21: every other row uses that column for a
  span during which the thing was true, so a range scans as "held through 2026"
  to anyone who reads the year and moves on, and it is currently 2026. The date
  itself has to carry the truth, because the body text only rescues a reader who
  does not skim. Never present them as current, and never restore a range here.

- **Do not name a legal entity for Whole Yield.** None is filed. See the
  `wholeyield-site` README for the full reasoning.
- **Perfume(D)ecay is that show's real styling** (its own title tag, Apple, and
  og:site_name all agree). It is co-hosted by three equal partners, so the page
  scopes Daniel to production and audio.
- No em dashes, per Daniel's standing rule.
- The prior land business is described without naming the entity or the reasons
  it wound down. That story is Daniel's to tell, not the page's to assume.
