---
ms.date: 2017-06-12
ms.topic: conceptual
keywords: dsc,powershell,configuration,setup
title: Ressource DSC WaitForSome
ms.openlocfilehash: cbe16c543f0eeb62dbe1fb439af2f9147f1bc210
ms.sourcegitcommit: a444406120e5af4e746cbbc0558fe89a7e78aef6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/17/2018
---
# <a name="dsc-waitforsome-resource"></a>Ressource DSC WaitForSome

> S’applique à : Windows PowerShell 5.0 et ultérieur

La ressource de configuration d’état souhaité (DSC) **WaitForAny** peut être utilisée dans un bloc de nœud dans une [configuration DSC](configurations.md) pour spécifier les dépendances sur les configurations sur d’autres nœuds.

La ressource réussit si la ressource spécifiée dans la propriété **ResourceName** est dans l’état souhaité sur un nombre minimal de nœuds (spécifié par **NodeCount**) défini par la propriété **NodeName**. 


## <a name="syntax"></a>Syntaxe

```
WaitForSome [String] #ResourceName
{
    NodeCount = [UInt32]
    NodeName = [string[]]
    ResourceName = [string]
    [DependsOn = [string[]]]
    [PsDscRunAsCredential = [PSCredential]]
    [RetryCount = [UInt32]]
    [RetryIntervalSec = [UInt64]]
    [ThrottleLimit = [UInt32]]
}
```

## <a name="properties"></a>Propriétés

|  Propriété  |  Description   | 
|---|---| 
| NodeCount| Le nombre minimal de nœuds qui doivent être dans l’état souhaité pour que cette ressource réussisse.|
| NodeName| Les nœuds cible de la ressource de la dépendance.| 
| Nom_ressource| Le nom de la ressource de la dépendance.| 
| RetryIntervalSec| Le nombre de secondes avant la nouvelle tentative. Le minimum est 1.| 
| RetryCount| Le nombre maximum de nouvelles tentatives.| 
| ThrottleLimit| Le nombre de machines à connecter simultanément. La valeur par défaut est new-cimsession.| 
| DependsOn | Indique que la configuration d’une autre ressource doit être exécutée avant celle de cette ressource. Par exemple, si vous voulez exécuter en premier le bloc de script de configuration de ressource __ResourceName__ de type __ResourceType__, la syntaxe pour utiliser cette propriété est `DependsOn = "[ResourceType]ResourceName"`.|
| PsDscRunAsCredential | Voir [Exécution de DSC avec les informations d’identification de l’utilisateur](https://docs.microsoft.com/en-us/powershell/dsc/runasuser) |


## <a name="example"></a>Exemple

Pour obtenir un exemple d’utilisation de cette ressource, consultez [Spécification des dépendances entre nœuds](crossNodeDependencies.md)

