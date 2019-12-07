---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 80149a37dfb4d8d900066d11c315d125ff7fd670
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895845"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="2077b-103">Тип ресурса Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="2077b-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2077b-104">Представляет тип запроса на сдвиг для замены [смены](../resources/shift.md) другим пользователем в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2077b-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2077b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2077b-105">Methods</span></span>

| <span data-ttu-id="2077b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2077b-106">Method</span></span>       | <span data-ttu-id="2077b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2077b-107">Return Type</span></span> | <span data-ttu-id="2077b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2077b-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2077b-109">[получение](../api/swapshiftschangerequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="2077b-109">[Get](../api/swapshiftschangerequest-get.md)</span></span> | [<span data-ttu-id="2077b-110">свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="2077b-110">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="2077b-111">Чтение свойств и связей объекта **свапшифтсчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="2077b-111">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
| <span data-ttu-id="2077b-112">[обновление](../api/swapshiftschangerequest-update.md).</span><span class="sxs-lookup"><span data-stu-id="2077b-112">[Update](../api/swapshiftschangerequest-update.md)</span></span> | [<span data-ttu-id="2077b-113">свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="2077b-113">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="2077b-114">Обновление объекта **свапшифтсчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="2077b-114">Update a **swapShiftsChangeRequest** object.</span></span> |
| <span data-ttu-id="2077b-115">[удаление](../api/swapshiftschangerequest-delete.md);</span><span class="sxs-lookup"><span data-stu-id="2077b-115">[Delete](../api/swapshiftschangerequest-delete.md)</span></span> | <span data-ttu-id="2077b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2077b-116">None</span></span> | <span data-ttu-id="2077b-117">Удаление объекта **свапшифтсчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="2077b-117">Delete a **swapShiftsChangeRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2077b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2077b-118">Properties</span></span>

| <span data-ttu-id="2077b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2077b-119">Property</span></span>     | <span data-ttu-id="2077b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2077b-120">Type</span></span>        | <span data-ttu-id="2077b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2077b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2077b-122">реЦипиентшифтид</span><span class="sxs-lookup"><span data-stu-id="2077b-122">recipientShiftId</span></span>|<span data-ttu-id="2077b-123">String</span><span class="sxs-lookup"><span data-stu-id="2077b-123">String</span></span>|<span data-ttu-id="2077b-124">Идентификатор получателя запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="2077b-124">ID of the recipient of the swap request.</span></span> <span data-ttu-id="2077b-125">Это пользователь, с которым запрос перенаправляется.</span><span class="sxs-lookup"><span data-stu-id="2077b-125">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2077b-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2077b-126">Relationships</span></span>

<span data-ttu-id="2077b-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2077b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2077b-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2077b-128">JSON representation</span></span>

<span data-ttu-id="2077b-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2077b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
