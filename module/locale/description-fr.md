# Ally Support

**Auteur** : Monsterfish
**Version** : 1.0.19

Les alliés IA s'entraident entre eux comme ils vous aident déjà. Chaque volet peut être désactivé dans les paramètres.

## Ressources

Lorsqu'un seigneur IA manque d'une ressource qu'il ne peut pas acheter, il la demande à ses alliés. Normalement, vous êtes le seul à répondre. Désormais ses alliés IA répondent aussi — mais seulement s'ils conservent leur propre minimum après l'envoi (le « minimum de ressources conservé après échange » de leur personnage IA), selon la même règle que pour vos demandes. Dès qu'un allié a livré, les autres n'envoient rien. Un allié qui ne peut rien céder refuse immédiatement.

Après une demande satisfaite, le demandeur attend son « délai de requête IA » avant de redemander — compté en semaines de jeu, exactement comme après vos propres envois. Après un refus, il attend un mois.

Les seigneurs IA ne demandent que ce dont ils ont besoin sans pouvoir l'acheter, donc cela n'arrive pas sans cesse. Les envois apparaissent dans les statistiques de ressources envoyées/reçues en fin de partie.

Si l'allié demandeur est affaibli et que le donneur ne peut pas fournir toute la quantité, il envoie tout de même jusqu'à la moitié, en descendant au besoin jusqu'à la moitié de son propre minimum.

## Un partage réellement utile

Chacune de ces règles dispose d'un réglage, tous activés par défaut :

- **Pas de renvoi en boucle.** Une demande satisfaite est rayée de la liste d'achats du demandeur, un seigneur ne donne jamais ce qu'il cherche lui-même, et les ressources reçues d'un allié ne sont pas retransmises pendant 3 mois. (Auparavant, deux alliés pouvaient se renvoyer la même pierre chaque seconde.)
- **Uniquement ce qui aide.** Un allié envoie la quantité réellement souhaitée et jamais plus que le demandeur ne peut stocker (le surplus serait vendu à perte). Les armes et la nourriture passent en premier ; le bois, la pierre et les autres matériaux de construction uniquement tant que le demandeur n'est pas menacé.
- **Seuls les alliés mieux lotis donnent.** Un seigneur menacé ou affaibli ne donne rien, et seul un allié mieux portant que le demandeur aide — le plus aisé est sollicité en premier. Chaque seigneur donne au plus 30 % de chaque ressource, or compris, par mois.
- **Aide à la reconstruction.** Un seigneur ayant perdu son camp de mercenaires, sa caserne, son armurerie, son grenier ou son marché reçoit du bois et de la pierre en priorité jusqu'à le reconstruire — même s'il est menacé, car sans ces bâtiments il ne peut pas se défendre.
- **Or pour le recrutement.** Un seigneur affaibli ou menacé qui ne peut pas recruter reçoit l'or nécessaire d'un allié mieux loti (l'or de recrutement de son personnage IA plus 300).

## Or

Un allié IA riche à qui l'on demande des ressources envoie aussi de l'or. Chaque seigneur conserve 1000 or pour son propre recrutement (réglable) et ne partage que le surplus. Il envoie un quart de cet excédent, et uniquement à un allié plus pauvre que lui.

## Demandes d'or

Lorsqu'un seigneur IA veut des ressources qu'il ne peut pas payer, il demande désormais à ses alliés — vous et les IA — l'or qui lui manque (pas plus souvent que son délai de requête IA ne le permet). Vous voyez la demande sur votre écran des alliés comme toute autre requête. Un allié IA envoie l'or s'il conserve ses 1000 or après l'envoi ; à un allié affaibli, il envoie jusqu'à la moitié, en descendant au besoin jusqu'à la moitié de ce seuil.

## Troupes

- **Les alliés IA s'entraident.** Lorsque des ennemis s'approchent d'un seigneur IA, ses alliés IA envoient leurs troupes, comme quand vous appelez à l'aide. Un allié ne vient que s'il n'est pas lui-même menacé, n'attaque pas déjà et dispose de la taille d'armée requise par son personnage IA. Son armée d'attaque reste au moins 6 mois de jeu, et plus longtemps tant que le château est en danger. Elle rentre aussitôt si l'allié se sent de nouveau fort — ou, si vous choisissez cette option dans les paramètres, dès que la propre armée de l'aidant est prête à attaquer, pour ne pas retarder son assaut. Les troupes rentrent ensuite et le seigneur attend 3 mois (ou sa propre attaque) avant d'aider de nouveau.
- **75 % de l'armée d'attaque part en renfort.** Lorsqu'un allié IA aide — vous ou une autre IA — il envoie 75 % de son armée d'attaque et garde le reste dans son camp. Les défenseurs, patrouilles et pillards restent toujours ; les ingénieurs, écheliers, tunneliers et engins de siège restent en priorité. Une fois l'aide finie, tout le monde rejoint l'armée.
- **La porte s'ouvre aux renforts.** Quand les troupes de renfort attendent devant une porte du château aidé, celle-ci s'ouvre pour les laisser entrer. Dès que plus personne n'attend, elle se referme d'elle-même comme d'habitude (si des ennemis approchent). À la fin de l'aide, elle se rouvre de la même façon pour les laisser sortir. Cela marche aussi pour vos portes.
- **Les renforts montent sur le donjon.** Une fois à l'intérieur, les renforts se placent sur le donjon du seigneur aidé — l'ordre qu'une IA donne à ses propres archers quand elle s'inquiète — pour que les archers et arbalétriers puissent tirer d'en haut. Ceux qui n'ont pas de place en haut se postent autour du donjon.

Seuls les alliés (même équipe) reçoivent ressources, or ou troupes.

## Bon à savoir

- Les demandes que vous envoyez et recevez fonctionnent exactement comme avant.
- Pas encore testé en jeu.
