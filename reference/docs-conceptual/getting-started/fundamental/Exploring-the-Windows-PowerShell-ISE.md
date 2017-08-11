---
ms.date: 2017-06-05
keywords: powershell,applet de commande
title: "Découverte de Windows PowerShell ISE"
ms.assetid: e0d2c6e8-5126-40e7-a1e1-d1cff29fe94a
ms.openlocfilehash: 979209d4b200728b7e78e341bb9595741d2b8e68
ms.sourcegitcommit: 598b7835046577841aea2211d613bb8513271a8b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/08/2017
---
# <a name="exploring-the-windows-powershell-ise"></a><span data-ttu-id="b623d-103">Découverte de Windows PowerShell ISE</span><span class="sxs-lookup"><span data-stu-id="b623d-103">Exploring the Windows PowerShell ISE</span></span>
<span data-ttu-id="b623d-104">Vous pouvez utiliser l’environnement d’écriture de scripts intégré (ISE) de Windows PowerShell® pour créer, exécuter et déboguer des commandes et des scripts.</span><span class="sxs-lookup"><span data-stu-id="b623d-104">You can use the Windows PowerShell® Integrated Scripting Environment (ISE) to create, run, and debug commands and scripts.</span></span> <span data-ttu-id="b623d-105">Windows PowerShell ISE se compose d’une barre de menus, d’onglets Windows PowerShell, d’une barre d’outils, d’onglets de script, d’un volet Script, d’un volet Console, d’une barre d’état, d’un curseur de taille de texte et d’une aide contextuelle.</span><span class="sxs-lookup"><span data-stu-id="b623d-105">The Windows PowerShell ISE consists of the menu bar, Windows PowerShell tabs, the toolbar, script tabs, a Script Pane, a Console Pane, a status bar, a text-size slider and context-sensitive Help.</span></span>

> [!NOTE]
> <span data-ttu-id="b623d-106">Depuis Windows PowerShell ISE 3.0, les volets Commande et Sortie ont été combinés en un seul volet Console.</span><span class="sxs-lookup"><span data-stu-id="b623d-106">Beginning with Windows PowerShell ISE 3.0 the Command and Output Panes were combined into a single Console Pane.</span></span>

## <a name="menu-bar"></a><span data-ttu-id="b623d-107">Barre de menus</span><span class="sxs-lookup"><span data-stu-id="b623d-107">Menu Bar</span></span>
<span data-ttu-id="b623d-108">La barre de menus contient les menus **Fichier**, **Modifier**, **Affichage**, **Outils**, **Débogage**, **Modules complémentaires** et **Aide**.</span><span class="sxs-lookup"><span data-stu-id="b623d-108">The menu bar contains the **File**, **Edit**, **View**, **Tools**, **Debug**, **Add-ons**, and **Help** menus.</span></span> <span data-ttu-id="b623d-109">Les boutons dans les menus permettent d’effectuer des tâches liées à l’écriture et à l’exécution de scripts, ainsi qu’à l’exécution de commandes dans Windows PowerShell ISE.</span><span class="sxs-lookup"><span data-stu-id="b623d-109">The buttons on the menus allow you to perform tasks related to writing and running scripts and running commands in the Windows PowerShell ISE.</span></span> <span data-ttu-id="b623d-110">En outre, il est possible de placer un [outil complémentaire](../../core-powershell/ise/The-ISEAddOnTool-Object.md) sur la barre de menus en exécutant des scripts qui utilisent le [Modèle objet de script Windows PowerShell ISE](../../core-powershell/ise/The-Windows-PowerShell-ISE-Scripting-Object-Model.md).</span><span class="sxs-lookup"><span data-stu-id="b623d-110">Additionally, an [add-on tool](../../core-powershell/ise/The-ISEAddOnTool-Object.md) may be placed on the menu bar by running scripts that use the [Windows PowerShell ISE Scripting Object Model](../../core-powershell/ise/The-Windows-PowerShell-ISE-Scripting-Object-Model.md).</span></span>

