---
layout: "post"
title: "Découvrir la cinétique avec de drôles de réactions chimiques : un TP autour de l'iode et du peroxyde d'hydrogène"
date: 2024-10-19 10:00:00 +0100
categories: [Ressources_Physique-Chimie, Travaux_Pratiques]
tags: [ressources_physique-chimie, ressources_lycée, travaux_pratiques, lycée, cinétique_chimique]     # TAG names should always be lowercase
author: <tobias>
---

Découvrir la cinétique avec de drôles de réactions chimiques : un TP autour de l'iode et du peroxyde d'hydrogène
=======

Je vous propose aujourd'hui un sujet de **TP** pour expliquer la **notion de cinétique chimique** au travers de deux réactions visuelles et amusantes. Idéal dans le cadre du programme de **terminale spécialité physique-chimie**. Ce TP se penche sur deux réactions : la réaction de **Briggs-Rauscher**, et la réaction du **Dentifrice d'Éléphant**. Le caractère ludique de ces deux réactions est propice à un TP "avant vacances" plus détendu même si de nombreuses questions d'exploitation sont présentes et même si **d'importantes précautions de sécurité sont à prévoir**.

Le plan du TP
-----------
J'ai découpé le TP en trois parties :
* **Partie 1 : La réaction de Briggs-Rauscher**
* **Partie 1bis : Briggs-Rauscher en Python** (cette partie est uniquement théorique, elle consiste en l'étude d'un programme python modélisant les lois de vitesse et les concentrations des intermédiaires qui agissent dans la réaction)
* **Partie 2 : Le dentifrice d’éléphant**

Le TP peut être réalisé en deux heures, avec environ **1h10** sur la réaction de Briggs-Rauscher, **15 min** sur l'exploitation python et **25 min** sur la réaction du dentifrice d'éléphant. Toutefois, les questions plus portées sur la théorie ou l'exploitation de résultats sont précédées d'un petit icône en forme d'ampoule. On peut donc les repérer et ne les traiter qu'à l'issue du TP pour se concentrer sur la manipulation.

Avertissements de sécurité
-----------
Ce TP utilise **des réactifs dangereux si on ne les manipule pas correctement** dont : du peroxyde d'hydrogène, du diiode, de l'iodure et de l'iodate de potassium, de l'acide sulfurique concentré etc. Les précautions nécessaires sont expliquées dans le TP et plusieurs questions portent sur la sécurité, mais je préfère lister ici tous les avertissements de sécurité et les précautions conseillées que l'on rencontre sur els étiquettes des produits utilisés, selon la nomenclature du règlement CLP :

**Mentions de danger** :
* H272 - Peut aggraver un incendie ; comburant
* H290 - Peut être corrosif pour les métaux
* H302 - Nocif en cas d’ingestion
* H312 - Nocif par contact cutané
* H314 - Provoque de graves brûlures de la peau et de graves lésions des yeux
* H315 - Provoque une irritation cutanée
* H318 - Provoque de graves lésions des yeux
* H319 - Provoque une sévère irritation des yeux
* H332 - Nocif par inhalation
* H335 - Peut irriter les voies respiratoires
* H400 - Très toxique pour les organismes aquatiques

**Conseils de prudence**
* P210 - Tenir à l’écart de la chaleur, des surfaces chaudes, des étincelles, des flammes nues et de toute autre source d’inflammation. Ne pas fumer.
* P220 - Tenir à l’écart des vêtements et d’autres matières combustibles
* P234 - Conserver uniquement dans l’emballage d’origine
* P264 - Se laver. . . soigneusement après manipulation
* P273 - Eviter le rejet dans l’environnement
* P280 - Porter des gants de protection/des vêtements de protection/un équipement de protection des yeux/du visage/une protection auditive/. . .
* P301 + P312 - EN CAS D’INGESTION : appeler un CENTRE ANTIPOISON / un médecin . . ./en cas de malaise
* P302 + P352 - EN CAS DE CONTACT AVEC LA PEAU : laver abondamment à l’eau / . . .
* P303 + P362 + P353 - EN CAS DE CONTACT AVEC LA PEAU (ou les cheveux) : enlever immédiatement tous les vêtements contaminés. Rincer la peau à l’eau [ou se doucher]
* P304 + P340 - EN CAS D’INHALATION : transporter la personne à l’extérieur et la maintenir dans une position où elle peut confortablement respirer
* P305 + P351 + P338 - EN CAS DE CONTACT AVEC LES YEUX : rincer avec précaution à l’eau pendant
* plusieurs minutes. Enlever les lentilles de contact si la victime en porte et si elles peuvent être facilement enlevées. Continuer à rincer
* P314 - Consulter un médecin en cas de malaise
* P363 - Laver les vêtements contaminés avant réutilisation
* P501 - Éliminer le contenu/récipient dans un contenant prévu à cet effet
