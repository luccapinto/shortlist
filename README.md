# Shortlist — waitlist landing

Landing page and waitlist for **Shortlist**, an AI recruiter that works inside your team chat (Teams, Slack, Google Chat): it ranks résumés, runs WhatsApp phone screens, conducts live voice interviews and returns a shortlist where every score cites the candidate's own words.

Live: https://shortlist.luccabuilds.com

## Stack
- Static HTML/CSS/JS, no build step, deployed on Vercel.
- Waitlist stored in Supabase through `SECURITY DEFINER` RPCs (`shortlist_join`, `shortlist_enrich`, `shortlist_count`); the table itself is not readable or writable by the anon role.
- UTM parameters are captured per signup so each acquisition channel can be measured.
- Vercel Web Analytics (cookieless) for page views and CTA events.

## Local preview
```bash
python3 -m http.server 8777
```
