# ONIRIQUE F76 (JUCE 8 / VST3, AU)

le compresseur FET de VOCALBOX (BLACK / BLUE) : INPUT, OUTPUT, ATTACK, RELEASE, RATIO 4 / 8 / 12 / 20 / ALL, METER GR / +8 / +4 / OFF, sur une façade à lui dans la DA ONIRIQUE, avec son VU.
En bas : OVERSAMPLING (OFF / 2x / 4x / 8x, latence déclarée), MIX (son direct en phase), réduction de gain.

Même code pour les deux appareils : `set(SOLO_MODEL "1176")` ou `"LA2A"` dans CMakeLists.txt. Le moteur (Source/dsp/Comp1176.h,
CompLA2A.h) est celui de VOCALBOX, sans changement. Banc : `SoloBench` (MIX 0 et BYPASS exacts, calage, compression).
Chaque envoi sur `main` compile Mac et Windows, passe le banc et publie dans ONIRIQUE CENTRAL.
