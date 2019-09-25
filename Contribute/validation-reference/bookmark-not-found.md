---
title: internal-bookmark-not-found
description: Erklärung und Lösung zu Problemen beim Erstellen von Dokumentationsartikeln – internal-bookmark-not-found
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 9/10/2019
ms.prod: non-product-specific
ms.openlocfilehash: 53b98f8da199e3495cc00b2388d983191268eee6
ms.sourcegitcommit: 89147521f0aa3b39e7ddf390136b09a43d95c416
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/10/2019
ms.locfileid: "70856218"
---
# <a name="bookmark-not-found"></a><span data-ttu-id="c48dc-103">bookmark-not-found</span><span class="sxs-lookup"><span data-stu-id="c48dc-103">bookmark-not-found</span></span>

## <a name="warning"></a><span data-ttu-id="c48dc-104">Warnung</span><span class="sxs-lookup"><span data-stu-id="c48dc-104">Warning</span></span>

`Cannot find bookmark '{bookmark-id}' in '{parent-file}'.`

<span data-ttu-id="c48dc-105">Sie versuchen, in der aktuellen oder einer anderen Datei eine Überschrift zu verknüpfen, die nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c48dc-105">You're trying to link to a heading in the current file or another file that doesn't exist.</span></span>

## <a name="resolution"></a><span data-ttu-id="c48dc-106">Lösung</span><span class="sxs-lookup"><span data-stu-id="c48dc-106">Resolution</span></span>

[!INCLUDE [docs-authoring-pack](includes/docs-authoring-pack.md)]

<span data-ttu-id="c48dc-107">Überprüfen Sie die Überschrift, die Sie verknüpfen möchten, und aktualisieren Sie den Link.</span><span class="sxs-lookup"><span data-stu-id="c48dc-107">Verify the heading you want to link to and update the link.</span></span>

<span data-ttu-id="c48dc-108">Verwenden Sie ein Hashsymbol gefolgt von der Überschrift, um einen Abschnitt im aktuellen Artikel zu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="c48dc-108">To link to a section in the current article, use a hash symbol, followed by the words of the heading.</span></span> <span data-ttu-id="c48dc-109">Entfernen Sie Satzzeichen aus der Überschrift, und ersetzen Sie Leerzeichen durch Bindestriche.</span><span class="sxs-lookup"><span data-stu-id="c48dc-109">Remove punctuation from the heading and replace spaces with dashes.</span></span> <span data-ttu-id="c48dc-110">Dies ist ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c48dc-110">The following is an example:</span></span>

```markdown
[Managed Disks](#managed-disks)
```

<span data-ttu-id="c48dc-111">Um eine Verknüpfung mit einer Überschrift in einer anderen Datei herzustellen, verwenden Sie einen relativen Link zu dieser Datei gefolgt von einem Hashsymbol und den Wörtern der Überschrift.</span><span class="sxs-lookup"><span data-stu-id="c48dc-111">To link to a heading in another file, use a relative link to that file, followed by a hash symbol and the words of the heading.</span></span> <span data-ttu-id="c48dc-112">Entfernen Sie Satzzeichen aus der Überschrift, und ersetzen Sie Leerzeichen durch Bindestriche.</span><span class="sxs-lookup"><span data-stu-id="c48dc-112">Remove punctuation from the heading and replace spaces with dashes.</span></span> <span data-ttu-id="c48dc-113">Dies ist ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c48dc-113">The following is an example:</span></span>

```markdown
See [the Resolution section in h1-empty](h1-empty.md#resolution).
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]