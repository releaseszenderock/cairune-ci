# Cairune: privacy policy / Règles de confidentialité

[English](#cairune-extension-privacy-policy) · [Français](#règles-de-confidentialité-de-lextension-cairune)

# Cairune extension privacy policy

Last updated: September 30, 2026. Extension version: 1.0.0.

This policy covers the Cairune browser extension for Chrome, Microsoft Edge and Firefox. It is published by Emmanuel Zenderock, who can be reached at support@zenderock.me.

## In short

- The extension talks only to the Cairune app installed on your computer, at the local address `127.0.0.1`. It sends nothing to the publisher or to any remote server.
- It reads a page only when you ask it to, and sends only what you choose to keep.
- No account, no usage analytics, no advertising, no selling, no remotely loaded code.

## What the extension reads, and when

The extension runs no script in your pages outside your own actions. It reads a page only in these three cases:

1. **"Save page"**: the tab's address and title, and what the page declares about itself (canonical address, description, language, author name or link, preview image address).
2. **"Save selection"**: the text you selected (64 KiB at most), up to 600 characters of the passage on each side, and the page's address, title, canonical address and language.
3. **"Circle to save"** (the Alt+Shift+C shortcut or the "Circle" button): only what lies under your stroke, when you release the mouse. For the item you then choose: its address, title and text (a post's, a passage's or an article's), and for a post, its author's name and handle, its date and the addresses of its videos or photos. If nothing recognizable lies under your stroke, or you choose "Keep as an image", a picture of the circled zone as it is on your screen: the extension captures the visible part of that tab once, with nothing of its own interface in it, and keeps only the zone.

The extension never reads your cookies, passwords, form fields, site storage or the pages' HTML. It keeps no browsing history.

## Where this data goes

Only to the Cairune desktop app on the same computer, over the local address `127.0.0.1` (ports 47381 to 47390), and only after you choose. The app keeps it in your Library, on your computer. To save a video or preserve a page, the app may then download that content from the original site, as you asked it to.

The extension talks only to a Cairune app you paired yourself, with a one-time code the app shows.

## What the extension keeps in the browser

- **The pairing credential** issued by your Cairune app, in the extension's local storage. It is used only to talk to that app, and it is never synced between devices.
- **Your sound settings**, and the app's last "Interface sounds" setting.
- **The state of an ongoing "Circle"**, in the browser's session storage (cleared when the browser closes). If the extension is not paired yet, the chosen item waits there five minutes at most, then it is deleted. The picture of a circled zone stays there only until Cairune has answered, and never waits for pairing.

## What the extension does not do

- It sends nothing to the publisher or to any third party.
- It uses no usage analytics, advertising or trackers.
- It sells and shares no data.
- It uses your data for nothing but saving what you chose into Cairune.
- It loads no remote code.

## Permissions

- `activeTab`: access the tab where you just clicked the extension or pressed its shortcut, and that tab only.
- `scripting`: read there what you want to save, or show the "Circle" interface there.
- `storage`: keep the pairing credential, your settings and the state of an ongoing "Circle".
- `http://127.0.0.1/*`: talk to the Cairune app on your computer, and to nothing else.

## Deleting your data

- "Disconnect this browser", in the extension or in Cairune's settings, deletes the pairing credential.
- Uninstalling the extension deletes everything it keeps in the browser.
- What you saved is in your Cairune Library, on your computer: you delete it from the app.

## Changes

If this policy changes, the new version is published at this address, https://github.com/releaseszenderock/cairune-ci/blob/main/PRIVACY.md, with its date.

## Contact

support@zenderock.me

---

# Règles de confidentialité de l'extension Cairune

Dernière mise à jour : 30 septembre 2026. Version de l'extension : 1.0.0.

Ces règles concernent l'extension de navigateur Cairune pour Chrome, Microsoft Edge et Firefox. Elle est éditée par Emmanuel Zenderock, que vous pouvez joindre à support@zenderock.me.

## En bref

- L'extension ne parle qu'à l'application Cairune installée sur votre ordinateur, à l'adresse locale `127.0.0.1`. Elle n'envoie rien à l'éditeur, ni à aucun serveur distant.
- Elle ne lit une page que lorsque vous le lui demandez, et n'envoie que ce que vous choisissez de garder.
- Pas de compte, pas de statistiques d'usage, pas de publicité, pas de revente, pas de code chargé à distance.

## Ce que l'extension lit, et quand

L'extension ne fait tourner aucun script dans vos pages en dehors de vos actions. Elle lit une page seulement dans ces trois cas :

1. **« Enregistrer la page »** : l'adresse et le titre de l'onglet, et ce que la page déclare d'elle-même (adresse canonique, description, langue, nom ou lien de l'auteur, adresse de l'image d'aperçu).
2. **« Enregistrer la sélection »** : le texte que vous avez sélectionné (64 Kio au plus), jusqu'à 600 caractères du passage de chaque côté, et l'adresse, le titre, l'adresse canonique et la langue de la page.
3. **« Entourer pour enregistrer »** (le raccourci Alt+Maj+C ou le bouton « Entourer ») : seulement ce qui se trouve sous votre trait, quand vous relâchez la souris. Pour l'élément que vous choisissez ensuite : son adresse, son titre, son texte (celui d'un post, d'un passage ou d'un article), et pour un post, le nom et l'identifiant de son auteur, sa date et l'adresse de ses vidéos ou photos. Si rien de reconnaissable ne se trouve sous votre trait, ou si vous choisissez « Garder comme image », une image de la zone entourée telle qu'elle est à l'écran : l'extension capture une fois la partie visible de cet onglet, sans rien de sa propre interface, et n'en garde que la zone.

