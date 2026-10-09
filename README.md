# Shishii Translator

Traduction de texte et de parole pour Windows, avec DeepL, ElevenLabs, Whisper local, historique, favoris, VRChat OSC et sous-titres SteamVR.

![Logo Shishii Translator](ui/shishii-logo.png)

## Fonctions

- Traduction simple par défaut, avec mode **trois langues simultanées** activable depuis l’interface.
- DeepL Free ou Pro, avec clés conservées chiffrées par Windows.
- Speech-to-text local avec Whisper Base et raccourci global F8.
- Text-to-speech par ElevenLabs ou les voix installées dans Windows.
- Historique local, favoris et export JSON.
- Sous-titres devant le casque SteamVR et chatbox VRChat par OSC local.
- Interface en français, anglais, espagnol, allemand et japonais.

## Utilisation

1. Téléchargez l’archive de la dernière version depuis la page **Releases**.
2. Extrayez le dossier puis ouvrez `Shishii Translator.exe`.
3. Dans Connexions IA, ajoutez vos clés DeepL et ElevenLabs si vous souhaitez les utiliser.
4. Écrivez une phrase et appuyez sur **Entrée** pour traduire. Utilisez **Maj+Entrée** pour ajouter une ligne.

Le mode local fourni contient les modèles français ↔ anglais. DeepL et ElevenLabs demandent vos propres clés et envoient le texte au service choisi pour effectuer leur tâche.

## Développement

Le projet contient le code de l’application. Les modèles et le runtime portable sont distribués avec les archives de version afin d’éviter d’alourdir le dépôt. Consultez `LISEZ-MOI.md` pour les détails de fonctionnement.

## Licence

Le code de Shishii Translator est sous licence MIT. Le logo Shishii reste réservé à Shiiou. Les composants et modèles tiers conservent leurs propres licences : consultez [LICENSE.md](LICENSE.md) et [licenses/CREDITS.md](licenses/CREDITS.md).
