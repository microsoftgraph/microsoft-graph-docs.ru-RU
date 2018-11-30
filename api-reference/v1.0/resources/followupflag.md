---
title: Тип ресурса followupFlag
description: 'Позволяет флаг в элементе для пользователя к исполнению более поздней версии. '
ms.openlocfilehash: 5aa9d82fc90d7142717ac5ef05f9d837bac371ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027961"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="8b6db-103">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="8b6db-103">followupFlag resource type</span></span>


<span data-ttu-id="8b6db-104">Позволяет флаг в элементе для пользователя к исполнению более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="8b6db-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="8b6db-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b6db-105">Properties</span></span>
| <span data-ttu-id="8b6db-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b6db-106">Property</span></span>     | <span data-ttu-id="8b6db-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8b6db-107">Type</span></span>   |<span data-ttu-id="8b6db-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8b6db-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b6db-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b6db-109">completedDateTime</span></span>|[<span data-ttu-id="8b6db-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8b6db-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8b6db-111">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="8b6db-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="8b6db-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="8b6db-112">dueDateTime</span></span>|<span data-ttu-id="8b6db-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="8b6db-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="8b6db-114">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="8b6db-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="8b6db-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="8b6db-115">flagStatus</span></span>|<span data-ttu-id="8b6db-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="8b6db-116">followupFlagStatus</span></span>|<span data-ttu-id="8b6db-117">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="8b6db-117">The status for follow-up for an item.</span></span> <span data-ttu-id="8b6db-118">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="8b6db-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="8b6db-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8b6db-119">startDateTime</span></span>|<span data-ttu-id="8b6db-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="8b6db-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="8b6db-121">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="8b6db-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b6db-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b6db-122">JSON representation</span></span>

<span data-ttu-id="8b6db-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b6db-123">Here is a JSON representation of the resource</span></span>

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
