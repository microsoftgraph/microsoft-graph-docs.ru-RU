---
title: Тип ресурса followupFlag
description: Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже. К поддерживаемым элементам относятся message и contact.
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869380"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="0f977-104">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="0f977-104">followupFlag resource type</span></span>

> <span data-ttu-id="0f977-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f977-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f977-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f977-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f977-107">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="0f977-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="0f977-108">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="0f977-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f977-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f977-109">Properties</span></span>
| <span data-ttu-id="0f977-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f977-110">Property</span></span>     | <span data-ttu-id="0f977-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0f977-111">Type</span></span>   |<span data-ttu-id="0f977-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0f977-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f977-113">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f977-113">completedDateTime</span></span>|[<span data-ttu-id="0f977-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0f977-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0f977-115">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="0f977-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0f977-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0f977-116">dueDateTime</span></span>|<span data-ttu-id="0f977-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0f977-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0f977-118">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="0f977-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="0f977-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0f977-119">flagStatus</span></span>|<span data-ttu-id="0f977-120">String</span><span class="sxs-lookup"><span data-stu-id="0f977-120">String</span></span>|<span data-ttu-id="0f977-121">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="0f977-121">The status for follow-up for an item.</span></span> <span data-ttu-id="0f977-122">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="0f977-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0f977-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f977-123">startDateTime</span></span>|<span data-ttu-id="0f977-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0f977-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0f977-125">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="0f977-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f977-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f977-126">JSON representation</span></span>

<span data-ttu-id="0f977-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f977-127">Here is a JSON representation of the resource</span></span>

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
