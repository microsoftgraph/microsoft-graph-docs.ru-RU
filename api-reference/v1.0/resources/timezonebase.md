---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
ms.openlocfilehash: 4c112a3118bf3f4d00be790d7923bc0fe82dc72f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860636"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="c6d53-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="c6d53-103">timeZoneBase resource type</span></span>

<span data-ttu-id="c6d53-104">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="c6d53-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="c6d53-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6d53-105">Properties</span></span>
| <span data-ttu-id="c6d53-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6d53-106">Property</span></span>     | <span data-ttu-id="c6d53-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c6d53-107">Type</span></span>   |<span data-ttu-id="c6d53-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c6d53-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6d53-109">name</span><span class="sxs-lookup"><span data-stu-id="c6d53-109">name</span></span> | <span data-ttu-id="c6d53-110">строка</span><span class="sxs-lookup"><span data-stu-id="c6d53-110">string</span></span> | <span data-ttu-id="c6d53-111">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="c6d53-111">The name of a time zone.</span></span> <span data-ttu-id="c6d53-112">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="c6d53-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c6d53-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6d53-113">JSON representation</span></span>

<span data-ttu-id="c6d53-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6d53-114">Here is a JSON representation of the resource.</span></span>

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
