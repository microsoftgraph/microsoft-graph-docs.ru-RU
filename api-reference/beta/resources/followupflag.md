---
title: Тип ресурса followupFlag
description: Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже. К поддерживаемым элементам относятся message и contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 4d075b36cf06db3d4c470ece46229c05c44949af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129459"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="3e230-104">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="3e230-104">followupFlag resource type</span></span>

<span data-ttu-id="3e230-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e230-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e230-106">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="3e230-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="3e230-107">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="3e230-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e230-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e230-108">Properties</span></span>
| <span data-ttu-id="3e230-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e230-109">Property</span></span>     | <span data-ttu-id="3e230-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e230-110">Type</span></span>   |<span data-ttu-id="3e230-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e230-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e230-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e230-112">completedDateTime</span></span>|[<span data-ttu-id="3e230-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e230-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e230-114">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="3e230-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="3e230-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="3e230-115">dueDateTime</span></span>|<span data-ttu-id="3e230-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="3e230-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="3e230-117">Дата и время завершения последующего действия.</span><span class="sxs-lookup"><span data-stu-id="3e230-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="3e230-118">**Примечание.** Чтобы задать дату окончания, необходимо также указать; в противном случае вы `startDateTime` получите `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="3e230-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="3e230-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="3e230-119">flagStatus</span></span>|<span data-ttu-id="3e230-120">String</span><span class="sxs-lookup"><span data-stu-id="3e230-120">String</span></span>|<span data-ttu-id="3e230-121">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="3e230-121">The status for follow-up for an item.</span></span> <span data-ttu-id="3e230-122">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="3e230-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="3e230-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3e230-123">startDateTime</span></span>|<span data-ttu-id="3e230-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="3e230-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="3e230-125">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="3e230-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e230-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e230-126">JSON representation</span></span>

<span data-ttu-id="3e230-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e230-127">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


