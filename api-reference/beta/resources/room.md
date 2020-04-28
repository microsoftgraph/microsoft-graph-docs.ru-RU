---
title: Тип ресурса "комната"
description: Задает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e23d8a873abb0de5a086350b3748f9e40d7e12ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521042"
---
# <a name="room-resource-type"></a><span data-ttu-id="086d9-103">Тип ресурса "комната"</span><span class="sxs-lookup"><span data-stu-id="086d9-103">room resource type</span></span>

<span data-ttu-id="086d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="086d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086d9-105">Представляет комнату в клиенте.</span><span class="sxs-lookup"><span data-stu-id="086d9-105">Represents a room in a tenant.</span></span> 

<span data-ttu-id="086d9-106">В Exchange Online каждая комната связана с почтовым ящиком комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-106">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="086d9-107">Производный от [позиции](place.md).</span><span class="sxs-lookup"><span data-stu-id="086d9-107">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="086d9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="086d9-108">Methods</span></span>

| <span data-ttu-id="086d9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="086d9-109">Method</span></span>                              | <span data-ttu-id="086d9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="086d9-110">Return Type</span></span>                  | <span data-ttu-id="086d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="086d9-111">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="086d9-112">Список мест</span><span class="sxs-lookup"><span data-stu-id="086d9-112">List places</span></span>](../api/place-list.md) | <span data-ttu-id="086d9-113">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="086d9-113">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="086d9-114">Получение коллекции указанного типа объекта **Place** , определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="086d9-114">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="086d9-115">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="086d9-115">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="086d9-116">Получение</span><span class="sxs-lookup"><span data-stu-id="086d9-116">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="086d9-117">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="086d9-117">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="086d9-118">Получение свойств и связей указанного объекта **Place** , например комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-118">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="086d9-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="086d9-119">Properties</span></span>

