---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341871"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="f9bbe-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="f9bbe-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9bbe-104">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f9bbe-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="f9bbe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9bbe-105">Properties</span></span>
| <span data-ttu-id="f9bbe-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9bbe-106">Property</span></span>     | <span data-ttu-id="f9bbe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f9bbe-107">Type</span></span>   |<span data-ttu-id="f9bbe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f9bbe-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9bbe-109">name</span><span class="sxs-lookup"><span data-stu-id="f9bbe-109">name</span></span> | <span data-ttu-id="f9bbe-110">string</span><span class="sxs-lookup"><span data-stu-id="f9bbe-110">string</span></span> | <span data-ttu-id="f9bbe-111">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="f9bbe-111">The name of a time zone.</span></span> <span data-ttu-id="f9bbe-112">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="f9bbe-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f9bbe-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9bbe-113">JSON representation</span></span>

<span data-ttu-id="f9bbe-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9bbe-114">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
