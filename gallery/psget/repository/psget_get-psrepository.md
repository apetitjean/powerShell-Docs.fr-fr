---
ms.date: 2017-06-12
contributor: manikb
ms.topic: reference
keywords: gallery,powershell,cmdlet,psget
title: Get-PSRepository
ms.openlocfilehash: 96f87428312c233757aa5fcae405a192aadff385
ms.sourcegitcommit: 75f70c7df01eea5e7a2c16f9a3ab1dd437a1f8fd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/12/2017
---
# <a name="get-psrepository"></a>Get-PSRepository

Obtient les référentiels enregistrés sur un ordinateur.

## <a name="description"></a>Description

L’applet de commande Get-PSRepository obtient les référentiels de modules PowerShell qui sont enregistrés pour l’utilisateur actuel sur un ordinateur.

Pour chaque référentiel enregistré, Get-PSRepository retourne un objet PSRepository qui peut éventuellement être transmis à Unregister-PSRepository pour annuler l’enregistrement d’un référentiel enregistré.

## <a name="cmdlet-syntax"></a>Syntaxe de l’applet de commande
```powershell
Get-Command -Name Get-PSRepository -Module PowerShellGet -Syntax
```

## <a name="cmdlet-online-help-reference"></a>Référence de l’aide en ligne de l’applet de commande

[Get-PSRepository](http://go.microsoft.com/fwlink/?LinkID=517127)

## <a name="example-commands"></a>Exemples de commandes

```powershell

# Properties of Get-PSRepository returned object
Get-PSRepository PSGallery | Format-List * -Force

Name                      : PSGallery
SourceLocation            : https://www.powershellgallery.com/api/v2/
Trusted                   : False
Registered                : True
InstallationPolicy        : Untrusted
PackageManagementProvider : NuGet
PublishLocation           : https://www.powershellgallery.com/api/v2/package/
ScriptSourceLocation      : https://www.powershellgallery.com/api/v2/items/psscript/
ScriptPublishLocation     : https://www.powershellgallery.com/api/v2/package/
ProviderOptions           : {}

# Get all registered repositories
Get-PSRepository

# Get a specific registered repository
Get-PSRepository PSGallery

Name                      InstallationPolicy   SourceLocation
----                      ------------------   --------------
PSGallery                 Untrusted            https://www.powershellgallery.com/api/v2/

# Get registered repository with wildcards
Get-PSRepository *Gallery*

```

