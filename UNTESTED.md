# Untested changes (2026-09-29)

The 18 q4os-tools/<lang>/desktop-profiler.po sources are synced from q4os-sw-profiler 4.16.0-a7 (profile description translations, plus the three fix-round-2 strings). This package does not ship desktop-profiler.mo, so nothing it builds changes. The translations are tested with q4os-sw-profiler 4.16.0-a7; delete this file then.

# Untested changes (2026-10-05)

The welcome-screen sources are synced from q4os-welcome 4.4.0-a4: the template and the 18 translated languages gain the "No web browser is installed yet" string. The desktop-profiler template is synced from q4os-sw-profiler 4.16.0-a7. Both templates are merged (msgmerge, as a_q4os/locales_update.sh does) into the remaining 156 languages, which drops three obsolete untranslated welcome-screen strings there. This package ships neither catalog, so nothing it builds changes; all touched .po files pass msgfmt -c. Delete this section once q4os-welcome 4.4.0-a4 is tested.
