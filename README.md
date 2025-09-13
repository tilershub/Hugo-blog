# FXFORECAST — Hugo Production Starter (AdSense + GA)

A production-grade Hugo starter with **Google AdSense**, **Google Analytics 4 (gtag)**, consent banner, and Netlify config.

## Quick Start
1. Install Hugo (extended): https://gohugo.io/getting-started/installing/
2. Set your IDs in `config.toml`:
   - `params.ga_measurement_id = "G-XXXXXXX"`
   - `params.adsense_client_id  = "ca-pub-XXXXXXXX"`
3. Dev:
   ```bash
   hugo server -D
   ```
4. Build:
   ```bash
   hugo
   ```

## Netlify
- **Build command:** `hugo`
- **Publish directory:** `public`
- Optional environment: `HUGO_VERSION`

## Ad Units
Use `{{ partial "adsense/unit.html" (dict "slot" "1234567890") }}` where you want an ad. For responsive in-article demo, leave `slot` empty and set `params.show_demo_ads = true` during testing.

## Consent
Basic GDPR-style consent banner is included. It defers ad/analytics until accepted.
