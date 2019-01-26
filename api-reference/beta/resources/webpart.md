---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574280"
---
# <a name="webpart-resource"></a><span data-ttu-id="72d72-102">веб-часть ресурсов</span><span class="sxs-lookup"><span data-stu-id="72d72-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d72-103">Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .</span><span class="sxs-lookup"><span data-stu-id="72d72-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="72d72-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72d72-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="72d72-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="72d72-105">Properties</span></span>

| <span data-ttu-id="72d72-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="72d72-106">Property</span></span>                | <span data-ttu-id="72d72-107">Тип</span><span class="sxs-lookup"><span data-stu-id="72d72-107">Type</span></span>             | <span data-ttu-id="72d72-108">Описание</span><span class="sxs-lookup"><span data-stu-id="72d72-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="72d72-109">**type**</span><span class="sxs-lookup"><span data-stu-id="72d72-109">**type**</span></span>                | <span data-ttu-id="72d72-110">String (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="72d72-110">String (identifier)</span></span>         | <span data-ttu-id="72d72-111">Уникальный идентификатор, определяющий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="72d72-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="72d72-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d72-112">Read-only.</span></span>
| <span data-ttu-id="72d72-113">**data**</span><span class="sxs-lookup"><span data-stu-id="72d72-113">**data**</span></span>                | [<span data-ttu-id="72d72-114">sitePageData</span><span class="sxs-lookup"><span data-stu-id="72d72-114">sitePageData</span></span>](sitepagedata.md) | <span data-ttu-id="72d72-115">Обязательные свойства для веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="72d72-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="72d72-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="72d72-116">Remarks</span></span>

<span data-ttu-id="72d72-117">Веб-части можно определить собственные необходимые свойства в области **данных**.</span><span class="sxs-lookup"><span data-stu-id="72d72-117">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="72d72-118">Дополнительные сведения о страницах можно [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="72d72-118">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
