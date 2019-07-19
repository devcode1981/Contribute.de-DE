---
title: validation-timeout
description: Erklärung und Lösung zu Problemen beim Erstellen von Dokumentationsartikeln – validation-timeout
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 6/5/2019
ms.prod: non-product-specific
ms.openlocfilehash: 00461768491c25b9bafaff6b117a356d9e291e22
ms.sourcegitcommit: 412ce4ab23e758d41947043f1463e96595ba3bfe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2019
ms.locfileid: "67033295"
---
# <a name="validation-timeout"></a><span data-ttu-id="25898-103">validation-timeout</span><span class="sxs-lookup"><span data-stu-id="25898-103">validation-timeout</span></span>

## <a name="warning"></a><span data-ttu-id="25898-104">Warnung</span><span class="sxs-lookup"><span data-stu-id="25898-104">Warning</span></span>

`The call to the validation service timed out and validation was not completed. This happens when there's an issue with the service and continuing to retry the call could cause build delays. You might have content issues that were not reported. To retry validation, close and re-open your PR, or rebuild your branch via Docs Portal (requires admin permissions). If you need admin help or  If you continue to see this message, file an issue via https://SiteHelp.`

<span data-ttu-id="25898-105">Gelegentlich verhindern vorübergehende Probleme beim Validierungsdienst (z.B. ein fehlerhafter Serverzustand), dass der Dienst bei der Erstellung von Dokumentationsartikeln erfolgreich aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="25898-105">Sometimes transient issues in the validation service, such as a server in a bad state, prevent Docs Build from successfully calling the service.</span></span> <span data-ttu-id="25898-106">Nach mehreren Versuchen erfolgt ein Timeout für den Aufruf, und die Validierung wird abgebrochen, um Verzögerungen bei der Erstellung und eine Blockierung der Buildpipeline zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="25898-106">After several tries, the call times out and validation is canceled to avoid build delays and clogging the build pipeline.</span></span>

## <a name="resolution"></a><span data-ttu-id="25898-107">Lösung</span><span class="sxs-lookup"><span data-stu-id="25898-107">Resolution</span></span>

<span data-ttu-id="25898-108">Schließen Sie den PR, und öffnen Sie ihn noch mal, oder führen Sie einen manuellen Buildvorgang über das Docs-Portal durch (nur für Repositoryadministratoren).</span><span class="sxs-lookup"><span data-stu-id="25898-108">Try closing and re-opening your PR, or re-running a manual build via Docs Portal (repo admins only).</span></span> <span data-ttu-id="25898-109">Häufig erledigen sich Dienstprobleme nach dem ersten Wiederholungsversuch von selbst.</span><span class="sxs-lookup"><span data-stu-id="25898-109">Often service issues clear themselves up after the initial retry.</span></span> <span data-ttu-id="25898-110">Wenn Sie die Hilfe eines Administrators benötigen oder die Meldung weiterhin erhalten, erstellen Sie ein Issue über [https://SiteHelp](https://SiteHelp), wenn Sie Microsoft-Mitarbeiter sind, oder erwähnen Sie in Ihrem PR den Autor eines Artikels mithilfe des @-Zeichens, um Unterstützung zu erhalten, wenn Sie ein externer Mitwirkender sind.</span><span class="sxs-lookup"><span data-stu-id="25898-110">If you need help from an admin or if you continue to get this message, file an issue via [https://SiteHelp](https://SiteHelp) if you're a Microsoft employee, or @ mention the author of an article in your PR for assistance if you're an external contributor.</span></span>

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]