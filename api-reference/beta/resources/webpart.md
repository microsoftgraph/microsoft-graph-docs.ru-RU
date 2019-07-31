---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007356"
---
# <a name="webpart-resource"></a><span data-ttu-id="7cca0-103">ресурс webPart</span><span class="sxs-lookup"><span data-stu-id="7cca0-103">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cca0-104">Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="7cca0-104">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cca0-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cca0-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7cca0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cca0-106">Properties</span></span>

| <span data-ttu-id="7cca0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cca0-107">Property</span></span>                | <span data-ttu-id="7cca0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7cca0-108">Type</span></span>             | <span data-ttu-id="7cca0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7cca0-109">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="7cca0-110">**type**</span><span class="sxs-lookup"><span data-stu-id="7cca0-110">**type**</span></span>                | <span data-ttu-id="7cca0-111">String</span><span class="sxs-lookup"><span data-stu-id="7cca0-111">String</span></span>           | <span data-ttu-id="7cca0-112">Уникальный идентификатор, указывающий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="7cca0-112">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="7cca0-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7cca0-113">Read-only.</span></span>
| <span data-ttu-id="7cca0-114">**data**</span><span class="sxs-lookup"><span data-stu-id="7cca0-114">**data**</span></span>                | <span data-ttu-id="7cca0-115">[Ситепажедата][]</span><span class="sxs-lookup"><span data-stu-id="7cca0-115">[sitePageData][]</span></span> | <span data-ttu-id="7cca0-116">Обязательные свойства веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="7cca0-116">The required properties for the webPart (varies by webPart)</span></span>

[Ситепажедата]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="7cca0-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="7cca0-118">Remarks</span></span>

<span data-ttu-id="7cca0-119">Веб-части могут определять собственные обязательные свойства в разделе **Data**.</span><span class="sxs-lookup"><span data-stu-id="7cca0-119">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="7cca0-120">Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="7cca0-120">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