> [!NOTE]
> <span data-ttu-id="b623d-111">Dans Windows PowerShell ISE 2.0, les menus **Outils** et **Modules complémentaires** n’étaient pas présents.</span><span class="sxs-lookup"><span data-stu-id="b623d-111">In Windows PowerShell ISE 2.0, The **Tools** and **Add-ons** menus were not present.</span></span>

## <a name="windows-powershell-tabs"></a><span data-ttu-id="b623d-112">Onglets Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="b623d-112">Windows PowerShell Tabs</span></span>
<span data-ttu-id="b623d-113">Un onglet Windows PowerShell est un environnement dans lequel s’exécute un script Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b623d-113">A Windows PowerShell tab is the environment in which a Windows PowerShell script runs.</span></span> <span data-ttu-id="b623d-114">Vous pouvez ouvrir de nouveaux onglets Windows PowerShell dans Windows PowerShell ISE pour créer des environnements distincts sur votre ordinateur local ou sur des ordinateurs distants.</span><span class="sxs-lookup"><span data-stu-id="b623d-114">You can open new Windows PowerShell tabs in the Windows PowerShell ISE to create separate environments on your local computer or on remote computers.</span></span> <span data-ttu-id="b623d-115">Vous pouvez avoir au maximum huit onglets PowerShell ouverts simultanément.</span><span class="sxs-lookup"><span data-stu-id="b623d-115">You may have a maximum of eight PowerShell tabs simultaneously open.</span></span>

## <a name="toolbar"></a><span data-ttu-id="b623d-116">Barre d’outils</span><span class="sxs-lookup"><span data-stu-id="b623d-116">Toolbar</span></span>
<span data-ttu-id="b623d-117">La barre d’outils contient les boutons suivants.</span><span class="sxs-lookup"><span data-stu-id="b623d-117">The following buttons are located on the toolbar.</span></span>

