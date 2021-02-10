---
title: Тип ресурса room
description: Указывает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3936338aee39eb0c10a179e5d1970b3e18493214
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156331"
---
# <a name="room-resource-type"></a><span data-ttu-id="c3dd8-103">Тип ресурса room</span><span class="sxs-lookup"><span data-stu-id="c3dd8-103">room resource type</span></span>

<span data-ttu-id="c3dd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3dd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3dd8-105">Представляет комнату в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="c3dd8-106">В Exchange Online каждая комната связана с почтовым ящиком помещения.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="c3dd8-107">Является производным от [места.](place.md)</span><span class="sxs-lookup"><span data-stu-id="c3dd8-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c3dd8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c3dd8-108">Methods</span></span>

| <span data-ttu-id="c3dd8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c3dd8-109">Method</span></span>                              | <span data-ttu-id="c3dd8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3dd8-110">Return Type</span></span>                  | <span data-ttu-id="c3dd8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3dd8-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="c3dd8-112">Места списка</span><span class="sxs-lookup"><span data-stu-id="c3dd8-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="c3dd8-113">Коллекция запрашиваемого производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="c3dd8-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="c3dd8-114">Получите коллекцию указанного типа объекта **place,** определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="c3dd8-115">Например, можно получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="c3dd8-116">Получить место</span><span class="sxs-lookup"><span data-stu-id="c3dd8-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="c3dd8-117">Запрашиваемая производная тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="c3dd8-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="c3dd8-118">Получите свойства и связи объекта указанного **места,** например помещения.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3dd8-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3dd8-119">Properties</span></span>

