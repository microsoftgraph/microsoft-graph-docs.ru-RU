---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
ms.openlocfilehash: 4c112a3118bf3f4d00be790d7923bc0fe82dc72f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456954"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="cb4c2-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="cb4c2-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb4c2-104">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="cb4c2-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="cb4c2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb4c2-105">Properties</span></span>
| <span data-ttu-id="cb4c2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb4c2-106">Property</span></span>     | <span data-ttu-id="cb4c2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb4c2-107">Type</span></span>   |<span data-ttu-id="cb4c2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cb4c2-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cb4c2-109">name</span><span class="sxs-lookup"><span data-stu-id="cb4c2-109">name</span></span> | <span data-ttu-id="cb4c2-110">string</span><span class="sxs-lookup"><span data-stu-id="cb4c2-110">string</span></span> | <span data-ttu-id="cb4c2-111">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="cb4c2-111">The name of a time zone.</span></span> <span data-ttu-id="cb4c2-112">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="cb4c2-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cb4c2-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb4c2-113">JSON representation</span></span>

<span data-ttu-id="cb4c2-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb4c2-114">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/timezonebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
