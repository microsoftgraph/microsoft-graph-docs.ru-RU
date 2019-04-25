---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535615"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="b9db5-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="b9db5-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9db5-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="b9db5-104">The type of attendee.</span></span>

<span data-ttu-id="b9db5-105">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="b9db5-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9db5-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9db5-106">JSON representation</span></span>

<span data-ttu-id="b9db5-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b9db5-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="b9db5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9db5-108">Properties</span></span>
| <span data-ttu-id="b9db5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9db5-109">Property</span></span>     | <span data-ttu-id="b9db5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b9db5-110">Type</span></span>   |<span data-ttu-id="b9db5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9db5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9db5-112">type</span><span class="sxs-lookup"><span data-stu-id="b9db5-112">type</span></span>|<span data-ttu-id="b9db5-113">String</span><span class="sxs-lookup"><span data-stu-id="b9db5-113">String</span></span>| <span data-ttu-id="b9db5-p101">Тип участника. Возможные значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="b9db5-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="b9db5-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b9db5-117">emailAddress</span></span>|[<span data-ttu-id="b9db5-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b9db5-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b9db5-119">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="b9db5-119">Includes the name and SMTP address of the attendee.</span></span>|

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
