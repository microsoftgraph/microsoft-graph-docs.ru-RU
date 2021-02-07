---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе для последующего действия пользователя. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b690c86a6ccbef6f5c215e268f7b34243e3023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130208"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="25e40-103">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="25e40-103">followupFlag resource type</span></span>

<span data-ttu-id="25e40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e40-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="25e40-105">Позволяет установить флаг в элементе для последующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="25e40-105">Allows setting a flag in an item for the user to follow up on later.</span></span>

## <a name="properties"></a><span data-ttu-id="25e40-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25e40-106">Properties</span></span>
| <span data-ttu-id="25e40-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25e40-107">Property</span></span>     | <span data-ttu-id="25e40-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25e40-108">Type</span></span>   |<span data-ttu-id="25e40-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25e40-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25e40-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="25e40-110">completedDateTime</span></span>|[<span data-ttu-id="25e40-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="25e40-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="25e40-112">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="25e40-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="25e40-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="25e40-113">dueDateTime</span></span>|<span data-ttu-id="25e40-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="25e40-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="25e40-115">Дата и время завершения последующего действия.</span><span class="sxs-lookup"><span data-stu-id="25e40-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="25e40-116">**Примечание.** Чтобы задать дату окончания, необходимо также указать; в противном случае вы `startDateTime` получите `400 Bad Request` ответ.</span><span class="sxs-lookup"><span data-stu-id="25e40-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="25e40-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="25e40-117">flagStatus</span></span>|<span data-ttu-id="25e40-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="25e40-118">followupFlagStatus</span></span>|<span data-ttu-id="25e40-119">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="25e40-119">The status for follow-up for an item.</span></span> <span data-ttu-id="25e40-120">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="25e40-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="25e40-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="25e40-121">startDateTime</span></span>|<span data-ttu-id="25e40-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="25e40-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="25e40-123">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="25e40-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25e40-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25e40-124">JSON representation</span></span>

<span data-ttu-id="25e40-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25e40-125">Here is a JSON representation of the resource.</span></span>

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

