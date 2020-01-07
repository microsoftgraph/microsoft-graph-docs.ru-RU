---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a172737f40572b29358ecdc6fba804db2a8b80e5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951960"
---
# <a name="swapshiftschangerequest-resource-type"></a><span data-ttu-id="286a5-103">Тип ресурса Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="286a5-103">swapShiftsChangeRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="286a5-104">Представляет тип запроса на сдвиг для замены [смены](../resources/shift.md) другим пользователем в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="286a5-104">Represents a type of shift request to swap a [shift](../resources/shift.md) with another user in the [team](../resources/team.md).</span></span>

## <a name="methods"></a><span data-ttu-id="286a5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="286a5-105">Methods</span></span>

| <span data-ttu-id="286a5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="286a5-106">Method</span></span>       | <span data-ttu-id="286a5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="286a5-107">Return Type</span></span> | <span data-ttu-id="286a5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="286a5-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="286a5-109">List</span><span class="sxs-lookup"><span data-stu-id="286a5-109">List</span></span>](../api/swapshiftschangerequest-list.md) | <span data-ttu-id="286a5-110">Коллекция [свапшифтсчанжерекуест](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="286a5-110">Collection of [swapShiftsChangeRequest](swapshiftschangerequest.md)</span></span> | <span data-ttu-id="286a5-111">Перечисление свойств и связей объектов **свапшифтсчанжерекуест** в команде.</span><span class="sxs-lookup"><span data-stu-id="286a5-111">List the properties and relationships of **swapShiftsChangeRequest** objects in a team.</span></span> |
| <span data-ttu-id="286a5-112">[создание](../api/swapshiftschangerequest-post.md);</span><span class="sxs-lookup"><span data-stu-id="286a5-112">[Create](../api/swapshiftschangerequest-post.md)</span></span> | [<span data-ttu-id="286a5-113">свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="286a5-113">swapshiftschangerequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="286a5-114">Создайте экземпляр объекта свапшифтсчанжерекуест.</span><span class="sxs-lookup"><span data-stu-id="286a5-114">Create an instance of an swapshiftschangerequest object.</span></span> |
| <span data-ttu-id="286a5-115">[получение](../api/swapshiftschangerequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="286a5-115">[Get](../api/swapshiftschangerequest-get.md)</span></span> | [<span data-ttu-id="286a5-116">свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="286a5-116">swapShiftsChangeRequest</span></span>](swapshiftschangerequest.md) | <span data-ttu-id="286a5-117">Чтение свойств и связей объекта **свапшифтсчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="286a5-117">Read the properties and relationships of a **swapShiftsChangeRequest** object.</span></span> |
|[<span data-ttu-id="286a5-118">Утвердить</span><span class="sxs-lookup"><span data-stu-id="286a5-118">Approve</span></span>](../api/swapshiftschangerequest-approve.md)|<span data-ttu-id="286a5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="286a5-119">None</span></span>|<span data-ttu-id="286a5-120">Утверждение свапшифтсчанжерекуест.</span><span class="sxs-lookup"><span data-stu-id="286a5-120">Approve an swapshiftschangerequest.</span></span> |

## <a name="properties"></a><span data-ttu-id="286a5-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="286a5-121">Properties</span></span>

| <span data-ttu-id="286a5-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="286a5-122">Property</span></span>     | <span data-ttu-id="286a5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="286a5-123">Type</span></span>        | <span data-ttu-id="286a5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="286a5-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="286a5-125">реЦипиентшифтид</span><span class="sxs-lookup"><span data-stu-id="286a5-125">recipientShiftId</span></span>|<span data-ttu-id="286a5-126">String</span><span class="sxs-lookup"><span data-stu-id="286a5-126">String</span></span>|<span data-ttu-id="286a5-127">Идентификатор получателя запроса на замену.</span><span class="sxs-lookup"><span data-stu-id="286a5-127">ID of the recipient of the swap request.</span></span> <span data-ttu-id="286a5-128">Это пользователь, с которым запрос перенаправляется.</span><span class="sxs-lookup"><span data-stu-id="286a5-128">This is the user with whom the request is to swap.</span></span>|

## <a name="relationships"></a><span data-ttu-id="286a5-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="286a5-129">Relationships</span></span>

<span data-ttu-id="286a5-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="286a5-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="286a5-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="286a5-131">JSON representation</span></span>

<span data-ttu-id="286a5-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="286a5-132">The following is a JSON representation of the resource.</span></span>

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
