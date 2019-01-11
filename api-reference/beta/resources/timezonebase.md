---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
ms.openlocfilehash: 95d3409c40b3cc151f7b2f4b69580b9c1bbbe1ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882455"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="f5b65-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="f5b65-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="f5b65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5b65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5b65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5b65-106">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f5b65-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="f5b65-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5b65-107">Properties</span></span>
| <span data-ttu-id="f5b65-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5b65-108">Property</span></span>     | <span data-ttu-id="f5b65-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b65-109">Type</span></span>   |<span data-ttu-id="f5b65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b65-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5b65-111">name</span><span class="sxs-lookup"><span data-stu-id="f5b65-111">name</span></span> | <span data-ttu-id="f5b65-112">строка</span><span class="sxs-lookup"><span data-stu-id="f5b65-112">string</span></span> | <span data-ttu-id="f5b65-113">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="f5b65-113">The name of a time zone.</span></span> <span data-ttu-id="f5b65-114">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="f5b65-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f5b65-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5b65-115">JSON representation</span></span>

<span data-ttu-id="f5b65-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5b65-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
