---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
ms.openlocfilehash: 18df657ab561163b64bcf224f8902f2ba7e0039c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026497"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="398b9-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="398b9-103">timeZoneBase resource type</span></span>

<span data-ttu-id="398b9-104">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="398b9-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="398b9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="398b9-105">Properties</span></span>
| <span data-ttu-id="398b9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="398b9-106">Property</span></span>     | <span data-ttu-id="398b9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="398b9-107">Type</span></span>   |<span data-ttu-id="398b9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="398b9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="398b9-109">name</span><span class="sxs-lookup"><span data-stu-id="398b9-109">name</span></span> | <span data-ttu-id="398b9-110">строка</span><span class="sxs-lookup"><span data-stu-id="398b9-110">string</span></span> | <span data-ttu-id="398b9-111">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="398b9-111">The name of a time zone.</span></span> <span data-ttu-id="398b9-112">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="398b9-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="398b9-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="398b9-113">JSON representation</span></span>

<span data-ttu-id="398b9-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="398b9-114">Here is a JSON representation of the resource.</span></span>

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