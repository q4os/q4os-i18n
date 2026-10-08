# Untested changes (2026-09-29)

The 18 q4os-tools/<lang>/desktop-profiler.po sources are synced from q4os-sw-profiler 4.16.0-a7 (profile description translations, plus the three fix-round-2 strings). This package does not ship desktop-profiler.mo, so nothing it builds changes. The translations are tested with q4os-sw-profiler 4.16.0-a7; delete this file then.

# Untested changes (2026-10-05)

The welcome-screen sources are synced from q4os-welcome 4.4.0-a4: the template and the 18 translated languages gain the "No web browser is installed yet" string. The desktop-profiler template is synced from q4os-sw-profiler 4.16.0-a7. Both templates are merged (msgmerge, as a_q4os/locales_update.sh does) into the remaining 156 languages, which drops three obsolete untranslated welcome-screen strings there. This package ships neither catalog, so nothing it builds changes; all touched .po files pass msgfmt -c. Delete this section once q4os-welcome 4.4.0-a4 is tested.

# Untested changes (2026-10-05, 3.17.6-a1)

The package no longer ships q4os-base.mo, its last catalog: q4os-base 4.31.15-a1 installs it. The package builds empty (transitional). The q4os-base sources are synced from q4os-base 4.31.15-a1 (regenerated template, 18 complete languages, Czech and Hebrew new and machine written; template merged into the other 156 languages). New catalog wificonnect, mirrored from q4os-wificonnect 1.1-a9 (template, 18 languages, 156 skeletons); not shipped from here. Checked: every touched .po passes msgfmt -c, the built deb holds no file outside /usr/share/doc, a simulated upgrade resolves. Not checked: a real upgrade in a VM with a translated session. Delete this section then.

The calamares-debian sources of 18 languages are synced from q4os_live_calamares (six new languages, eight reviewed and no longer fuzzy); see the UNTESTED.md there. Not shipped from here.

q4os-shortcuts: new tool `a_q4os/apply_shortcuts.sh` (the directory is git-ignored, the tool lives in the working tree only). Run on scratch copies of 75 Q4OS desktop files: 54 gain lines, a second run changes nothing, existing lines are kept. Applied for real to q4os-base 4.31.15-a1 only. Not checked in a session: a translated Trinity menu showing the new names.

