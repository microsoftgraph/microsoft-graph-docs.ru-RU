---
title: Тип ресурсов attendeeAvailability
description: Тип и занятость участника.
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025227"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="a9c96-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="a9c96-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="a9c96-104">Тип и занятость участника.</span><span class="sxs-lookup"><span data-stu-id="a9c96-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9c96-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a9c96-105">JSON representation</span></span>

<span data-ttu-id="a9c96-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a9c96-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a9c96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9c96-107">Properties</span></span>
| <span data-ttu-id="a9c96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9c96-108">Property</span></span>     | <span data-ttu-id="a9c96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a9c96-109">Type</span></span>   |<span data-ttu-id="a9c96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a9c96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9c96-111">attendee</span><span class="sxs-lookup"><span data-stu-id="a9c96-111">attendee</span></span>|[<span data-ttu-id="a9c96-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="a9c96-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="a9c96-113">Тип участника (сведения о том, является ли участник пользователем или ресурсом, а также о том, обязательный ли он, если объект представляет пользователя).</span><span class="sxs-lookup"><span data-stu-id="a9c96-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="a9c96-114">availability</span><span class="sxs-lookup"><span data-stu-id="a9c96-114">availability</span></span>|<span data-ttu-id="a9c96-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="a9c96-115">freeBusyStatus</span></span>| <span data-ttu-id="a9c96-116">Состояние доступности участника.</span><span class="sxs-lookup"><span data-stu-id="a9c96-116">The availability status of the attendee.</span></span> <span data-ttu-id="a9c96-117">Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a9c96-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