L'extension ne lit jamais vos cookies, vos mots de passe, les champs de formulaire, le stockage des sites ni le code HTML des pages. Elle ne tient aucun historique de navigation.

## Où vont ces données

Uniquement vers l'application de bureau Cairune, sur le même ordinateur, par l'adresse locale `127.0.0.1` (ports 47381 à 47390), et seulement après votre choix. L'application les garde dans votre Bibliothèque, sur votre ordinateur. Pour enregistrer une vidéo ou conserver une page, l'application peut ensuite télécharger ce contenu depuis le site d'origine, comme vous le lui avez demandé.

L'extension ne communique qu'avec une application Cairune que vous avez associée vous-même, avec un code à usage unique affiché par l'application.

## Ce que l'extension garde dans le navigateur

- **L'identifiant d'association** remis par votre application Cairune, dans le stockage local de l'extension. Il ne sert qu'à parler à cette application. Il n'est jamais synchronisé entre appareils.
- **Vos réglages de sons**, et le dernier réglage « Sons de l'interface » de l'application.
- **L'état d'un « Entourer » en cours**, dans le stockage de session du navigateur (effacé à sa fermeture). Si l'extension n'est pas encore associée, l'élément choisi y attend cinq minutes au plus, puis il est effacé. L'image d'une zone entourée n'y reste que jusqu'à la réponse de Cairune, et n'attend jamais l'association.

## Ce que l'extension ne fait pas

- Elle n'envoie rien à l'éditeur ni à un tiers.
- Elle n'utilise ni statistiques d'usage, ni publicité, ni pisteur.
- Elle ne vend ni ne partage aucune donnée.
- Elle n'utilise pas vos données à d'autres fins que d'enregistrer ce que vous avez choisi dans Cairune.
- Elle ne charge aucun code à distance.

## Permissions

- `activeTab` : accéder à l'onglet où vous venez de cliquer sur l'extension ou d'appuyer sur son raccourci, et à lui seul.
- `scripting` : y lire ce que vous voulez enregistrer, ou y afficher l'interface « Entourer ».
- `storage` : garder l'identifiant d'association, vos réglages et l'état d'un « Entourer » en cours.
- `http://127.0.0.1/*` : parler à l'application Cairune de votre ordinateur, et à rien d'autre.

## Effacer vos données

- « Déconnecter ce navigateur », dans l'extension ou dans les réglages de Cairune, efface l'identifiant d'association.
- Désinstaller l'extension efface tout ce qu'elle garde dans le navigateur.
- Ce que vous avez enregistré se trouve dans votre Bibliothèque Cairune, sur votre ordinateur : vous le supprimez depuis l'application.

## Modifications

Si ces règles changent, la nouvelle version est publiée à cette adresse, https://github.com/releaseszenderock/cairune-ci/blob/main/PRIVACY.md, avec sa date.

## Contact

support@zenderock.me
