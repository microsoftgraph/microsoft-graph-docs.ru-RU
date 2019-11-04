---
title: Тип ресурса "комната"
description: Задает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cfa1d87093c7f843dd9a8294a253751726b3d34b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938725"
---
# <a name="room-resource-type"></a><span data-ttu-id="0b8f5-103">Тип ресурса "комната"</span><span class="sxs-lookup"><span data-stu-id="0b8f5-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b8f5-104">Представляет комнату в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="0b8f5-105">В Exchange Online каждая комната связана с почтовым ящиком комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="0b8f5-106">Производный от [позиции](place.md).</span><span class="sxs-lookup"><span data-stu-id="0b8f5-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0b8f5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0b8f5-107">Methods</span></span>

| <span data-ttu-id="0b8f5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0b8f5-108">Method</span></span>                              | <span data-ttu-id="0b8f5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b8f5-109">Return Type</span></span>                  | <span data-ttu-id="0b8f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8f5-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="0b8f5-111">Список мест</span><span class="sxs-lookup"><span data-stu-id="0b8f5-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="0b8f5-112">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="0b8f5-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="0b8f5-113">Получение коллекции указанного типа объекта **Place** , определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="0b8f5-114">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="0b8f5-115">Получение</span><span class="sxs-lookup"><span data-stu-id="0b8f5-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="0b8f5-116">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="0b8f5-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="0b8f5-117">Получение свойств и связей указанного объекта **Place** , например комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b8f5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b8f5-118">Properties</span></span>

