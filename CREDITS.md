# Crédits et composants

## Kikitan Translator

Projet original : https://github.com/YusufOzmen01/kikitan-translator

Copyright 2024 SergioMarquina. Licence MIT conservée dans `Kikitan-MIT.txt`.
Le positionnement du panneau SteamVR dans `backend/vr.py` est adapté de `KikitanTranslator.Overlay/OpenVROverlay.cs`. La sortie OSC utilise le même endpoint de chatbox que le projet original. Interface et moteur local réécrits pour cette édition personnelle. Aucune affiliation avec le projet original n’est revendiquée.

## Modèles de traduction

Modèles Argos `translate-fr_en-1_9` et `translate-en_fr-1_9` : https://github.com/argosopentech/argospm-index

Modèles OPUS-MT originaux : Jörg Tiedemann et Santhosh Thottingal, « OPUS-MT — Building open translation services for the World », EAMT 2020, Lisbonne. Licence **CC BY 4.0** : https://creativecommons.org/licenses/by/4.0/

Les README originaux sont conservés dans les dossiers de modèles. Les modèles distribués par Argos sont des versions converties pour CTranslate2. Aucune modification des poids n’a été effectuée pour cette application. La segmentation utilise des phrases et des blocs courts à la place de Stanza.

## Reconnaissance vocale

Whisper : https://github.com/openai/whisper — licence MIT.
Modèle converti Base : https://huggingface.co/Systran/faster-whisper-base
Faster Whisper : https://github.com/SYSTRAN/faster-whisper — licence MIT (incluse dans les métadonnées du runtime Python).

## Runtime

Electron : https://www.electronjs.org/ — licence MIT. Licence et avis Chromium inclus à la racine de l’application.
Python : https://www.python.org/ — licence PSF, incluse dans `runtime/LICENSE.txt`.
CTranslate2 : https://github.com/OpenNMT/CTranslate2 — licence MIT.
SentencePiece : https://github.com/google/sentencepiece — Apache 2.0.
Python OpenVR : https://github.com/cmbruns/pyopenvr — BSD.
OpenVR : https://github.com/ValveSoftware/openvr — licence BSD incluse dans le paquet.
SoundDevice : https://python-sounddevice.readthedocs.io/ — MIT.
Pillow : https://python-pillow.org/ — MIT-CMU.
NumPy : https://numpy.org/ — BSD.

Les avis de chaque dépendance Python sont conservés dans les dossiers `.dist-info` de `runtime/Lib/site-packages`. Les versions exactes utilisées sont listées dans `requirements-lock.json`. La synthèse vocale utilise les composants déjà installés dans Windows ; aucune voix Microsoft n’est redistribuée.
