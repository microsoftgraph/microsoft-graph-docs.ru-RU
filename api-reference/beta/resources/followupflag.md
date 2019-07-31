---
title: Тип ресурса followupFlag
description: Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже. К поддерживаемым элементам относятся message и contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f60187fcfb3d41779547b6252edf69c1fc2735
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971979"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="b8c74-104">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="b8c74-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8c74-105">Позволяет установить отметку для пользователя, что к этому элементу необходимо вернуться позже.</span><span class="sxs-lookup"><span data-stu-id="b8c74-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="b8c74-106">К поддерживаемым элементам относятся [message](message.md) и [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="b8c74-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8c74-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8c74-107">Properties</span></span>
| <span data-ttu-id="b8c74-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8c74-108">Property</span></span>     | <span data-ttu-id="b8c74-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8c74-109">Type</span></span>   |<span data-ttu-id="b8c74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c74-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8c74-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c74-111">completedDateTime</span></span>|[<span data-ttu-id="b8c74-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b8c74-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b8c74-113">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="b8c74-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="b8c74-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c74-114">dueDateTime</span></span>|<span data-ttu-id="b8c74-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b8c74-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b8c74-116">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="b8c74-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="b8c74-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="b8c74-117">flagStatus</span></span>|<span data-ttu-id="b8c74-118">String</span><span class="sxs-lookup"><span data-stu-id="b8c74-118">String</span></span>|<span data-ttu-id="b8c74-119">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="b8c74-119">The status for follow-up for an item.</span></span> <span data-ttu-id="b8c74-120">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="b8c74-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="b8c74-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c74-121">startDateTime</span></span>|<span data-ttu-id="b8c74-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b8c74-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b8c74-123">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="b8c74-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8c74-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8c74-124">JSON representation</span></span>

<span data-ttu-id="b8c74-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8c74-125">Here is a JSON representation of the resource</span></span>

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
