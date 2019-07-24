---
title: Тип ресурса RoomList принимают одиночные
description: Представляет группу комнат, созданных компанией.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841257"
---
# <a name="roomlist-resource-type"></a><span data-ttu-id="aaa3a-103">Тип ресурса RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="aaa3a-103">roomList resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaa3a-104">Представляет группу объектов [комнаты](room.md) , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-104">Represents a group of [room](room.md) objects defined in the tenant.</span></span>

<span data-ttu-id="aaa3a-105">Производный от [позиции](place.md).</span><span class="sxs-lookup"><span data-stu-id="aaa3a-105">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aaa3a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aaa3a-106">Methods</span></span>

| <span data-ttu-id="aaa3a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aaa3a-107">Method</span></span>                              | <span data-ttu-id="aaa3a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aaa3a-108">Return Type</span></span>                  | <span data-ttu-id="aaa3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa3a-109">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="aaa3a-110">Список мест</span><span class="sxs-lookup"><span data-stu-id="aaa3a-110">List places</span></span>](../api/place-list.md) | <span data-ttu-id="aaa3a-111">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="aaa3a-111">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="aaa3a-112">Получение коллекции указанного типа объекта **Place** , определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-112">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="aaa3a-113">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-113">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>|
| [<span data-ttu-id="aaa3a-114">Получение</span><span class="sxs-lookup"><span data-stu-id="aaa3a-114">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="aaa3a-115">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="aaa3a-115">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="aaa3a-116">Получение свойств и связей указанного объекта **Place** , например списка помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-116">Get the properties and relationships of the specified **place** object, such as a room list.</span></span> |

## <a name="properties"></a><span data-ttu-id="aaa3a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="aaa3a-117">Properties</span></span>

| <span data-ttu-id="aaa3a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaa3a-118">Property</span></span>       | <span data-ttu-id="aaa3a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa3a-119">Type</span></span>                                              | <span data-ttu-id="aaa3a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa3a-120">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="aaa3a-121">address</span><span class="sxs-lookup"><span data-stu-id="aaa3a-121">address</span></span>        | [<span data-ttu-id="aaa3a-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="aaa3a-122">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="aaa3a-123">Почтовый адрес списка помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-123">The street address of the room list.</span></span> |
| <span data-ttu-id="aaa3a-124">displayName</span><span class="sxs-lookup"><span data-stu-id="aaa3a-124">displayName</span></span>    | <span data-ttu-id="aaa3a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="aaa3a-125">String</span></span>                                            | <span data-ttu-id="aaa3a-126">Имя, связанное со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-126">The name associated with the room list.</span></span> |
| <span data-ttu-id="aaa3a-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="aaa3a-127">emailAddress</span></span>   | <span data-ttu-id="aaa3a-128">String</span><span class="sxs-lookup"><span data-stu-id="aaa3a-128">String</span></span>                                            | <span data-ttu-id="aaa3a-129">Адрес электронной почты списка помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-129">The email address of the room list.</span></span> |
| <span data-ttu-id="aaa3a-130">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="aaa3a-130">geoCoordinates</span></span> | [<span data-ttu-id="aaa3a-131">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="aaa3a-131">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="aaa3a-132">Указывает расположение RoomList принимают одиночные в широте, долготе и (дополнительно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-132">Specifies the roomlist location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="aaa3a-133">id</span><span class="sxs-lookup"><span data-stu-id="aaa3a-133">id</span></span>             | <span data-ttu-id="aaa3a-134">String</span><span class="sxs-lookup"><span data-stu-id="aaa3a-134">String</span></span>                                            | <span data-ttu-id="aaa3a-135">Уникальный идентификатор для списка помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-135">Unique identifier for the room list.</span></span> <span data-ttu-id="aaa3a-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-136">Read-only.</span></span> |
| <span data-ttu-id="aaa3a-137">phone</span><span class="sxs-lookup"><span data-stu-id="aaa3a-137">phone</span></span>          | <span data-ttu-id="aaa3a-138">String</span><span class="sxs-lookup"><span data-stu-id="aaa3a-138">String</span></span>                                            | <span data-ttu-id="aaa3a-139">Номер телефона списка помещений.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-139">The phone number of the room list.</span></span> |

## <a name="relationships"></a><span data-ttu-id="aaa3a-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="aaa3a-140">Relationships</span></span>

| <span data-ttu-id="aaa3a-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="aaa3a-141">Relationship</span></span> | <span data-ttu-id="aaa3a-142">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa3a-142">Type</span></span>                         | <span data-ttu-id="aaa3a-143">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa3a-143">Description</span></span>          |
|:-------------|:-----------------------------|:---------------------|
| <span data-ttu-id="aaa3a-144">комната</span><span class="sxs-lookup"><span data-stu-id="aaa3a-144">rooms</span></span>        | <span data-ttu-id="aaa3a-145">[помещение](place.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="aaa3a-145">[place](place.md) collection</span></span> | <span data-ttu-id="aaa3a-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-p103">Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aaa3a-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aaa3a-148">JSON representation</span></span>

<span data-ttu-id="aaa3a-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaa3a-149">The following is a JSON representation of the resource.</span></span>

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
