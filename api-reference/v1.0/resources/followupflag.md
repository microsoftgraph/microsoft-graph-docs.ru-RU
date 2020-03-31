---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c59401a9265f892fb2573fc2be3b0525baf1ece
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062590"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="20963-103">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="20963-103">followupFlag resource type</span></span>

<span data-ttu-id="20963-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20963-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="20963-105">Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия.</span><span class="sxs-lookup"><span data-stu-id="20963-105">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="20963-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="20963-106">Properties</span></span>
| <span data-ttu-id="20963-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="20963-107">Property</span></span>     | <span data-ttu-id="20963-108">Тип</span><span class="sxs-lookup"><span data-stu-id="20963-108">Type</span></span>   |<span data-ttu-id="20963-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20963-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20963-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="20963-110">completedDateTime</span></span>|[<span data-ttu-id="20963-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="20963-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="20963-112">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="20963-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="20963-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="20963-113">dueDateTime</span></span>|<span data-ttu-id="20963-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="20963-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="20963-115">Дата и время выполнения дальнейших действий.</span><span class="sxs-lookup"><span data-stu-id="20963-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="20963-116">**Примечание**: чтобы задать дату выполнения, необходимо также указать значение `startDateTime`; в противном случае будет получен `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="20963-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="20963-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="20963-117">flagStatus</span></span>|<span data-ttu-id="20963-118">фолловупфлагстатус</span><span class="sxs-lookup"><span data-stu-id="20963-118">followupFlagStatus</span></span>|<span data-ttu-id="20963-119">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="20963-119">The status for follow-up for an item.</span></span> <span data-ttu-id="20963-120">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="20963-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="20963-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20963-121">startDateTime</span></span>|<span data-ttu-id="20963-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="20963-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="20963-123">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="20963-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20963-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="20963-124">JSON representation</span></span>

<span data-ttu-id="20963-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20963-125">Here is a JSON representation of the resource.</span></span>

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
