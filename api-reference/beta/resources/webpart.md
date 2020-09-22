---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b69762298f4f165ac18e4e0137dd979bde176652
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973477"
---
# <a name="webpart-resource"></a><span data-ttu-id="86b06-103">ресурс webPart</span><span class="sxs-lookup"><span data-stu-id="86b06-103">webPart resource</span></span>

<span data-ttu-id="86b06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86b06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86b06-105">Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="86b06-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="86b06-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86b06-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="86b06-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86b06-107">Properties</span></span>

| <span data-ttu-id="86b06-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86b06-108">Property</span></span>                | <span data-ttu-id="86b06-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86b06-109">Type</span></span>             | <span data-ttu-id="86b06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86b06-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="86b06-111">**type**</span><span class="sxs-lookup"><span data-stu-id="86b06-111">**type**</span></span>                | <span data-ttu-id="86b06-112">String</span><span class="sxs-lookup"><span data-stu-id="86b06-112">String</span></span>           | <span data-ttu-id="86b06-113">Уникальный идентификатор, указывающий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="86b06-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="86b06-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86b06-114">Read-only.</span></span>
| <span data-ttu-id="86b06-115">**data**</span><span class="sxs-lookup"><span data-stu-id="86b06-115">**data**</span></span>                | <span data-ttu-id="86b06-116">[ситепажедата][]</span><span class="sxs-lookup"><span data-stu-id="86b06-116">[sitePageData][]</span></span> | <span data-ttu-id="86b06-117">Обязательные свойства веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="86b06-117">The required properties for the webPart (varies by webPart)</span></span>

[ситепажедата]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="86b06-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="86b06-119">Remarks</span></span>

<span data-ttu-id="86b06-120">Веб-части могут определять собственные обязательные свойства в разделе **Data**.</span><span class="sxs-lookup"><span data-stu-id="86b06-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="86b06-121">Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="86b06-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
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


