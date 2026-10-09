# Shishii Translator

Application personnelle inspirée de Kikitan Translator, avec une interface moderne rouge, noire et blanche. Elle traduit une phrase vers une langue par défaut ; activez manuellement l’option de traduction simultanée pour l’envoyer vers trois langues, reconnaît la parole et peut lire les résultats.

## Démarrage

1. Extrayez entièrement le dossier **Shishii Translator** dans Documents ou un dossier où vous pouvez écrire.
2. Lancez **Shishii Translator.exe**.
3. Ouvrez **Connexions IA** et renseignez vos clés DeepL et ElevenLabs.
4. Choisissez la langue parlée et la langue de sortie, puis parlez avec le microphone ou écrivez un message. Activez **Traductions simultanées** si vous souhaitez utiliser les trois sorties.
5. Dans la zone de texte, appuyez sur **Entrée** pour traduire. Utilisez **Maj+Entrée** pour insérer une nouvelle ligne.

## DeepL

DeepL est utilisé pour la traduction en ligne. Ajoutez votre clé dans **Connexions IA**, puis choisissez Free ou Pro selon votre abonnement. Chaque texte envoyé par traduction DeepL est transmis à DeepL selon les conditions de votre compte.

Vous pouvez choisir le moteur Local dans Connexions. Il fonctionne sans clé, mais seulement pour les directions de langues dont le modèle est installé. L’édition livrée contient français ↔ anglais.

## ElevenLabs et voix

Activez **Text-to-speech** sur l’écran Traduire, puis, dans Connexions IA, collez la clé ElevenLabs, indiquez l’identifiant de la voix et choisissez ElevenLabs pour la synthèse vocale.

Shishii utilise le modèle eleven_multilingual_v2. Le texte lu est transmis à ElevenLabs, qui retourne un MP3 joué dans l’application. Sans clé ElevenLabs, choisissez Windows : les voix installées sur le PC sont alors utilisées sans service en ligne.

## Speech-to-text

Whisper Base est inclus et fonctionne localement. Appuyez sur F8 une première fois pour commencer, puis une seconde fois pour arrêter et lancer la ou les traductions actives. Le son du microphone n’est pas conservé.

## VRChat et SteamVR

- Activez **Chatbox VRChat** pour envoyer la première traduction sur le port OSC local 9000. Activez OSC dans VRChat : Actions → Options → OSC → Enabled.
- Activez **Sous-titres SteamVR** pour afficher la première traduction devant le casque. Ouvrez SteamVR et utilisez le bouton de test dans Réglages.

L’envoi vers VRChat n’a pas d’accusé de réception : l’application confirme l’envoi UDP local, pas l’affichage dans le jeu.

## Données et sécurité

Les clés DeepL et ElevenLabs sont conservées dans `data/providers.bin`, chiffré avec le mécanisme de protection Windows de la session. Elles ne sont jamais affichées dans l’interface ni écrites dans l’historique ou le journal.

`data/shishii.sqlite3` contient les réglages, l’historique et les favoris. L’historique n’est pas chiffré. Les traductions issues de DeepL ou les phrases lues par ElevenLabs sont des données envoyées aux services choisis. Le moteur local ne leur envoie rien.

## Interface

La langue de l’interface peut être changée dans la liste en haut à droite. Français, anglais, espagnol, allemand et japonais sont inclus pour les principales commandes de l’application.

## Crédits

Le logo fourni par le propriétaire est intégré comme `ui/shishii-logo.png`.

Crédits, licences et attribution de Kikitan Translator, Whisper, Argos/OPUS-MT, Electron, OpenVR et des dépendances sont dans `licenses/CREDITS.md`.

Les droits d’utilisation de Shishii Translator sont définis dans `LICENSE.md`. Le code est sous licence MIT ; le logo Shishii demeure réservé à son propriétaire.