|<span data-ttu-id="b623d-118">Bouton</span><span class="sxs-lookup"><span data-stu-id="b623d-118">Button</span></span>|<span data-ttu-id="b623d-119">Function</span><span class="sxs-lookup"><span data-stu-id="b623d-119">Function</span></span>|
|----------|------------|
|<span data-ttu-id="b623d-120">**Nouveau**</span><span class="sxs-lookup"><span data-stu-id="b623d-120">**New**</span></span>|<span data-ttu-id="b623d-121">Ouvre un nouveau script.</span><span class="sxs-lookup"><span data-stu-id="b623d-121">Opens a new script.</span></span>|
|<span data-ttu-id="b623d-122">**Ouvrir**</span><span class="sxs-lookup"><span data-stu-id="b623d-122">**Open**</span></span>|<span data-ttu-id="b623d-123">Ouvre un fichier ou un script existant.</span><span class="sxs-lookup"><span data-stu-id="b623d-123">Opens an existing script or file.</span></span>|
|<span data-ttu-id="b623d-124">**Enregistrer**</span><span class="sxs-lookup"><span data-stu-id="b623d-124">**Save**</span></span>|<span data-ttu-id="b623d-125">Enregistre un script ou un fichier.</span><span class="sxs-lookup"><span data-stu-id="b623d-125">Saves a script or file.</span></span>|
|<span data-ttu-id="b623d-126">**Couper**</span><span class="sxs-lookup"><span data-stu-id="b623d-126">**Cut**</span></span>|<span data-ttu-id="b623d-127">Coupe le texte sélectionné et le copie dans le Presse-papiers.</span><span class="sxs-lookup"><span data-stu-id="b623d-127">Cuts the selected text and copies it to the clipboard.</span></span>|
|<span data-ttu-id="b623d-128">**Copier**</span><span class="sxs-lookup"><span data-stu-id="b623d-128">**Copy**</span></span>|<span data-ttu-id="b623d-129">Copie le texte sélectionné dans le Presse-papiers.</span><span class="sxs-lookup"><span data-stu-id="b623d-129">Copies the selected text to the clipboard.</span></span>|
|<span data-ttu-id="b623d-130">**Coller**</span><span class="sxs-lookup"><span data-stu-id="b623d-130">**Paste**</span></span>|<span data-ttu-id="b623d-131">Colle le contenu du Presse-papiers à l’emplacement du curseur.</span><span class="sxs-lookup"><span data-stu-id="b623d-131">Pastes the contents of the clipboard at the cursor location.</span></span>|
|<span data-ttu-id="b623d-132">**Effacer le volet de sortie**</span><span class="sxs-lookup"><span data-stu-id="b623d-132">**Clear Output Pane**</span></span>|<span data-ttu-id="b623d-133">Efface tout le contenu du volet sortie.</span><span class="sxs-lookup"><span data-stu-id="b623d-133">Clears all content in the Output Pane.</span></span>|
|<span data-ttu-id="b623d-134">**Annuler**</span><span class="sxs-lookup"><span data-stu-id="b623d-134">**Undo**</span></span>|<span data-ttu-id="b623d-135">Annule l’action qui vient d’être exécutée.</span><span class="sxs-lookup"><span data-stu-id="b623d-135">Reverses the action that was just performed.</span></span>|
|<span data-ttu-id="b623d-136">**Rétablir**</span><span class="sxs-lookup"><span data-stu-id="b623d-136">**Redo**</span></span>|<span data-ttu-id="b623d-137">Effectue l’action qui vient d’être annulée.</span><span class="sxs-lookup"><span data-stu-id="b623d-137">Performs the action that was just undone.</span></span>|
|<span data-ttu-id="b623d-138">**Exécuter un script**</span><span class="sxs-lookup"><span data-stu-id="b623d-138">**Run Script**</span></span>|<span data-ttu-id="b623d-139">Exécute un script.</span><span class="sxs-lookup"><span data-stu-id="b623d-139">Runs a script.</span></span>|
|<span data-ttu-id="b623d-140">**Exécuter la sélection**</span><span class="sxs-lookup"><span data-stu-id="b623d-140">**Run Selction**</span></span>|<span data-ttu-id="b623d-141">Exécute une partie sélectionnée d’un script.</span><span class="sxs-lookup"><span data-stu-id="b623d-141">Runs a selected portion of a script.</span></span>|
|<span data-ttu-id="b623d-142">**Arrêter l’exécution**</span><span class="sxs-lookup"><span data-stu-id="b623d-142">**Stop Execution**</span></span>|<span data-ttu-id="b623d-143">Arrête un script en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="b623d-143">Stops a script that is running.</span></span>|
|<span data-ttu-id="b623d-144">**Nouvel onglet PowerShell à distance**</span><span class="sxs-lookup"><span data-stu-id="b623d-144">**New Remote PowerShell Tab**</span></span>|<span data-ttu-id="b623d-145">Crée un onglet PowerShell qui établit une session sur un ordinateur distant.</span><span class="sxs-lookup"><span data-stu-id="b623d-145">Creates a new PowerShell Tab that establishes a session on a remote computer.</span></span> <span data-ttu-id="b623d-146">Une boîte de dialogue s’affiche et vous invite à entrer les détails requis pour établir la connexion à distance.</span><span class="sxs-lookup"><span data-stu-id="b623d-146">A dialog box appears and prompts you to enter details required to establish the remote connection.</span></span>|
|<span data-ttu-id="b623d-147">**Démarrer PowerShell.exe**</span><span class="sxs-lookup"><span data-stu-id="b623d-147">**Start PowerShell.exe**</span></span>|<span data-ttu-id="b623d-148">Ouvre une console PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b623d-148">Opens a PowerShell Console.</span></span>|
|<span data-ttu-id="b623d-149">**Afficher le volet Script en haut**</span><span class="sxs-lookup"><span data-stu-id="b623d-149">**Show Script Pane Top**</span></span>|<span data-ttu-id="b623d-150">Déplace le volet Script vers le haut de l’écran.</span><span class="sxs-lookup"><span data-stu-id="b623d-150">Moves the Script Pane to the top in the display.</span></span>|
|<span data-ttu-id="b623d-151">**Afficher le volet Script à droite**</span><span class="sxs-lookup"><span data-stu-id="b623d-151">**Show Script Pane Right**</span></span>|<span data-ttu-id="b623d-152">Déplace le volet Script vers la droite de l’écran.</span><span class="sxs-lookup"><span data-stu-id="b623d-152">Moves the Script Pane to the right in the display.</span></span>|
|<span data-ttu-id="b623d-153">**Afficher le volet Script agrandi**</span><span class="sxs-lookup"><span data-stu-id="b623d-153">**Show Script Pane Maximized**</span></span>|<span data-ttu-id="b623d-154">Agrandit le volet Script.</span><span class="sxs-lookup"><span data-stu-id="b623d-154">Maximizes the Script Pane.</span></span>|

