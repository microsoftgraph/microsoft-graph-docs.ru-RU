---
title: Тип ресурса followupFlag
description: Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже. К поддерживаемым элементам относятся message и contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b4b33fc17eb8dfb44e46ac18cb18aaeabe3d06c
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062618"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="0cb19-104">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="0cb19-104">followupFlag resource type</span></span>

<span data-ttu-id="0cb19-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb19-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb19-106">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="0cb19-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="0cb19-107">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="0cb19-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0cb19-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cb19-108">Properties</span></span>
| <span data-ttu-id="0cb19-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cb19-109">Property</span></span>     | <span data-ttu-id="0cb19-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0cb19-110">Type</span></span>   |<span data-ttu-id="0cb19-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0cb19-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cb19-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb19-112">completedDateTime</span></span>|[<span data-ttu-id="0cb19-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0cb19-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0cb19-114">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="0cb19-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0cb19-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb19-115">dueDateTime</span></span>|<span data-ttu-id="0cb19-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0cb19-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0cb19-117">Дата и время выполнения дальнейших действий.</span><span class="sxs-lookup"><span data-stu-id="0cb19-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="0cb19-118">**Примечание**: чтобы задать дату выполнения, необходимо также указать значение `startDateTime`; в противном случае будет получен `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="0cb19-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="0cb19-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0cb19-119">flagStatus</span></span>|<span data-ttu-id="0cb19-120">String</span><span class="sxs-lookup"><span data-stu-id="0cb19-120">String</span></span>|<span data-ttu-id="0cb19-121">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="0cb19-121">The status for follow-up for an item.</span></span> <span data-ttu-id="0cb19-122">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="0cb19-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0cb19-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb19-123">startDateTime</span></span>|<span data-ttu-id="0cb19-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0cb19-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0cb19-125">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="0cb19-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cb19-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0cb19-126">JSON representation</span></span>

<span data-ttu-id="0cb19-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cb19-127">Here is a JSON representation of the resource</span></span>

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