| <span data-ttu-id="c3dd8-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3dd8-120">Property</span></span>               | <span data-ttu-id="c3dd8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c3dd8-121">Type</span></span>                                              | <span data-ttu-id="c3dd8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c3dd8-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="c3dd8-123">address</span><span class="sxs-lookup"><span data-stu-id="c3dd8-123">address</span></span>                | [<span data-ttu-id="c3dd8-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c3dd8-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="c3dd8-125">Адрес улицы помещения.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-125">The street address of the room.</span></span> |
| <span data-ttu-id="c3dd8-126">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="c3dd8-126">audioDeviceName</span></span>        | <span data-ttu-id="c3dd8-127">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-127">String</span></span>                                            | <span data-ttu-id="c3dd8-128">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="c3dd8-129">bookingType</span><span class="sxs-lookup"><span data-stu-id="c3dd8-129">bookingType</span></span>            | [<span data-ttu-id="c3dd8-130">bookingType</span><span class="sxs-lookup"><span data-stu-id="c3dd8-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="c3dd8-131">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-131">Type of room.</span></span> <span data-ttu-id="c3dd8-132">Возможные значения: `standard` и `reserved` .</span><span class="sxs-lookup"><span data-stu-id="c3dd8-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="c3dd8-133">building</span><span class="sxs-lookup"><span data-stu-id="c3dd8-133">building</span></span>               | <span data-ttu-id="c3dd8-134">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-134">String</span></span>                                            | <span data-ttu-id="c3dd8-135">Указывает имя здания или номер здания, в который находится помещение.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="c3dd8-136">capacity</span><span class="sxs-lookup"><span data-stu-id="c3dd8-136">capacity</span></span>               | <span data-ttu-id="c3dd8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c3dd8-137">Int32</span></span>                                             | <span data-ttu-id="c3dd8-138">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="c3dd8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c3dd8-139">displayName</span></span>            | <span data-ttu-id="c3dd8-140">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-140">String</span></span>                                            | <span data-ttu-id="c3dd8-141">Имя, связанное с комнатой.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-141">The name associated with the room.</span></span> |
| <span data-ttu-id="c3dd8-142">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="c3dd8-142">displayDeviceName</span></span>      | <span data-ttu-id="c3dd8-143">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-143">String</span></span>                                            | <span data-ttu-id="c3dd8-144">Указывает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="c3dd8-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c3dd8-145">emailAddress</span></span>           | <span data-ttu-id="c3dd8-146">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-146">String</span></span>                                            | <span data-ttu-id="c3dd8-147">Адрес электронной почты помещения.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-147">Email address of the room.</span></span> |
| <span data-ttu-id="c3dd8-148">floorLabel</span><span class="sxs-lookup"><span data-stu-id="c3dd8-148">floorLabel</span></span>             | <span data-ttu-id="c3dd8-149">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-149">String</span></span>                                            | <span data-ttu-id="c3dd8-150">Указывает описательную метку для полу, например P.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="c3dd8-151">floorNumber</span><span class="sxs-lookup"><span data-stu-id="c3dd8-151">floorNumber</span></span>            | <span data-ttu-id="c3dd8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c3dd8-152">Int32</span></span>                                             | <span data-ttu-id="c3dd8-153">Указывает номер этажа, на который находится комната.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="c3dd8-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c3dd8-154">geoCoordinates</span></span>         | [<span data-ttu-id="c3dd8-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="c3dd8-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="c3dd8-156">Указывает расположение помещения в широте, долготе и при желании в координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="c3dd8-157">id</span><span class="sxs-lookup"><span data-stu-id="c3dd8-157">id</span></span>                     | <span data-ttu-id="c3dd8-158">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-158">String</span></span>                                            | <span data-ttu-id="c3dd8-159">Уникальный идентификатор комнаты.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-159">Unique identifier for the room.</span></span> <span data-ttu-id="c3dd8-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-160">Read-only.</span></span> |
| <span data-ttu-id="c3dd8-161">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="c3dd8-161">isWheelChairAccessible</span></span> | <span data-ttu-id="c3dd8-162">Логическое</span><span class="sxs-lookup"><span data-stu-id="c3dd8-162">Boolean</span></span>                                           | <span data-ttu-id="c3dd8-163">Указывает, доступна ли комната.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="c3dd8-164">label</span><span class="sxs-lookup"><span data-stu-id="c3dd8-164">label</span></span>                  | <span data-ttu-id="c3dd8-165">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-165">String</span></span>                                            | <span data-ttu-id="c3dd8-166">Указывает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="c3dd8-167">nickname</span><span class="sxs-lookup"><span data-stu-id="c3dd8-167">nickname</span></span>               | <span data-ttu-id="c3dd8-168">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-168">String</span></span>                                            | <span data-ttu-id="c3dd8-169">Указывает псевдоним для комнаты, например "conf room".</span><span class="sxs-lookup"><span data-stu-id="c3dd8-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="c3dd8-170">phone</span><span class="sxs-lookup"><span data-stu-id="c3dd8-170">phone</span></span>                  | <span data-ttu-id="c3dd8-171">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-171">String</span></span>                                            | <span data-ttu-id="c3dd8-172">Номер телефона комнаты.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-172">The phone number of the room.</span></span> |
| <span data-ttu-id="c3dd8-173">tags</span><span class="sxs-lookup"><span data-stu-id="c3dd8-173">tags</span></span>                   | <span data-ttu-id="c3dd8-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-174">String collection</span></span>                                 | <span data-ttu-id="c3dd8-175">Указывает дополнительные функции комнаты, например сведения о типе представления или типе ветвя.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="c3dd8-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="c3dd8-176">videoDeviceName</span></span>        | <span data-ttu-id="c3dd8-177">String</span><span class="sxs-lookup"><span data-stu-id="c3dd8-177">String</span></span>                                            | <span data-ttu-id="c3dd8-178">Указывает имя видео устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="c3dd8-179">Значения bookingType</span><span class="sxs-lookup"><span data-stu-id="c3dd8-179">bookingType values</span></span>

| <span data-ttu-id="c3dd8-180">Значение</span><span class="sxs-lookup"><span data-stu-id="c3dd8-180">Value</span></span>    | <span data-ttu-id="c3dd8-181">Описание</span><span class="sxs-lookup"><span data-stu-id="c3dd8-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="c3dd8-182">standard</span><span class="sxs-lookup"><span data-stu-id="c3dd8-182">standard</span></span> | <span data-ttu-id="c3dd8-183">Комната доступна и может быть зарезервирована.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-183">The room is available and can be reserved.</span></span> <span data-ttu-id="c3dd8-184">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-184">This is the default value.</span></span> |
| <span data-ttu-id="c3dd8-185">reserved</span><span class="sxs-lookup"><span data-stu-id="c3dd8-185">reserved</span></span> | <span data-ttu-id="c3dd8-186">Комната доступна только при первом веданном помещении.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="c3dd8-187">Его нельзя зарезервировать.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3dd8-188">Связи</span><span class="sxs-lookup"><span data-stu-id="c3dd8-188">Relationships</span></span>

<span data-ttu-id="c3dd8-189">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3dd8-190">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3dd8-190">JSON representation</span></span>

<span data-ttu-id="c3dd8-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3dd8-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

