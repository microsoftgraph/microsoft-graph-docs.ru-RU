---
title: Тип ресурсов attendeeBase
description: Тип участника.
ms.openlocfilehash: 2d7d3889cd65886eba4cf9356862417928ed3296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074810"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="ff606-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="ff606-103">attendeeBase resource type</span></span>

> <span data-ttu-id="ff606-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff606-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff606-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff606-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff606-106">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="ff606-106">The type of attendee.</span></span>

<span data-ttu-id="ff606-107">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="ff606-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff606-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff606-108">JSON representation</span></span>

<span data-ttu-id="ff606-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ff606-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ff606-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff606-110">Properties</span></span>
| <span data-ttu-id="ff606-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff606-111">Property</span></span>     | <span data-ttu-id="ff606-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ff606-112">Type</span></span>   |<span data-ttu-id="ff606-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ff606-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff606-114">type</span><span class="sxs-lookup"><span data-stu-id="ff606-114">type</span></span>|<span data-ttu-id="ff606-115">String</span><span class="sxs-lookup"><span data-stu-id="ff606-115">String</span></span>| <span data-ttu-id="ff606-p102">Тип участника. Возможные значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="ff606-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="ff606-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ff606-119">emailAddress</span></span>|[<span data-ttu-id="ff606-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ff606-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ff606-121">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="ff606-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->