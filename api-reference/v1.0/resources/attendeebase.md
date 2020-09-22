---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59e1aa072d511c575bb6911e19387de753d47bee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988550"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="bb187-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="bb187-103">attendeeBase resource type</span></span>

<span data-ttu-id="bb187-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb187-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb187-105">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="bb187-105">The type of attendee.</span></span>

<span data-ttu-id="bb187-106">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="bb187-106">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb187-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb187-107">JSON representation</span></span>

<span data-ttu-id="bb187-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb187-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bb187-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb187-109">Properties</span></span>
| <span data-ttu-id="bb187-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb187-110">Property</span></span>     | <span data-ttu-id="bb187-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bb187-111">Type</span></span>   |<span data-ttu-id="bb187-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bb187-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb187-113">type</span><span class="sxs-lookup"><span data-stu-id="bb187-113">type</span></span>|<span data-ttu-id="bb187-114">attendeeType</span><span class="sxs-lookup"><span data-stu-id="bb187-114">attendeeType</span></span>| <span data-ttu-id="bb187-115">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="bb187-115">The type of attendee.</span></span> <span data-ttu-id="bb187-116">Допустимые значения: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="bb187-116">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="bb187-117">Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="bb187-117">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="bb187-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb187-118">emailAddress</span></span>|[<span data-ttu-id="bb187-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb187-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="bb187-120">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="bb187-120">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

