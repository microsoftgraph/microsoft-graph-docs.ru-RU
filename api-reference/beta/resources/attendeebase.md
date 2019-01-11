---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
ms.openlocfilehash: b30e054e6d89765d280340b31355403739381c2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844984"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="b908f-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="b908f-103">attendeeBase resource type</span></span>

> <span data-ttu-id="b908f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b908f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b908f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b908f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b908f-106">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="b908f-106">The type of attendee.</span></span>

<span data-ttu-id="b908f-107">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="b908f-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b908f-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b908f-108">JSON representation</span></span>

<span data-ttu-id="b908f-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b908f-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b908f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b908f-110">Properties</span></span>
| <span data-ttu-id="b908f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b908f-111">Property</span></span>     | <span data-ttu-id="b908f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b908f-112">Type</span></span>   |<span data-ttu-id="b908f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b908f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b908f-114">type</span><span class="sxs-lookup"><span data-stu-id="b908f-114">type</span></span>|<span data-ttu-id="b908f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b908f-115">String</span></span>| <span data-ttu-id="b908f-p102">Тип участника. Возможные значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="b908f-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="b908f-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b908f-119">emailAddress</span></span>|[<span data-ttu-id="b908f-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b908f-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b908f-121">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="b908f-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
