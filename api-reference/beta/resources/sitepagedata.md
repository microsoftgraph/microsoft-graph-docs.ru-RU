---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Ситепажедата
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 78661f5ce6336f4430297d8969ff8cd82b761c9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583398"
---
# <a name="sitepagedata-resource"></a><span data-ttu-id="656b0-102">ресурс Ситепажедата</span><span class="sxs-lookup"><span data-stu-id="656b0-102">sitePageData resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656b0-103">Ресурс **ситепажедата** представляет свойства [веб-части][].</span><span class="sxs-lookup"><span data-stu-id="656b0-103">The **sitePageData** resource represents the properties of a [webPart][].</span></span> <span data-ttu-id="656b0-104">Так как эти свойства зависят от веб-части, это OpenType без фиксированных свойств.</span><span class="sxs-lookup"><span data-stu-id="656b0-104">As these properties vary by web part, this is an OpenType with no fixed properties.</span></span>

[Частей]: webpart.md
[webPart]: webpart.md

## <a name="json-representation"></a><span data-ttu-id="656b0-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="656b0-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sitePageData"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="656b0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="656b0-107">Properties</span></span>
<span data-ttu-id="656b0-108">У этого ресурса нет фиксированных свойств, но это OpenType содержит все свойства, необходимые для определения веб-части.</span><span class="sxs-lookup"><span data-stu-id="656b0-108">This resource has no fixed properties, but is an OpenType containing all properties necessary to define a web part.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Defines the data in a web part",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/SitePageData",
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepagedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
