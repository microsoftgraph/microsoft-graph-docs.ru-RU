---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453611"
---
# <a name="webpart-resource"></a><span data-ttu-id="2bd15-102">ресурс webPart</span><span class="sxs-lookup"><span data-stu-id="2bd15-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bd15-103">Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="2bd15-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bd15-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bd15-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2bd15-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bd15-105">Properties</span></span>

| <span data-ttu-id="2bd15-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bd15-106">Property</span></span>                | <span data-ttu-id="2bd15-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2bd15-107">Type</span></span>             | <span data-ttu-id="2bd15-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2bd15-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="2bd15-109">**type**</span><span class="sxs-lookup"><span data-stu-id="2bd15-109">**type**</span></span>                | <span data-ttu-id="2bd15-110">Строка</span><span class="sxs-lookup"><span data-stu-id="2bd15-110">String</span></span>           | <span data-ttu-id="2bd15-111">Уникальный идентификатор, указывающий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="2bd15-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="2bd15-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2bd15-112">Read-only.</span></span>
| <span data-ttu-id="2bd15-113">**data**</span><span class="sxs-lookup"><span data-stu-id="2bd15-113">**data**</span></span>                | <span data-ttu-id="2bd15-114">[Ситепажедата][]</span><span class="sxs-lookup"><span data-stu-id="2bd15-114">[sitePageData][]</span></span> | <span data-ttu-id="2bd15-115">Обязательные свойства веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="2bd15-115">The required properties for the webPart (varies by webPart)</span></span>

[Ситепажедата]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="2bd15-117">Комментарии</span><span class="sxs-lookup"><span data-stu-id="2bd15-117">Remarks</span></span>

<span data-ttu-id="2bd15-118">Веб-части могут определять собственные обязательные свойства в разделе **Data**.</span><span class="sxs-lookup"><span data-stu-id="2bd15-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="2bd15-119">Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="2bd15-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
