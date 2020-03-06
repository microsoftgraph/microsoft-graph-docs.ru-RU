---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 28734c08d4626805de467ebad8c640acf3bdf7f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531391"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="7f8fe-103">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="7f8fe-103">followupFlag resource type</span></span>

<span data-ttu-id="7f8fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f8fe-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="7f8fe-105">Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-105">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="7f8fe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f8fe-106">Properties</span></span>
| <span data-ttu-id="7f8fe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f8fe-107">Property</span></span>     | <span data-ttu-id="7f8fe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7f8fe-108">Type</span></span>   |<span data-ttu-id="7f8fe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f8fe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f8fe-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8fe-110">completedDateTime</span></span>|[<span data-ttu-id="7f8fe-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7f8fe-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7f8fe-112">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="7f8fe-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8fe-113">dueDateTime</span></span>|<span data-ttu-id="7f8fe-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="7f8fe-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="7f8fe-115">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-115">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="7f8fe-116">flagStatus</span><span class="sxs-lookup"><span data-stu-id="7f8fe-116">flagStatus</span></span>|<span data-ttu-id="7f8fe-117">фолловупфлагстатус</span><span class="sxs-lookup"><span data-stu-id="7f8fe-117">followupFlagStatus</span></span>|<span data-ttu-id="7f8fe-118">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-118">The status for follow-up for an item.</span></span> <span data-ttu-id="7f8fe-119">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-119">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="7f8fe-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8fe-120">startDateTime</span></span>|<span data-ttu-id="7f8fe-121">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="7f8fe-121">**dateTimeTimeZone**</span></span>|<span data-ttu-id="7f8fe-122">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-122">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f8fe-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f8fe-123">JSON representation</span></span>

<span data-ttu-id="7f8fe-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f8fe-124">Here is a JSON representation of the resource</span></span>

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
