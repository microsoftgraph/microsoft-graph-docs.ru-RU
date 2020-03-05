---
author: rahmit
description: Ресурс webPart представляет тип и сведения о визуализации веб-части в Ситепаже.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: efcf6aa1db31246af607cda85aa799fcc6804a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519437"
---
# <a name="webpart-resource"></a><span data-ttu-id="38319-103">ресурс webPart</span><span class="sxs-lookup"><span data-stu-id="38319-103">webPart resource</span></span>

<span data-ttu-id="38319-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38319-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38319-105">Ресурс **WebPart** представляет тип и сведения о визуализации веб-части в [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="38319-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="38319-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38319-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="38319-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="38319-107">Properties</span></span>

| <span data-ttu-id="38319-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="38319-108">Property</span></span>                | <span data-ttu-id="38319-109">Тип</span><span class="sxs-lookup"><span data-stu-id="38319-109">Type</span></span>             | <span data-ttu-id="38319-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38319-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="38319-111">**type**</span><span class="sxs-lookup"><span data-stu-id="38319-111">**type**</span></span>                | <span data-ttu-id="38319-112">String</span><span class="sxs-lookup"><span data-stu-id="38319-112">String</span></span>           | <span data-ttu-id="38319-113">Уникальный идентификатор, указывающий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="38319-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="38319-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38319-114">Read-only.</span></span>
| <span data-ttu-id="38319-115">**data**</span><span class="sxs-lookup"><span data-stu-id="38319-115">**data**</span></span>                | <span data-ttu-id="38319-116">[ситепажедата][]</span><span class="sxs-lookup"><span data-stu-id="38319-116">[sitePageData][]</span></span> | <span data-ttu-id="38319-117">Обязательные свойства веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="38319-117">The required properties for the webPart (varies by webPart)</span></span>

[ситепажедата]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="38319-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="38319-119">Remarks</span></span>

<span data-ttu-id="38319-120">Веб-части могут определять собственные обязательные свойства в разделе **Data**.</span><span class="sxs-lookup"><span data-stu-id="38319-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="38319-121">Более подробную информацию о страницах можно узнать в статье [ситепаже](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="38319-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
