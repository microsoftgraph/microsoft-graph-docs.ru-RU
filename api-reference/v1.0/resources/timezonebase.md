---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4ddc8b01f494ee861d3ab50583dc12ea4c68c623
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033574"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="4a026-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="4a026-103">timeZoneBase resource type</span></span>

<span data-ttu-id="4a026-104">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4a026-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="4a026-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a026-105">Properties</span></span>
| <span data-ttu-id="4a026-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a026-106">Property</span></span>     | <span data-ttu-id="4a026-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4a026-107">Type</span></span>   |<span data-ttu-id="4a026-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4a026-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a026-109">name</span><span class="sxs-lookup"><span data-stu-id="4a026-109">name</span></span> | <span data-ttu-id="4a026-110">string</span><span class="sxs-lookup"><span data-stu-id="4a026-110">string</span></span> | <span data-ttu-id="4a026-111">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="4a026-111">The name of a time zone.</span></span> <span data-ttu-id="4a026-112">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="4a026-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4a026-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a026-113">JSON representation</span></span>

<span data-ttu-id="4a026-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a026-114">Here is a JSON representation of the resource.</span></span>

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