## <a name="script-tab"></a><span data-ttu-id="b623d-155">Onglet de script</span><span class="sxs-lookup"><span data-stu-id="b623d-155">Script Tab</span></span>
<span data-ttu-id="b623d-156">Affiche le nom du script que vous modifiez.</span><span class="sxs-lookup"><span data-stu-id="b623d-156">Displays the name of the script you are editing.</span></span> <span data-ttu-id="b623d-157">Vous pouvez cliquer sur un onglet de script pour sélectionner le script à modifier.</span><span class="sxs-lookup"><span data-stu-id="b623d-157">You can click a script tab to select the script you want to edit.</span></span>

<span data-ttu-id="b623d-158">Lorsque vous pointez sur l’onglet de script, le chemin d’accès complet au fichier de script s’affiche dans une info-bulle.</span><span class="sxs-lookup"><span data-stu-id="b623d-158">When you point to the script tab, the fully qualified path to the script file appears in a tooltip.</span></span>

## <a name="script-pane"></a><span data-ttu-id="b623d-159">Volet Script</span><span class="sxs-lookup"><span data-stu-id="b623d-159">Script Pane</span></span>
<span data-ttu-id="b623d-160">Permet de créer et d’exécuter des scripts.</span><span class="sxs-lookup"><span data-stu-id="b623d-160">Allows you to create and run scripts.</span></span> <span data-ttu-id="b623d-161">Vous pouvez ouvrir, modifier et exécuter des scripts dans le volet Script.</span><span class="sxs-lookup"><span data-stu-id="b623d-161">You can open, edit and run existing scripts in the Script Pane.</span></span>

## <a name="output-pane"></a><span data-ttu-id="b623d-162">Volet Sortie</span><span class="sxs-lookup"><span data-stu-id="b623d-162">Output Pane</span></span>
<span data-ttu-id="b623d-163">Affiche les résultats des commandes et des scripts que vous avez exécutés.</span><span class="sxs-lookup"><span data-stu-id="b623d-163">Displays the results of the commands and scripts you have run.</span></span> <span data-ttu-id="b623d-164">Vous pouvez également copier et effacer le contenu du volet de sortie.</span><span class="sxs-lookup"><span data-stu-id="b623d-164">You can also copy and clear the contents in the Output Pane.</span></span>

