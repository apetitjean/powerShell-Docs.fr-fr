---
ms.date: 2017-06-12
ms.topic: conceptual
keywords: dsc,powershell,configuration,setup
title: "Méthode RemoveConfiguration de la classe MSFT_DSCLocalConfigurationManager"
ms.openlocfilehash: fed45836293adedbce18f01cfe53cdfa1a474975
ms.sourcegitcommit: a444406120e5af4e746cbbc0558fe89a7e78aef6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/17/2018
---
# <a name="removeconfiguration-method-of-the-msftdsclocalconfigurationmanager-class"></a>Méthode RemoveConfiguration de la classe MSFT_DSCLocalConfigurationManager

Supprime les fichiers de configuration.

<a name="syntax"></a>Syntaxe
------

```mof
uint32 RemoveConfiguration(
  [in] uint32  Stage,
  [in] boolean Force
);
```

<a name="parameters"></a>Paramètres
----------

*Stage* \[in\]  
Spécifie le document de configuration à supprimer. Les valeurs suivantes sont valides :

|Valeur |Description |
|:--- |:---|
|**1** | Document de configuration **Current** (current.mof). |
|**2** | Document de configuration **Pending** (pending.mof).  |
|**4** | Document de configuration **Previous** (previous.mof). |

*Force* \[in\]  
**true** pour forcer la suppression de la configuration.

## <a name="return-value"></a>Valeur renvoyée
------------

Retourne zéro en cas de réussite ; sinon, retourne un code d’erreur.

## <a name="remarks"></a>Remarques

Il s’agit d’une méthode statique.

## <a name="requirements"></a>Spécifications
------------
>**MOF :** DscCore.mof

>**Espace de noms** : Root\Microsoft\Windows\DesiredStateConfiguration


## <a name="see-also"></a>Voir aussi


[**MSFT_DSCLocalConfigurationManager**](msft-dsclocalconfigurationmanager.md)


 

 



