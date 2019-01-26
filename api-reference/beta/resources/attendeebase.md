---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
ms.openlocfilehash: 6ec80f5505cb3dd742a2690ebb3cd5374635770d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572740"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="2af49-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="2af49-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2af49-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="2af49-104">The type of attendee.</span></span>

<span data-ttu-id="2af49-105">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="2af49-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2af49-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2af49-106">JSON representation</span></span>

<span data-ttu-id="2af49-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2af49-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="2af49-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2af49-108">Properties</span></span>
| <span data-ttu-id="2af49-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2af49-109">Property</span></span>     | <span data-ttu-id="2af49-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2af49-110">Type</span></span>   |<span data-ttu-id="2af49-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2af49-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2af49-112">type</span><span class="sxs-lookup"><span data-stu-id="2af49-112">type</span></span>|<span data-ttu-id="2af49-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="2af49-113">attendeeType</span></span>| <span data-ttu-id="2af49-114">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="2af49-114">The type of attendee.</span></span> <span data-ttu-id="2af49-115">Возможные значения: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="2af49-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="2af49-116">В настоящее время Если участник — это пользователь, [findMeetingTimes](../api/user-findmeetingtimes.md) всегда считает пользователя принадлежит `Required` типа.</span><span class="sxs-lookup"><span data-stu-id="2af49-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="2af49-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2af49-117">emailAddress</span></span>|[<span data-ttu-id="2af49-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2af49-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="2af49-119">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="2af49-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
