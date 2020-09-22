---
title: Тип ресурса RoomList принимают одиночные
description: Представляет группу комнат, созданных компанией.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 736eefce535a0a9ebaf6098fa10675f1357541da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016130"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="84c83-103">Тип ресурса RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="84c83-103">roomList resource type</span></span>

<span data-ttu-id="84c83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84c83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c83-105">Представляет группу объектов [комнаты](room.md) , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="84c83-105">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="84c83-106">Производный от [позиции](place.md).</span><span class="sxs-lookup"><span data-stu-id="84c83-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="84c83-107">Методы</span><span class="sxs-lookup"><span data-stu-id="84c83-107">Methods</span></span>

| <span data-ttu-id="84c83-108">Метод</span><span class="sxs-lookup"><span data-stu-id="84c83-108">Method</span></span>                              | <span data-ttu-id="84c83-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84c83-109">Return Type</span></span>                  | <span data-ttu-id="84c83-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84c83-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="84c83-111">Список мест</span><span class="sxs-lookup"><span data-stu-id="84c83-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="84c83-112">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="84c83-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="84c83-113">Получение коллекции указанного типа объекта **Place** , определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="84c83-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="84c83-114">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="84c83-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="84c83-115">Получение</span><span class="sxs-lookup"><span data-stu-id="84c83-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="84c83-116">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="84c83-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="84c83-117">Получение свойств и связей указанного объекта **Place** , например списка помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-117">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="84c83-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="84c83-118">Properties</span></span>

| <span data-ttu-id="84c83-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="84c83-119">Property</span></span>       | <span data-ttu-id="84c83-120">Тип</span><span class="sxs-lookup"><span data-stu-id="84c83-120">Type</span></span>                                              | <span data-ttu-id="84c83-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84c83-121">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="84c83-122">address</span><span class="sxs-lookup"><span data-stu-id="84c83-122">address</span></span>        | [<span data-ttu-id="84c83-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="84c83-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="84c83-124">Почтовый адрес списка помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-124">The street address of the room list.</span></span> |
| <span data-ttu-id="84c83-125">displayName</span><span class="sxs-lookup"><span data-stu-id="84c83-125">displayName</span></span>    | <span data-ttu-id="84c83-126">String</span><span class="sxs-lookup"><span data-stu-id="84c83-126">String</span></span>                                            | <span data-ttu-id="84c83-127">Имя, связанное со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-127">The name associated with the room list.</span></span> |
| <span data-ttu-id="84c83-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="84c83-128">emailAddress</span></span>   | <span data-ttu-id="84c83-129">String</span><span class="sxs-lookup"><span data-stu-id="84c83-129">String</span></span>                                            | <span data-ttu-id="84c83-130">Адрес электронной почты списка помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-130">The email address of the room list.</span></span> |
| <span data-ttu-id="84c83-131">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="84c83-131">geoCoordinates</span></span> | [<span data-ttu-id="84c83-132">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="84c83-132">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="84c83-133">Указывает расположение RoomList принимают одиночные в широте, долготе и (дополнительно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="84c83-133">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="84c83-134">id</span><span class="sxs-lookup"><span data-stu-id="84c83-134">id</span></span>             | <span data-ttu-id="84c83-135">String</span><span class="sxs-lookup"><span data-stu-id="84c83-135">String</span></span>                                            | <span data-ttu-id="84c83-136">Уникальный идентификатор для списка помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-136">Unique identifier for the room list.</span></span> <span data-ttu-id="84c83-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84c83-137">Read-only.</span></span> |
| <span data-ttu-id="84c83-138">phone</span><span class="sxs-lookup"><span data-stu-id="84c83-138">phone</span></span>          | <span data-ttu-id="84c83-139">String</span><span class="sxs-lookup"><span data-stu-id="84c83-139">String</span></span>                                            | <span data-ttu-id="84c83-140">Номер телефона списка помещений.</span><span class="sxs-lookup"><span data-stu-id="84c83-140">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84c83-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="84c83-141">Relationships</span></span>

| <span data-ttu-id="84c83-142">Связь</span><span class="sxs-lookup"><span data-stu-id="84c83-142">Relationship</span></span> | <span data-ttu-id="84c83-143">Тип</span><span class="sxs-lookup"><span data-stu-id="84c83-143">Type</span></span>                         | <span data-ttu-id="84c83-144">Описание</span><span class="sxs-lookup"><span data-stu-id="84c83-144">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="84c83-145">комната</span><span class="sxs-lookup"><span data-stu-id="84c83-145">rooms</span></span>        | <span data-ttu-id="84c83-146">[помещение](place.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="84c83-146">[place](place.md) collection</span></span> | <span data-ttu-id="84c83-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="84c83-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84c83-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84c83-149">JSON representation</span></span>

<span data-ttu-id="84c83-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84c83-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