| <span data-ttu-id="0b8f5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b8f5-119">Property</span></span>               | <span data-ttu-id="0b8f5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0b8f5-120">Type</span></span>                                              | <span data-ttu-id="0b8f5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8f5-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="0b8f5-122">address</span><span class="sxs-lookup"><span data-stu-id="0b8f5-122">address</span></span>                | [<span data-ttu-id="0b8f5-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0b8f5-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="0b8f5-124">Почтовый адрес комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-124">The street address of the room.</span></span> |
| <span data-ttu-id="0b8f5-125">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="0b8f5-125">audioDeviceName</span></span>        | <span data-ttu-id="0b8f5-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-126">String</span></span>                                            | <span data-ttu-id="0b8f5-127">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="0b8f5-128">букингтипе</span><span class="sxs-lookup"><span data-stu-id="0b8f5-128">bookingType</span></span>            | [<span data-ttu-id="0b8f5-129">букингтипе</span><span class="sxs-lookup"><span data-stu-id="0b8f5-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="0b8f5-130">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-130">Type of room.</span></span> <span data-ttu-id="0b8f5-131">Возможные значения: `standard`и `reserved`.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-131">Possible values are `standard`, and `reserved`.</span></span> |
| <span data-ttu-id="0b8f5-132">создания</span><span class="sxs-lookup"><span data-stu-id="0b8f5-132">building</span></span>               | <span data-ttu-id="0b8f5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-133">String</span></span>                                            | <span data-ttu-id="0b8f5-134">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="0b8f5-135">мощности</span><span class="sxs-lookup"><span data-stu-id="0b8f5-135">capacity</span></span>               | <span data-ttu-id="0b8f5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-136">String</span></span>                                            | <span data-ttu-id="0b8f5-137">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="0b8f5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0b8f5-138">displayName</span></span>            | <span data-ttu-id="0b8f5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-139">String</span></span>                                            | <span data-ttu-id="0b8f5-140">Имя, связанное с комнатой.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-140">The name associated with the room.</span></span> |
| <span data-ttu-id="0b8f5-141">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="0b8f5-141">displayDeviceName</span></span>      | <span data-ttu-id="0b8f5-142">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-142">String</span></span>                                            | <span data-ttu-id="0b8f5-143">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="0b8f5-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0b8f5-144">emailAddress</span></span>           | <span data-ttu-id="0b8f5-145">String</span><span class="sxs-lookup"><span data-stu-id="0b8f5-145">String</span></span>                                            | <span data-ttu-id="0b8f5-146">Адрес электронной почты комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-146">Email address of the room.</span></span> |
| <span data-ttu-id="0b8f5-147">флурлабел</span><span class="sxs-lookup"><span data-stu-id="0b8f5-147">floorLabel</span></span>             | <span data-ttu-id="0b8f5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-148">String</span></span>                                            | <span data-ttu-id="0b8f5-149">Задает описательную метку для пола, например P.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-149">Specifies a descriptive label for the floor, for example, P.</span></span> |
| <span data-ttu-id="0b8f5-150">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="0b8f5-150">floorNumber</span></span>            | <span data-ttu-id="0b8f5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8f5-151">Int32</span></span>                                             | <span data-ttu-id="0b8f5-152">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-152">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="0b8f5-153">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0b8f5-153">geoCoordinates</span></span>         | [<span data-ttu-id="0b8f5-154">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0b8f5-154">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="0b8f5-155">Указывает расположение комнаты в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-155">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="0b8f5-156">id</span><span class="sxs-lookup"><span data-stu-id="0b8f5-156">id</span></span>                     | <span data-ttu-id="0b8f5-157">String</span><span class="sxs-lookup"><span data-stu-id="0b8f5-157">String</span></span>                                            | <span data-ttu-id="0b8f5-158">Уникальный идентификатор комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-158">Unique identifier for the room.</span></span> <span data-ttu-id="0b8f5-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-159">Read-only.</span></span> |
| <span data-ttu-id="0b8f5-160">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="0b8f5-160">isWheelchairAccessible</span></span> | <span data-ttu-id="0b8f5-161">Логический</span><span class="sxs-lookup"><span data-stu-id="0b8f5-161">Boolean</span></span>                                           | <span data-ttu-id="0b8f5-162">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-162">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="0b8f5-163">label</span><span class="sxs-lookup"><span data-stu-id="0b8f5-163">label</span></span>                  | <span data-ttu-id="0b8f5-164">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-164">String</span></span>                                            | <span data-ttu-id="0b8f5-165">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-165">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="0b8f5-166">прозвищ</span><span class="sxs-lookup"><span data-stu-id="0b8f5-166">nickname</span></span>               | <span data-ttu-id="0b8f5-167">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-167">String</span></span>                                            | <span data-ttu-id="0b8f5-168">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="0b8f5-168">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="0b8f5-169">phone</span><span class="sxs-lookup"><span data-stu-id="0b8f5-169">phone</span></span>                  | <span data-ttu-id="0b8f5-170">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-170">String</span></span>                                            | <span data-ttu-id="0b8f5-171">Номер телефона комнаты.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-171">The phone number of the room.</span></span> |
| <span data-ttu-id="0b8f5-172">tags</span><span class="sxs-lookup"><span data-stu-id="0b8f5-172">tags</span></span>                   | <span data-ttu-id="0b8f5-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0b8f5-173">String collection</span></span>                                 | <span data-ttu-id="0b8f5-174">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-174">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="0b8f5-175">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="0b8f5-175">videoDeviceName</span></span>        | <span data-ttu-id="0b8f5-176">Строка</span><span class="sxs-lookup"><span data-stu-id="0b8f5-176">String</span></span>                                            | <span data-ttu-id="0b8f5-177">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-177">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="0b8f5-178">значения Букингтипе</span><span class="sxs-lookup"><span data-stu-id="0b8f5-178">bookingType values</span></span>

| <span data-ttu-id="0b8f5-179">Значение</span><span class="sxs-lookup"><span data-stu-id="0b8f5-179">Value</span></span>    | <span data-ttu-id="0b8f5-180">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8f5-180">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="0b8f5-181">Стандартный</span><span class="sxs-lookup"><span data-stu-id="0b8f5-181">standard</span></span> | <span data-ttu-id="0b8f5-182">Комнату можно зарезервировать в соответствии с другими параметрами в этом командлете.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-182">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="0b8f5-183">Для сообщений, отправляемых почтовому пользователю или почтовому контакту, используется формат, настроенный для почтового пользователя или почтового контакта.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-183">This is the default value.</span></span> |
| <span data-ttu-id="0b8f5-184">резервирования</span><span class="sxs-lookup"><span data-stu-id="0b8f5-184">reserved</span></span> | <span data-ttu-id="0b8f5-185">Комната доступна только в первый поступающий, первый обслуживаемый.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-185">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="0b8f5-186">Оно не может быть зарезервировано.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-186">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b8f5-187">Связи</span><span class="sxs-lookup"><span data-stu-id="0b8f5-187">Relationships</span></span>

<span data-ttu-id="0b8f5-188">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-188">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b8f5-189">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0b8f5-189">JSON representation</span></span>

<span data-ttu-id="0b8f5-190">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-190">The following is a JSON representation of the resource.</span></span>

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
