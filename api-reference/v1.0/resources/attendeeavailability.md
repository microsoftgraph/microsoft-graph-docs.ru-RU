---
title: Тип ресурсов attendeeAvailability
description: Тип и занятость участника.
localization_priority: Normal
ms.openlocfilehash: a6dee994fc5eb3786fc1a432adcb9333bdb56ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834750"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="2eb67-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="2eb67-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="2eb67-104">Тип и занятость участника.</span><span class="sxs-lookup"><span data-stu-id="2eb67-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2eb67-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2eb67-105">JSON representation</span></span>

<span data-ttu-id="2eb67-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2eb67-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2eb67-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2eb67-107">Properties</span></span>
| <span data-ttu-id="2eb67-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eb67-108">Property</span></span>     | <span data-ttu-id="2eb67-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb67-109">Type</span></span>   |<span data-ttu-id="2eb67-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb67-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2eb67-111">attendee</span><span class="sxs-lookup"><span data-stu-id="2eb67-111">attendee</span></span>|[<span data-ttu-id="2eb67-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="2eb67-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="2eb67-113">Тип участника (сведения о том, является ли участник пользователем или ресурсом, а также о том, обязательный ли он, если объект представляет пользователя).</span><span class="sxs-lookup"><span data-stu-id="2eb67-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="2eb67-114">availability</span><span class="sxs-lookup"><span data-stu-id="2eb67-114">availability</span></span>|<span data-ttu-id="2eb67-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2eb67-115">freeBusyStatus</span></span>| <span data-ttu-id="2eb67-116">Состояние доступности участника.</span><span class="sxs-lookup"><span data-stu-id="2eb67-116">The availability status of the attendee.</span></span> <span data-ttu-id="2eb67-117">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2eb67-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
