# MechaACraft

Bienvenue sur le projet **MechaACraft**, un framework Minecraft modulaire dédié à l’automatisation, aux circuits logiques, aux systèmes énergétiques et à l’informatique appliquée.

## Sommaire

- [`Explication`](#explication)
- [`Structure du projet`](#structure-du-projet)
- [`Mods`](#mods)
- [`Contribuer`](#contribuer)

## Explication

Nous sommes deux passionnés d'informatique, d'électronique, de systèmes logiques et de tout ce qui touche à l’ingénierie technique. L’idée de base de MechaACraft part d’un constat simple : les modpacks existants sont souvent soit surchargés de contenus inutiles (trop de mods), soit trop peu documentés pour être réellement compréhensibles et exploitables.

Ici, on a choisi de faire les choses **progressivement**, de manière **claire, cohérente et documentée**. Pas d'excès : chaque ajout est réfléchi pour maximiser la **compatibilité**, la **lisibilité** et l'**expérience technique**. L’approche est minimaliste et modulaire, à la manière d’une distribution personnalisable (**S/o Arch Linux 😉**).

Ce projet peut ressembler à un modpack dans sa forme initiale, mais dans le fond, l’ambition est toute autre. Il ne s’agit pas simplement de regrouper des mods : il s’agit de construire un **cadre structuré**, un **espace d’expérimentation** libre, évolutif et entièrement personnalisable.

> Développé par deux amis, ce projet n’a aucune garantie de maintenance régulière. Il évolue selon notre temps, notre motivation et nos envies. À la base, MechaACraft a été conçu pour nous deux, sans vocation publique. Mais on s’est dit que cela pourrait intéresser d’autres passionnés, alors autant le partager. Et si certains veulent contribuer, proposer des idées ou même s’impliquer, ce sera avec plaisir.

## Structure du projet

> Remarque : les dépôts `Client` et `Installer` sont encore en cours de développement.

| Dépôt | Description |
|-------|-------------|
| [`MechaACraft`](https://github.com/MechaACraft/MechaACraft) | Contient la documentation générale du projet MechaACraft, ainsi que la configuration logique et organisationnelle des modules associés.  |
| [`MechaACraft-Server`](https://github.com/MechaACraft/MechaACraft-Server) | Contient les fichiers de configuration, le script de démarrage et les paramètres système nécessaires à l’exécution reproductible du serveur. |
| [`MechaACraft-Client`](https://github.com/MechaACraft/MechaACraft-Client) | Contient le client officiel de MechaACraft, conçu pour être utilisé en conjonction avec le serveur du projet. |
| [`MechaACraft-Installer`](https://github.com/MechaACraft/MechaACraft-Installer) | Contient l’installeur officiel du projet, permettant l’installation des fichiers client et serveur à partir des dépôts sources. |

## Mods

### Ce tableau présente la liste exhaustive des mods utilisés dans MechaACraft, leur rôle dans l’écosystème du projet, et leur emplacement d’exécution (client, serveur ou partagé).

| Mod | Description | Client / Serveur |
|-----|-------------|------------------|
| SecurityCraft | Fournit un système de sécurité avancé : claviers numériques, scanners rétiniens, mines, caméras, portes renforcées. Permet de restreindre l'accès, d’automatiser la défense et de protéger les zones sensibles dans un contexte technique et multi-joueur. | Partagé |
| Electrodynamics | Base électrique modulaire : machines industrielles, générateurs haute tension, transformateurs, systèmes de câblage réalistes. Sert de socle pour une infrastructure énergétique avancée et interconnectée. | Partagé |
| Framework | Bibliothèque technique nécessaire au fonctionnement de mods comme Electrodynamics et Ballistix. Ne contient aucun contenu en jeu, mais assure la compatibilité des systèmes. | Partagé |
| Cloth Config API | Librairie d’interface graphique utilisée par de nombreux mods pour créer des menus de configuration ergonomiques directement en jeu. | Partagé |
| Ballistix | Ajoute des missiles, radars, silos de lancement et systèmes de ciblage. S’intègre aux infrastructures industrielles et énergétiques pour la gestion de la balistique. | Partagé |
| Ultimate Car | Implémente un système de véhicules fonctionnels avec carburant, moteur, routes, stations-service et mécanique de conduite réaliste. | Partagé |
| MrCrayfish's Gun **(Unofficial)** | Ajoute des armes à feu modulaires (pistolets, fusils, etc.) avec système de munitions, viseur, rechargement et compatibilité avec des accessoires. | Partagé |
| BetterF3 | Remplace l’écran de débogage (F3) par une interface personnalisable, plus lisible et segmentée : FPS, mémoire, position, chunk, entités, etc. | Client |
| Shulker Box Tooltip | Affiche le contenu des shulker boxes et conteneurs similaires directement dans l’info-bulle de l’inventaire, sans avoir à les poser. | Partagé |
| The One Probe | Affiche des informations contextuelles sur les blocs et entités : énergie stockée, redstone, inventaire interne, nom du bloc, etc | Partagé |
| Konkrete | Librairie utilitaire requise par certains mods. Fournit des extensions de base pour l’interface, les événements ou le rendu. | Partagé |
| RPG-Hud | Transforme l’interface en HUD de type RPG : barre de vie stylisée, équipements visibles, horloge, boussole, faim, etc. | Client |
| Just Zoom | Ajoute une fonction de zoom fluide, paramétrable via les touches et la molette, avec animation personnalisable. | Client |
| Polymorph | Résout les conflits de recettes en permettant au joueur de choisir manuellement entre plusieurs crafts identiques proposés par différents mods. | Partagé |
| FramedBlocks | Ajoute des blocs à structure définie (escaliers, piliers, cadres, etc.) dont la texture peut être personnalisée avec n’importe quel bloc. | Partagé |
| Torch Slabs Renewed | Permet de placer des torches sur des demi-dalles, escaliers, murs et autres blocs non compatibles par défaut. | Partagé |
| Presence Footsteps | Améliore les sons de pas en fonction du matériau, de l’environnement et de l’équipement, pour un rendu audio plus immersif. | Client |
| Mouse Tweaks | Ajoute des raccourcis et comportements avancés à la souris dans les interfaces : glisser-déposer rapide, tri d’inventaire, remplissage automatique. | Client |
| Placebo | Librairie technique utilisée par certains mods pour gérer des fonctionnalités avancées comme les timers, les effets ou les systèmes de loot. | Partagé |
| Dynamic FPS | Réduit automatiquement l'utilisation des ressources (FPS, rendu) lorsque le jeu est en arrière-plan ou inactif, pour économiser CPU et GPU. | Client |
| ModernFix | Améliore drastiquement les performances client en optimisant la gestion mémoire, les temps de chargement et certains processus internes de rendu. | Partagé |
| FastSuite | Optimise les performances côté serveur pour les systèmes de crafting complexes, en réduisant les calculs redondants lors de la fabrication automatisée. | Partagé |
| Common Capabilities | Étend les capacités Forge partagées entre mods (énergie, inventaires, fluides, etc.) pour améliorer l'interopérabilité et la compatibilité technique. | Partagé |
| Cyclops Core | Librairie de base utilisée par les mods Cyclops. Fournit des outils de configuration, de logique et d’interaction entre blocs. | Partagé |
| CC: Tweaked | Implémente des ordinateurs programmables en Lua, permettant l’automatisation avancée via scripts : redstone, réseau, fichiers, périphériques virtuels. | Partagé |
| Integrated Dynamics | Fournit un système de logique câblée basé sur des variables, réseaux, opérateurs et automatisations conditionnelles. S’intègre avec de nombreux autres mods. | Partagé |
| Applied Energistics 2 | Introduit un système de stockage numérique en réseau avec automatisation, tri, crafting, bus logiques et gestion de l’énergie via canaux. | Partagé |
| Mekanism | Mod industriel complet : machines avancées, tuyaux, systèmes énergétiques, multiblocs, traitement des minerais, gaz et fusions. | Partagé |
| Configured | 	Permet de visualiser et modifier graphiquement les fichiers de configuration .toml directement depuis le jeu. | Client |
| Searchables | Ajoute une fonction de recherche dans les interfaces d'inventaire et de configuration compatibles, pour un accès rapide aux éléments. | Client |
| Embeddium | Fork de Sodium pour Forge. Améliore drastiquement les performances de rendu via une meilleure gestion des chunks, du pipeline graphique et des animations. | Client |
| Oculus | Ajoute le support des shaders via l’API Iris sur Forge. Nécessaire pour utiliser des shaders compatibles Embeddium. | Client |
| Controlling | Améliore l’interface de gestion des contrôles clavier : recherche, détection de conflits et tri des raccourcis. | Client |
| Just Enough Items | Ajoute une interface listant les recettes de craft, de cuisson, et d’utilisation des objets avec moteur de recherche. | Partagé |
| FerriteCore | Réduit l’utilisation mémoire des mods en optimisant les structures de données des objets, blocs et entités. | Partagé |
| Simple Rich Discord Presence | Affiche des informations personnalisées sur le statut du joueur dans Discord via le Rich Presence. | Client |
| Architectury API | API nécessaire au fonctionnement du mod Simple Rich Discord Presence dans l’environnement Forge. | Client |
| Sound Physics Remastered | Implémente un système acoustique avancé simulant la réverbération, l'atténuation et la propagation réaliste du son dans l'environnement du jeu. | Client |
| Alex's Mobs | Ajoute de nouvelles créatures terrestres, aquatiques et volantes avec comportements, loots et mécaniques spécifiques. | Partagé |
| Biomes O' Plenty | Ajoute une large gamme de biomes supplémentaires avec leur génération, végétation et blocs dédiés. | Partagé |

## Contribuer

> Aucune contrainte : ce projet avance au rythme de nos idées, nourri par la passion, la curiosité et le plaisir de concevoir. 😄

Une idée, une amélioration, une envie de t’impliquer ? Tu es le bienvenu — que ce soit par passion, par curiosité ou juste pour le plaisir d’expérimenter ensemble.
