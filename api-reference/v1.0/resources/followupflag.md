---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: adf67d503fa7576ad7446845a98bf799218f768d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030291"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="6deb3-103">Тип ресурса followupFlag</span><span class="sxs-lookup"><span data-stu-id="6deb3-103">followupFlag resource type</span></span>


<span data-ttu-id="6deb3-104">Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия.</span><span class="sxs-lookup"><span data-stu-id="6deb3-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="6deb3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6deb3-105">Properties</span></span>
| <span data-ttu-id="6deb3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6deb3-106">Property</span></span>     | <span data-ttu-id="6deb3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6deb3-107">Type</span></span>   |<span data-ttu-id="6deb3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6deb3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6deb3-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6deb3-109">completedDateTime</span></span>|[<span data-ttu-id="6deb3-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6deb3-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6deb3-111">Дата и время, когда выполнение было завершено.</span><span class="sxs-lookup"><span data-stu-id="6deb3-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="6deb3-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="6deb3-112">dueDateTime</span></span>|<span data-ttu-id="6deb3-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6deb3-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6deb3-114">Дата и время, когда выполнение должно быть завершено.</span><span class="sxs-lookup"><span data-stu-id="6deb3-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="6deb3-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="6deb3-115">flagStatus</span></span>|<span data-ttu-id="6deb3-116">Фолловупфлагстатус</span><span class="sxs-lookup"><span data-stu-id="6deb3-116">followupFlagStatus</span></span>|<span data-ttu-id="6deb3-117">Состояние выполнения для элемента.</span><span class="sxs-lookup"><span data-stu-id="6deb3-117">The status for follow-up for an item.</span></span> <span data-ttu-id="6deb3-118">Возможные значения: `notFlagged`, `complete` и `flagged`.</span><span class="sxs-lookup"><span data-stu-id="6deb3-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="6deb3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6deb3-119">startDateTime</span></span>|<span data-ttu-id="6deb3-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6deb3-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6deb3-121">Дата и время, когда следует начать выполнение.</span><span class="sxs-lookup"><span data-stu-id="6deb3-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6deb3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6deb3-122">JSON representation</span></span>

<span data-ttu-id="6deb3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6deb3-123">Here is a JSON representation of the resource</span></span>

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
