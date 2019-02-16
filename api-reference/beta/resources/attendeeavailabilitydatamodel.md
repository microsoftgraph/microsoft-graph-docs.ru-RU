---
title: Тип ресурса Аттендиаваилабилитидатамодел
description: Тип и занятость участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6d7436a640b4aaba0a9b71ef62ee91b3fe0d7cee
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057418"
---
# <a name="attendeeavailabilitydatamodel-resource-type"></a><span data-ttu-id="bd1f4-103">Тип ресурса Аттендиаваилабилитидатамодел</span><span class="sxs-lookup"><span data-stu-id="bd1f4-103">attendeeAvailabilityDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd1f4-104">Представляет пользователя или ресурс, а также их доступность для собрания.</span><span class="sxs-lookup"><span data-stu-id="bd1f4-104">Represents a person or resource and their availability for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd1f4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd1f4-105">JSON representation</span></span>

<span data-ttu-id="bd1f4-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd1f4-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailabilityDataModel"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeDataModel"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="bd1f4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd1f4-107">Properties</span></span>
| <span data-ttu-id="bd1f4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd1f4-108">Property</span></span>     | <span data-ttu-id="bd1f4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bd1f4-109">Type</span></span>   |<span data-ttu-id="bd1f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd1f4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd1f4-111">attendee</span><span class="sxs-lookup"><span data-stu-id="bd1f4-111">attendee</span></span>|[<span data-ttu-id="bd1f4-112">Аттендидатамодел</span><span class="sxs-lookup"><span data-stu-id="bd1f4-112">attendeeDataModel</span></span>](attendeedatamodel.md)|<span data-ttu-id="bd1f4-113">Представляет сведения о лице или ресурсе, а также о том, является ли участник обязательным или необязательным для собрания.</span><span class="sxs-lookup"><span data-stu-id="bd1f4-113">Represents a person or resource attendee and whether the attendee is required or optional for the meeting.</span></span>|
|<span data-ttu-id="bd1f4-114">availability</span><span class="sxs-lookup"><span data-stu-id="bd1f4-114">availability</span></span>|<span data-ttu-id="bd1f4-115">availabilityStatus</span><span class="sxs-lookup"><span data-stu-id="bd1f4-115">availabilityStatus</span></span>| <span data-ttu-id="bd1f4-116">Состояние доступности участника.</span><span class="sxs-lookup"><span data-stu-id="bd1f4-116">The availability status of the attendee.</span></span> <span data-ttu-id="bd1f4-117">Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="bd1f4-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailabilityDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailabilitydatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->