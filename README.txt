RC Monitoring App — install package
====================================

Upload index.html to its own folder/repo on GitHub Pages. This file is
self-contained — it generates its own icon and manifest at runtime, so
no extra files are needed alongside it.

IMPORTANT — this file was just fixed to connect to the same backend
as the MBR2 Dashboard. It previously pointed at a separate Firebase
project while the dashboard had migrated to Supabase, so the two apps
were silently NOT sharing data. That's fixed now: this file's
`supabaseConfig` block near the top matches the dashboard's exactly.
Do not change one without updating the other to match — that's what
keeps the two apps' data connected.

Install on phone/computer: open the link, then use your browser's
Install / Add to Home Screen option.