## <a name="command-pane"></a><span data-ttu-id="b623d-165">Volet Commande</span><span class="sxs-lookup"><span data-stu-id="b623d-165">Command Pane</span></span>
<span data-ttu-id="b623d-166">Permet d’écrire des commandes.</span><span class="sxs-lookup"><span data-stu-id="b623d-166">Allows you to write commands.</span></span> <span data-ttu-id="b623d-167">Vous pouvez exécuter une commande d’une ou plusieurs lignes dans le volet Commande.</span><span class="sxs-lookup"><span data-stu-id="b623d-167">You can run a one line command or a multiline command in the Command Pane.</span></span> <span data-ttu-id="b623d-168">Appuyez sur Maj+Entrée pour entrer chaque ligne d’une commande en comportant plusieurs, puis appuyez sur Entrée après la dernière ligne pour exécuter la commande multiligne.</span><span class="sxs-lookup"><span data-stu-id="b623d-168">Press SHIFT+ENTER to enter each line of a multiline command, and press ENTER after the last line to execute the multiline command.</span></span> <span data-ttu-id="b623d-169">L’invite affichée en haut du volet Commandes affiche le chemin d’accès au répertoire de travail actif.</span><span class="sxs-lookup"><span data-stu-id="b623d-169">The prompt displayed on top of the Command Pane shows the path to the current working directory.</span></span>

## <a name="status-bar"></a><span data-ttu-id="b623d-170">Barre d’état</span><span class="sxs-lookup"><span data-stu-id="b623d-170">Status Bar</span></span>
<span data-ttu-id="b623d-171">Permet de voir si l’exécution de commandes et de scripts est terminée.</span><span class="sxs-lookup"><span data-stu-id="b623d-171">Allows you to see whether the commands and scripts that you run are complete.</span></span> <span data-ttu-id="b623d-172">La barre d’état figure au bas de l’écran.</span><span class="sxs-lookup"><span data-stu-id="b623d-172">The status bar is at the very bottom of the display.</span></span> <span data-ttu-id="b623d-173">La barre d’état affiche des parties sélectionnées des messages d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b623d-173">Selected portions of error messages are displayed on the status bar.</span></span>

## <a name="text-size-slider"></a><span data-ttu-id="b623d-174">Curseur de taille de texte</span><span class="sxs-lookup"><span data-stu-id="b623d-174">Text-Size Slider</span></span>
<span data-ttu-id="b623d-175">Augmente ou diminue la taille du texte à l’écran.</span><span class="sxs-lookup"><span data-stu-id="b623d-175">Increases or decreases the size of the text on the screen.</span></span>

## <a name="help"></a><span data-ttu-id="b623d-176">Aide</span><span class="sxs-lookup"><span data-stu-id="b623d-176">Help</span></span>
<span data-ttu-id="b623d-177">L’aide sur Windows PowerShell ISE est disponible sur le web dans la bibliothèque TechNet.</span><span class="sxs-lookup"><span data-stu-id="b623d-177">Help for Windows PowerShell ISE is available on the Web in the TechNet Library.</span></span> <span data-ttu-id="b623d-178">Vous pouvez accéder à l’aide en cliquant sur **Aide Windows PowerShell ISE** dans le menu **Aide**, ou en appuyant sur la touche F1 n’importe où, sauf quand le curseur est positionné sur un nom d’applet de commande dans le volet Script ou Console.</span><span class="sxs-lookup"><span data-stu-id="b623d-178">You can open the Help by clicking **Windows PowerShell ISE Help** on the **Help** menu or by pressing the F1 key anywhere except when the cursor is on a cmdlet name in either the Script Pane or the Console Pane.</span></span> <span data-ttu-id="b623d-179">À partir du menu **Aide** vous pouvez également exécuter l’applet de commande Update-Help et afficher la fenêtre Commande qui vous aide à construire des commandes en affichant tous les paramètres disponibles pour une applet de commande, et en vous permettant d’entrer les paramètres dans un formulaire simple d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="b623d-179">From the **Help** menu you can also run the Update-Help cmdlet, and display the Command Window which assists you in constructing commands by showing you all of the parameters for a cmdlet and enabling you to fill in the parameters in an easy-to-use form.</span></span>

## <a name="see-also"></a><span data-ttu-id="b623d-180">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b623d-180">See Also</span></span>
- [<span data-ttu-id="b623d-181">Utilisation de Windows PowerShell ISE</span><span class="sxs-lookup"><span data-stu-id="b623d-181">Using the Windows PowerShell ISE</span></span>](../../core-powershell/ise/Using-the-Windows-PowerShell-ISE.md)
