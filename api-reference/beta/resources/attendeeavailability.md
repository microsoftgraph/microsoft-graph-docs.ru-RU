---
title: Тип ресурсов attendeeAvailability
description: Тип и занятость участника.
localization_priority: Normal
ms.openlocfilehash: 37b344f110557d6e04129a2b93592009635bddcf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576285"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="f12f5-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="f12f5-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f12f5-104">Тип и занятость участника.</span><span class="sxs-lookup"><span data-stu-id="f12f5-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f12f5-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f12f5-105">JSON representation</span></span>

<span data-ttu-id="f12f5-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f12f5-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="f12f5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f12f5-107">Properties</span></span>
| <span data-ttu-id="f12f5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f12f5-108">Property</span></span>     | <span data-ttu-id="f12f5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f12f5-109">Type</span></span>   |<span data-ttu-id="f12f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f12f5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f12f5-111">attendee</span><span class="sxs-lookup"><span data-stu-id="f12f5-111">attendee</span></span>|[<span data-ttu-id="f12f5-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="f12f5-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="f12f5-113">Тип участника (сведения о том, является ли участник пользователем или ресурсом, а также о том, обязательный ли он, если объект представляет пользователя).</span><span class="sxs-lookup"><span data-stu-id="f12f5-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="f12f5-114">availability</span><span class="sxs-lookup"><span data-stu-id="f12f5-114">availability</span></span>|<span data-ttu-id="f12f5-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f12f5-115">freeBusyStatus</span></span>| <span data-ttu-id="f12f5-116">Состояние доступности участника.</span><span class="sxs-lookup"><span data-stu-id="f12f5-116">The availability status of the attendee.</span></span> <span data-ttu-id="f12f5-117">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f12f5-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
