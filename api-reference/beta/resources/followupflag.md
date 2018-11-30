---
title: Тип ресурса followupFlag
description: Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже. К поддерживаемым элементам относятся message и contact.
ms.openlocfilehash: a996bc05e5297149e587d7372e989580146c1fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079013"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="d00cc-104">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="d00cc-104">followupFlag resource type</span></span>

> <span data-ttu-id="d00cc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d00cc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d00cc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d00cc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d00cc-107">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="d00cc-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="d00cc-108">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="d00cc-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d00cc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d00cc-109">Properties</span></span>
| <span data-ttu-id="d00cc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d00cc-110">Property</span></span>     | <span data-ttu-id="d00cc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d00cc-111">Type</span></span>   |<span data-ttu-id="d00cc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d00cc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d00cc-113">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d00cc-113">completedDateTime</span></span>|[<span data-ttu-id="d00cc-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d00cc-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d00cc-115">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="d00cc-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="d00cc-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d00cc-116">dueDateTime</span></span>|<span data-ttu-id="d00cc-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d00cc-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d00cc-118">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="d00cc-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="d00cc-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="d00cc-119">flagStatus</span></span>|<span data-ttu-id="d00cc-120">String</span><span class="sxs-lookup"><span data-stu-id="d00cc-120">String</span></span>|<span data-ttu-id="d00cc-121">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="d00cc-121">The status for follow-up for an item.</span></span> <span data-ttu-id="d00cc-122">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="d00cc-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="d00cc-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d00cc-123">startDateTime</span></span>|<span data-ttu-id="d00cc-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d00cc-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d00cc-125">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="d00cc-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d00cc-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d00cc-126">JSON representation</span></span>

<span data-ttu-id="d00cc-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d00cc-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