| <span data-ttu-id="086d9-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="086d9-120">Property</span></span>               | <span data-ttu-id="086d9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="086d9-121">Type</span></span>                                              | <span data-ttu-id="086d9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="086d9-122">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="086d9-123">address</span><span class="sxs-lookup"><span data-stu-id="086d9-123">address</span></span>                | [<span data-ttu-id="086d9-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="086d9-124">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="086d9-125">Почтовый адрес комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-125">The street address of the room.</span></span> |
| <span data-ttu-id="086d9-126">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="086d9-126">audioDeviceName</span></span>        | <span data-ttu-id="086d9-127">String</span><span class="sxs-lookup"><span data-stu-id="086d9-127">String</span></span>                                            | <span data-ttu-id="086d9-128">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="086d9-128">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="086d9-129">букингтипе</span><span class="sxs-lookup"><span data-stu-id="086d9-129">bookingType</span></span>            | [<span data-ttu-id="086d9-130">букингтипе</span><span class="sxs-lookup"><span data-stu-id="086d9-130">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="086d9-131">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-131">Type of room.</span></span> <span data-ttu-id="086d9-132">Возможные значения: `standard`и `reserved`.</span><span class="sxs-lookup"><span data-stu-id="086d9-132">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="086d9-133">создания</span><span class="sxs-lookup"><span data-stu-id="086d9-133">building</span></span>               | <span data-ttu-id="086d9-134">String</span><span class="sxs-lookup"><span data-stu-id="086d9-134">String</span></span>                                            | <span data-ttu-id="086d9-135">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="086d9-135">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="086d9-136">мощности</span><span class="sxs-lookup"><span data-stu-id="086d9-136">capacity</span></span>               | <span data-ttu-id="086d9-137">String</span><span class="sxs-lookup"><span data-stu-id="086d9-137">String</span></span>                                            | <span data-ttu-id="086d9-138">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-138">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="086d9-139">displayName</span><span class="sxs-lookup"><span data-stu-id="086d9-139">displayName</span></span>            | <span data-ttu-id="086d9-140">Строка</span><span class="sxs-lookup"><span data-stu-id="086d9-140">String</span></span>                                            | <span data-ttu-id="086d9-141">Имя, связанное с комнатой.</span><span class="sxs-lookup"><span data-stu-id="086d9-141">The name associated with the room.</span></span> |
| <span data-ttu-id="086d9-142">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="086d9-142">displayDeviceName</span></span>      | <span data-ttu-id="086d9-143">String</span><span class="sxs-lookup"><span data-stu-id="086d9-143">String</span></span>                                            | <span data-ttu-id="086d9-144">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="086d9-144">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="086d9-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="086d9-145">emailAddress</span></span>           | <span data-ttu-id="086d9-146">String</span><span class="sxs-lookup"><span data-stu-id="086d9-146">String</span></span>                                            | <span data-ttu-id="086d9-147">Адрес электронной почты комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-147">Email address of the room.</span></span> |
| <span data-ttu-id="086d9-148">флурлабел</span><span class="sxs-lookup"><span data-stu-id="086d9-148">floorLabel</span></span>             | <span data-ttu-id="086d9-149">String</span><span class="sxs-lookup"><span data-stu-id="086d9-149">String</span></span>                                            | <span data-ttu-id="086d9-150">Задает описательную метку для пола, например P.</span><span class="sxs-lookup"><span data-stu-id="086d9-150">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="086d9-151">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="086d9-151">floorNumber</span></span>            | <span data-ttu-id="086d9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="086d9-152">Int32</span></span>                                             | <span data-ttu-id="086d9-153">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="086d9-153">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="086d9-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="086d9-154">geoCoordinates</span></span>         | [<span data-ttu-id="086d9-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="086d9-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="086d9-156">Указывает расположение комнаты в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="086d9-156">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="086d9-157">id</span><span class="sxs-lookup"><span data-stu-id="086d9-157">id</span></span>                     | <span data-ttu-id="086d9-158">String</span><span class="sxs-lookup"><span data-stu-id="086d9-158">String</span></span>                                            | <span data-ttu-id="086d9-159">Уникальный идентификатор комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-159">Unique identifier for the room.</span></span> <span data-ttu-id="086d9-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="086d9-160">Read-only.</span></span> |
| <span data-ttu-id="086d9-161">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="086d9-161">isWheelchairAccessible</span></span> | <span data-ttu-id="086d9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="086d9-162">Boolean</span></span>                                           | <span data-ttu-id="086d9-163">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="086d9-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="086d9-164">label</span><span class="sxs-lookup"><span data-stu-id="086d9-164">label</span></span>                  | <span data-ttu-id="086d9-165">String</span><span class="sxs-lookup"><span data-stu-id="086d9-165">String</span></span>                                            | <span data-ttu-id="086d9-166">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="086d9-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="086d9-167">прозвищ</span><span class="sxs-lookup"><span data-stu-id="086d9-167">nickname</span></span>               | <span data-ttu-id="086d9-168">String</span><span class="sxs-lookup"><span data-stu-id="086d9-168">String</span></span>                                            | <span data-ttu-id="086d9-169">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="086d9-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="086d9-170">phone</span><span class="sxs-lookup"><span data-stu-id="086d9-170">phone</span></span>                  | <span data-ttu-id="086d9-171">String</span><span class="sxs-lookup"><span data-stu-id="086d9-171">String</span></span>                                            | <span data-ttu-id="086d9-172">Номер телефона комнаты.</span><span class="sxs-lookup"><span data-stu-id="086d9-172">The phone number of the room.</span></span> |
| <span data-ttu-id="086d9-173">tags</span><span class="sxs-lookup"><span data-stu-id="086d9-173">tags</span></span>                   | <span data-ttu-id="086d9-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="086d9-174">String collection</span></span>                                 | <span data-ttu-id="086d9-175">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="086d9-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="086d9-176">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="086d9-176">videoDeviceName</span></span>        | <span data-ttu-id="086d9-177">String</span><span class="sxs-lookup"><span data-stu-id="086d9-177">String</span></span>                                            | <span data-ttu-id="086d9-178">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="086d9-178">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="086d9-179">значения Букингтипе</span><span class="sxs-lookup"><span data-stu-id="086d9-179">bookingType values</span></span>

| <span data-ttu-id="086d9-180">Значение</span><span class="sxs-lookup"><span data-stu-id="086d9-180">Value</span></span>    | <span data-ttu-id="086d9-181">Описание</span><span class="sxs-lookup"><span data-stu-id="086d9-181">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="086d9-182">Стандартный</span><span class="sxs-lookup"><span data-stu-id="086d9-182">standard</span></span> | <span data-ttu-id="086d9-183">Комнату можно зарезервировать в соответствии с другими параметрами в этом командлете.</span><span class="sxs-lookup"><span data-stu-id="086d9-183">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="086d9-184">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="086d9-184">This is the default value.</span></span> |
| <span data-ttu-id="086d9-185">резервирования</span><span class="sxs-lookup"><span data-stu-id="086d9-185">reserved</span></span> | <span data-ttu-id="086d9-186">Комната доступна только в первый поступающий, первый обслуживаемый.</span><span class="sxs-lookup"><span data-stu-id="086d9-186">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="086d9-187">Оно не может быть зарезервировано.</span><span class="sxs-lookup"><span data-stu-id="086d9-187">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="086d9-188">Связи</span><span class="sxs-lookup"><span data-stu-id="086d9-188">Relationships</span></span>

<span data-ttu-id="086d9-189">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="086d9-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="086d9-190">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="086d9-190">JSON representation</span></span>

<span data-ttu-id="086d9-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="086d9-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
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
