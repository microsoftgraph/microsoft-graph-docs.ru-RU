---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
ms.openlocfilehash: a0095a2076cd09bee2d4b934bac29cd030924ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328592"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="59131-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="59131-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59131-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="59131-104">The type of attendee.</span></span>

<span data-ttu-id="59131-105">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="59131-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="59131-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59131-106">JSON representation</span></span>

<span data-ttu-id="59131-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="59131-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="59131-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59131-108">Properties</span></span>
| <span data-ttu-id="59131-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="59131-109">Property</span></span>     | <span data-ttu-id="59131-110">Тип</span><span class="sxs-lookup"><span data-stu-id="59131-110">Type</span></span>   |<span data-ttu-id="59131-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59131-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59131-112">type</span><span class="sxs-lookup"><span data-stu-id="59131-112">type</span></span>|<span data-ttu-id="59131-113">String</span><span class="sxs-lookup"><span data-stu-id="59131-113">String</span></span>| <span data-ttu-id="59131-p101">Тип участника. Возможные значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="59131-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="59131-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59131-117">emailAddress</span></span>|[<span data-ttu-id="59131-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59131-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="59131-119">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="59131-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
