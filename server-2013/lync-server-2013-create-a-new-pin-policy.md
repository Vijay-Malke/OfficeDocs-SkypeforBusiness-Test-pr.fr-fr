﻿---
title: Créer une stratégie de code confidentiel
TOCTitle: Créer une stratégie de code confidentiel
ms:assetid: 8bdf0478-fe9f-4371-93ff-db39381a25db
ms:mtpsurl: https://technet.microsoft.com/fr-fr/library/Gg182547(v=OCS.15)
ms:contentKeyID: 49298000
ms.date: 05/20/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Créer une stratégie de code confidentiel

 

_**Dernière rubrique modifiée :** 2012-06-19_

Vous pouvez utiliser la page **Stratégie de code confidentiel** pour fournir une authentification par code confidentiel (PIN) aux utilisateurs qui se connectent à Lync 2013 avec des téléphones IP. Pour utiliser l’authentification par code confidentiel, assurez-vous que l’option **Activer l’authentification par code confidentiel** est sélectionnée dans les paramètres de service web. Pour plus d’informations, voir [Modification des paramètres de configuration d’un service web existant](lync-server-2013-modify-existing-web-service-configuration-settings.md).

Suivez cette procédure pour créer une stratégie de code confidentiel au niveau utilisateur ou site.

## Pour créer une stratégie de code confidentiel au niveau utilisateur ou site

1.  À partir d’un compte d’utilisateur membre du groupe RTCUniversalServerAdmins (ou disposant des mêmes droits), ou affecté au rôle CsServerAdministrator ou CsAdministrator, ouvrez une session sur un ordinateur qui se trouve sur le réseau sur lequel vous avez déployé Lync Server 2013.

2.  Ouvrez une fenêtre de navigateur, puis entrez l’URL d’administration pour ouvrir le Panneau de configuration Lync Server. Pour plus d’informations sur les différentes méthodes de démarrage du Panneau de configuration Lync Server, voir [Ouvrir les outils d’administration Lync Server](lync-server-2013-open-lync-server-administrative-tools.md).

3.  Dans la barre de navigation de gauche, cliquez sur **Sécurité**, puis sur **Stratégie de code confidentiel**.

4.  Dans la page **Stratégie de code confidentiel**, cliquez sur **Nouveau**, puis effectuez l’une des opérations suivantes :
    
      - Pour créer une stratégie au niveau utilisateur, cliquez sur **Stratégie de l’utilisateur**. Dans **Nouvelle stratégie de code confidentiel**, dans **Nom**, tapez un nom décrivant la stratégie.
    
      - Pour créer une stratégie au niveau site, cliquez sur **Stratégie du site**. Dans la zone de recherche **Sélectionner un site**, tapez entièrement ou partiellement le nom du site pour lequel vous voulez créer une stratégie. Dans la liste des sites obtenus, cliquez sur le site voulu, puis cliquez sur **OK**.

5.  Dans le champ **Description**, tapez la description de la stratégie de code confidentiel.

6.  Dans le champ **Longueur minimale du code confidentiel**, tapez ou sélectionnez la longueur minimale du code confidentiel que vous souhaitez autoriser. La longueur minimale par défaut est de cinq chiffres.

7.  Si vous voulez spécifier le nombre maximal de tentatives de connexion avant le verrouillage de l’utilisateur, activez la case à cocher **Spécifier le nombre maximal de tentatives de connexion**. Si vous ne sélectionnez pas cette option, le nombre maximal de tentatives est automatiquement déterminé en fonction de la longueur du code confidentiel. Par défaut, le nombre maximal de tentatives est automatiquement déterminé.

8.  Si vous avez activé la case à cocher **Spécifier le nombre maximal de tentatives de connexion**, dans **Nombre maximal de tentatives de connexion**, tapez ou sélectionnez le nombre maximal de tentatives de connexion que vous souhaitez autoriser.

9.  Si vous voulez que les codes confidentiels expirent, activez la case à cocher **Activer l’expiration du code confidentiel**. Si vous ne sélectionnez pas cette option, les codes confidentiels n’expirent jamais. Par défaut, les codes confidentiels n’expirent jamais.

10. Si vous avez activé la case à cocher **Activer l’expiration du code confidentiel**, dans **Le code confidentiel expire au bout de (jours)**, tapez ou sélectionnez le nombre de jours après lequel les codes confidentiels expirent.

11. Dans **Comptage de l’historique du code confidentiel**, tapez le nombre de codes confidentiels qu’un utilisateur doit créer avant qu’il ne puisse réutiliser un code. Par défaut, les utilisateurs peuvent réutiliser leur code confidentiel.

12. Pour autoriser les modèles courants de codes confidentiels, tels que les jeux de chiffres séquentiels et répétitifs, activez la case à cocher **Autoriser les modèles courants**. Si vous ne sélectionnez pas cette option, seuls les modèles complexes de chiffres sont autorisés. Par défaut, seuls les modèles complexes de chiffres sont autorisés.
    
    > [!important]  
    > Nous vous recommandons de ne pas autoriser les modèles courants.

13. Cliquez sur **Valider**.

