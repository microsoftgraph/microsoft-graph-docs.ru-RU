---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f1487523d89dc6677f2fc04b62013e7db9602b92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508138"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="bb423-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="bb423-103">attendeeBase resource type</span></span>

<span data-ttu-id="bb423-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb423-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb423-105">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="bb423-105">The type of attendee.</span></span>

<span data-ttu-id="bb423-106">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="bb423-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb423-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb423-107">JSON representation</span></span>

<span data-ttu-id="bb423-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb423-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bb423-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb423-109">Properties</span></span>
| <span data-ttu-id="bb423-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb423-110">Property</span></span>     | <span data-ttu-id="bb423-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bb423-111">Type</span></span>   |<span data-ttu-id="bb423-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bb423-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb423-113">type</span><span class="sxs-lookup"><span data-stu-id="bb423-113">type</span></span>|<span data-ttu-id="bb423-114">String</span><span class="sxs-lookup"><span data-stu-id="bb423-114">String</span></span>| <span data-ttu-id="bb423-p101">Тип участника. Возможные значения: `required`, `optional`, `resource`. Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="bb423-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="bb423-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb423-118">emailAddress</span></span>|[<span data-ttu-id="bb423-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb423-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="bb423-120">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="bb423-120">Includes the name and SMTP address of the attendee.</span></span>|

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
