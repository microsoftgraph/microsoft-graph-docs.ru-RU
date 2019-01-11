---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.openlocfilehash: f7293b986b5e6d77d0601cffb6b60edc5dfd2dd7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856030"
---
# <a name="webpart-resource"></a><span data-ttu-id="adc78-102">веб-часть ресурсов</span><span class="sxs-lookup"><span data-stu-id="adc78-102">webPart resource</span></span>

> <span data-ttu-id="adc78-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="adc78-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adc78-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adc78-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adc78-105">Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .</span><span class="sxs-lookup"><span data-stu-id="adc78-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="adc78-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adc78-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="adc78-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="adc78-107">Properties</span></span>

| <span data-ttu-id="adc78-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="adc78-108">Property</span></span>                | <span data-ttu-id="adc78-109">Тип</span><span class="sxs-lookup"><span data-stu-id="adc78-109">Type</span></span>             | <span data-ttu-id="adc78-110">Описание</span><span class="sxs-lookup"><span data-stu-id="adc78-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="adc78-111">**type**</span><span class="sxs-lookup"><span data-stu-id="adc78-111">**type**</span></span>                | <span data-ttu-id="adc78-112">Строка</span><span class="sxs-lookup"><span data-stu-id="adc78-112">String</span></span>           | <span data-ttu-id="adc78-113">Уникальный идентификатор, определяющий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="adc78-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="adc78-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adc78-114">Read-only.</span></span>
| <span data-ttu-id="adc78-115">**data**</span><span class="sxs-lookup"><span data-stu-id="adc78-115">**data**</span></span>                | <span data-ttu-id="adc78-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="adc78-116">[sitePageData][]</span></span> | <span data-ttu-id="adc78-117">Обязательные свойства для веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="adc78-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="adc78-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="adc78-119">Remarks</span></span>

<span data-ttu-id="adc78-120">Веб-части можно определить собственные необходимые свойства в области **данных**.</span><span class="sxs-lookup"><span data-stu-id="adc78-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="adc78-121">Дополнительные сведения о страницах можно [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="adc78-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
