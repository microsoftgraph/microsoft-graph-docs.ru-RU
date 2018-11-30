---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077810"
---
# <a name="webpart-resource"></a><span data-ttu-id="5b905-102">веб-часть ресурсов</span><span class="sxs-lookup"><span data-stu-id="5b905-102">webPart resource</span></span>

> <span data-ttu-id="5b905-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b905-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b905-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b905-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b905-105">Тип и отображение сведений о веб-части на [sitePage](sitepage.md)представляет ресурс **веб-части** .</span><span class="sxs-lookup"><span data-stu-id="5b905-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b905-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b905-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5b905-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b905-107">Properties</span></span>

| <span data-ttu-id="5b905-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b905-108">Property</span></span>                | <span data-ttu-id="5b905-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b905-109">Type</span></span>             | <span data-ttu-id="5b905-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b905-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="5b905-111">**type**</span><span class="sxs-lookup"><span data-stu-id="5b905-111">**type**</span></span>                | <span data-ttu-id="5b905-112">String</span><span class="sxs-lookup"><span data-stu-id="5b905-112">String</span></span>           | <span data-ttu-id="5b905-113">Уникальный идентификатор, определяющий тип веб-части.</span><span class="sxs-lookup"><span data-stu-id="5b905-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="5b905-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b905-114">Read-only.</span></span>
| <span data-ttu-id="5b905-115">**data**</span><span class="sxs-lookup"><span data-stu-id="5b905-115">**data**</span></span>                | <span data-ttu-id="5b905-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="5b905-116">[sitePageData][]</span></span> | <span data-ttu-id="5b905-117">Обязательные свойства для веб-части (зависит от веб-части)</span><span class="sxs-lookup"><span data-stu-id="5b905-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="5b905-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="5b905-119">Remarks</span></span>

<span data-ttu-id="5b905-120">Веб-части можно определить собственные необходимые свойства в области **данных**.</span><span class="sxs-lookup"><span data-stu-id="5b905-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="5b905-121">Дополнительные сведения о страницах можно [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="5b905-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
