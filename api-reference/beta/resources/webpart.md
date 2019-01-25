---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510241"
---
# <a name="webpart-resource"></a><span data-ttu-id="7c3ff-102">веб-часть ресурсов</span><span class="sxs-lookup"><span data-stu-id="7c3ff-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3ff-103">Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .</span><span class="sxs-lookup"><span data-stu-id="7c3ff-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c3ff-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c3ff-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="7c3ff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c3ff-105">Properties</span></span>

| <span data-ttu-id="7c3ff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c3ff-106">Property</span></span>                | <span data-ttu-id="7c3ff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7c3ff-107">Type</span></span>             | <span data-ttu-id="7c3ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c3ff-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="7c3ff-109">**type**</span><span class="sxs-lookup"><span data-stu-id="7c3ff-109">**type**</span></span>                | <span data-ttu-id="7c3ff-110">String</span><span class="sxs-lookup"><span data-stu-id="7c3ff-110">String</span></span>           | <span data-ttu-id="7c3ff-111">Уникальный идентификатор, определяющий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="7c3ff-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="7c3ff-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c3ff-112">Read-only.</span></span>
| <span data-ttu-id="7c3ff-113">**data**</span><span class="sxs-lookup"><span data-stu-id="7c3ff-113">**data**</span></span>                | <span data-ttu-id="7c3ff-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="7c3ff-114">[sitePageData][]</span></span> | <span data-ttu-id="7c3ff-115">Обязательные свойства для веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="7c3ff-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="7c3ff-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c3ff-117">Remarks</span></span>

<span data-ttu-id="7c3ff-118">Веб-части можно определить собственные необходимые свойства в области **данных**.</span><span class="sxs-lookup"><span data-stu-id="7c3ff-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="7c3ff-119">Дополнительные сведения о страницах можно [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="7c3ff-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
