---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345795"
---
# <a name="webpart-resource"></a><span data-ttu-id="b7484-102">ресурс webPart</span><span class="sxs-lookup"><span data-stu-id="b7484-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7484-103">Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="b7484-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7484-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7484-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a><span data-ttu-id="b7484-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7484-105">Properties</span></span>

| <span data-ttu-id="b7484-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7484-106">Property</span></span>                | <span data-ttu-id="b7484-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b7484-107">Type</span></span>             | <span data-ttu-id="b7484-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b7484-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="b7484-109">**type**</span><span class="sxs-lookup"><span data-stu-id="b7484-109">**type**</span></span>                | <span data-ttu-id="b7484-110">String</span><span class="sxs-lookup"><span data-stu-id="b7484-110">String</span></span>           | <span data-ttu-id="b7484-111">Уникальный идентификатор, указывающий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="b7484-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="b7484-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7484-112">Read-only.</span></span>
| <span data-ttu-id="b7484-113">**data**</span><span class="sxs-lookup"><span data-stu-id="b7484-113">**data**</span></span>                | <span data-ttu-id="b7484-114">[Ситепажедата][]</span><span class="sxs-lookup"><span data-stu-id="b7484-114">[sitePageData][]</span></span> | <span data-ttu-id="b7484-115">Обязательные свойства веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="b7484-115">The required properties for the webPart (varies by webPart)</span></span>

[Ситепажедата]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="b7484-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="b7484-117">Remarks</span></span>

<span data-ttu-id="b7484-118">Веб-части могут определять собственные обязательные свойства в разделе **Data**.</span><span class="sxs-lookup"><span data-stu-id="b7484-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="b7484-119">Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="b7484-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
