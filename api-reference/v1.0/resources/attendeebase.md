---
title: Тип ресурсов attendeeBase
description: Тип участника.
ms.openlocfilehash: 6995ac94a600a60313ef26208b441c6ef6fdf001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027022"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="16d4a-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="16d4a-103">attendeeBase resource type</span></span>

<span data-ttu-id="16d4a-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="16d4a-104">The type of attendee.</span></span>

<span data-ttu-id="16d4a-105">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="16d4a-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="16d4a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16d4a-106">JSON representation</span></span>

<span data-ttu-id="16d4a-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="16d4a-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="16d4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="16d4a-108">Properties</span></span>
| <span data-ttu-id="16d4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="16d4a-109">Property</span></span>     | <span data-ttu-id="16d4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="16d4a-110">Type</span></span>   |<span data-ttu-id="16d4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16d4a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16d4a-112">type</span><span class="sxs-lookup"><span data-stu-id="16d4a-112">type</span></span>|<span data-ttu-id="16d4a-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="16d4a-113">attendeeType</span></span>| <span data-ttu-id="16d4a-114">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="16d4a-114">The type of attendee.</span></span> <span data-ttu-id="16d4a-115">Возможные значения: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="16d4a-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="16d4a-116">В настоящее время Если участник — это пользователь, [findMeetingTimes](../api/user-findmeetingtimes.md) всегда считает пользователя принадлежит `Required` типа.</span><span class="sxs-lookup"><span data-stu-id="16d4a-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="16d4a-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="16d4a-117">emailAddress</span></span>|[<span data-ttu-id="16d4a-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="16d4a-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="16d4a-119">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="16d4a-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
