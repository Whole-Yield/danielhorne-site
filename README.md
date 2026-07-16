# danielhorne.com

Daniel Horne's personal site. One page, static HTML, no build system, no
dependencies, no analytics, no web fonts. `index.html` is the whole site.

Same visual system as `Whole-Yield/wholeyield-site` (warm cream, Iowan Old Style
serif headings, light and dark via `prefers-color-scheme`).

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

- **Do not name a legal entity for Whole Yield.** None is filed. See the
  `wholeyield-site` README for the full reasoning.
- **Perfume(D)ecay is that show's real styling** (its own title tag, Apple, and
  og:site_name all agree). It is co-hosted by three equal partners, so the page
  scopes Daniel to production and audio.
- No em dashes, per Daniel's standing rule.
- The prior land business is described without naming the entity or the reasons
  it wound down. That story is Daniel's to tell, not the page's to assume.
