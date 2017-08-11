---
ms.date: 2017-06-05
keywords: powershell,applet de commande
title: Objet ISEMenuItem
ms.assetid: a16660bd-0aee-46fd-ac17-3f022165d089
ms.openlocfilehash: 33de866d706ec2b0894c5bfe49e07fee142b95c0
ms.sourcegitcommit: 598b7835046577841aea2211d613bb8513271a8b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/08/2017
---
# <a name="the-isemenuitem-object"></a><span data-ttu-id="44e50-103">Objet ISEMenuItem</span><span class="sxs-lookup"><span data-stu-id="44e50-103">The ISEMenuItem Object</span></span>
  <span data-ttu-id="44e50-104">Un objet **ISEMenuItem** est une instance de la classe Microsoft.PowerShell.Host.ISE.ISEMenuItem.</span><span class="sxs-lookup"><span data-stu-id="44e50-104">An **ISEMenuItem** object is an instance of the Microsoft.PowerShell.Host.ISE.ISEMenuItem class.</span></span> <span data-ttu-id="44e50-105">Tous les objets du menu **Modules complémentaires** sont des instances de la classe **Microsoft.PowerShell.Host.ISE.ISEMenuItem**.</span><span class="sxs-lookup"><span data-stu-id="44e50-105">All menu objects on the **Add-ons** menu are instances of the **Microsoft.PowerShell.Host.ISE.ISEMenuItem** class.</span></span>

## <a name="properties"></a><span data-ttu-id="44e50-106">Propriétés</span><span class="sxs-lookup"><span data-stu-id="44e50-106">Properties</span></span>

###  <span data-ttu-id="44e50-107"><a name="DisplayName"></a> DisplayName</span><span class="sxs-lookup"><span data-stu-id="44e50-107"><a name="DisplayName"></a> DisplayName</span></span>
  <span data-ttu-id="44e50-108">Prise en charge dans Windows PowerShell ISE 2.0 et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="44e50-108">Supported in Windows PowerShell ISE 2.0 and later.</span></span> 

 <span data-ttu-id="44e50-109">Propriété en lecture seule qui obtient le nom complet de l’élément de menu.</span><span class="sxs-lookup"><span data-stu-id="44e50-109">The read-only property that gets the display name of the menu item.</span></span>

```
# Get the display name of the Add-ons menu item
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
$psISE.CurrentPowerShellTab.AddOnsMenu.DisplayName

```

###  <span data-ttu-id="44e50-110"><a name="Action"></a> Action</span><span class="sxs-lookup"><span data-stu-id="44e50-110"><a name="Action"></a> Action</span></span>
  <span data-ttu-id="44e50-111">Prise en charge dans Windows PowerShell ISE 2.0 et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="44e50-111">Supported in Windows PowerShell ISE 2.0 and later.</span></span> 

 <span data-ttu-id="44e50-112">Propriété en lecture seule qui obtient le bloc de script.</span><span class="sxs-lookup"><span data-stu-id="44e50-112">The read-only property that gets the block of script.</span></span> <span data-ttu-id="44e50-113">Elle appelle l’action qui est associée à l’élément de menu sur lequel vous cliquez.</span><span class="sxs-lookup"><span data-stu-id="44e50-113">It invokes the action when you click the menu item.</span></span>

```
# Get the action associated with the first submenu item.
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus[0].Action

# Invoke the script associated with the first submenu item 
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus[0].Action.Invoke()
```

###  <span data-ttu-id="44e50-114"><a name="Shortcut"></a> Shortcut</span><span class="sxs-lookup"><span data-stu-id="44e50-114"><a name="Shortcut"></a> Shortcut</span></span>
  <span data-ttu-id="44e50-115">Prise en charge dans Windows PowerShell ISE 2.0 et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="44e50-115">Supported in Windows PowerShell ISE 2.0 and later.</span></span> 

 <span data-ttu-id="44e50-116">Propriété en lecture seule qui obtient le raccourci clavier d’entrée Windows associé à l’élément de menu.</span><span class="sxs-lookup"><span data-stu-id="44e50-116">The read-only property that gets the Windows input keyboard shortcut for the menu item.</span></span>

```
# Get the shortcut for the first submenu item.
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus[0].Shortcut
```

###  <span data-ttu-id="44e50-117"><a name="Submenus"></a> Submenus</span><span class="sxs-lookup"><span data-stu-id="44e50-117"><a name="Submenus"></a> Submenus</span></span>
  <span data-ttu-id="44e50-118">Prise en charge dans Windows PowerShell ISE 2.0 et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="44e50-118">Supported in Windows PowerShell ISE 2.0 and later.</span></span> 

 <span data-ttu-id="44e50-119">Propriété en lecture seule qui obtient la [liste des sous-menus](The-ISEMenuItemCollection-Object.md) de l’élément de menu.</span><span class="sxs-lookup"><span data-stu-id="44e50-119">The read-only property that gets the [list of submenus](The-ISEMenuItemCollection-Object.md) of the menu item.</span></span>

```
# List the submenus of the Add-ons menu
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P")
$psISE.CurrentPowerShellTab.AddOnsMenu.Submenus
```

## <a name="scripting-example"></a><span data-ttu-id="44e50-120">Exemple de script</span><span class="sxs-lookup"><span data-stu-id="44e50-120">Scripting example</span></span>
 <span data-ttu-id="44e50-121">Pour mieux comprendre l’utilisation du menu Modules complémentaires et ses propriétés de script, consultez l’exemple de script suivant.</span><span class="sxs-lookup"><span data-stu-id="44e50-121">To better understand the use of the Add-ons menu and its scriptable properties, read through the following scripting example.</span></span>

```

# This is a scripting example that shows the use of the Add-ons menu.
# Clear the Add-ons menu if any entries currently exist
$psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Clear()

# Add an Add-ons menu item with an shortcut and fast access key.
# Note the use of “_”  as opposed to the “&” for mapping to the fast access key letter for the menu item.
$menuAdded = $psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("_Process",{get-process},"Alt+P") 
# Add a nested menu - a parent and a child submenu item. 
$parentAdded = $psISE.CurrentPowerShellTab.AddOnsMenu.SubMenus.Add("Parent",$null,$null) 
$parentAdded.SubMenus.Add("_Dir",{dir},"Alt+D")

```

## <a name="see-also"></a><span data-ttu-id="44e50-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44e50-122">See Also</span></span>
- [<span data-ttu-id="44e50-123">Objet ISEMenuItemCollection</span><span class="sxs-lookup"><span data-stu-id="44e50-123">The ISEMenuItemCollection Object</span></span>](The-ISEMenuItemCollection-Object.md) 
- [<span data-ttu-id="44e50-124">Modèle objet de script Windows PowerShell ISE</span><span class="sxs-lookup"><span data-stu-id="44e50-124">The Windows PowerShell ISE Scripting Object Model</span></span>](The-Windows-PowerShell-ISE-Scripting-Object-Model.md) 
- [<span data-ttu-id="44e50-125">Informations de référence sur le modèle objet Windows PowerShell ISE</span><span class="sxs-lookup"><span data-stu-id="44e50-125">Windows PowerShell ISE Object Model Reference</span></span>](Windows-PowerShell-ISE-Object-Model-Reference.md) 
- [<span data-ttu-id="44e50-126">Hiérarchie du modèle objet ISE</span><span class="sxs-lookup"><span data-stu-id="44e50-126">The ISE Object Model Hierarchy</span></span>](The-ISE-Object-Model-Hierarchy.md)

  