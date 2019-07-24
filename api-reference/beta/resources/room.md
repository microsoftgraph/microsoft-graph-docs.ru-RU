---
title: Тип ресурса "комната"
description: Задает свойства комнаты в клиенте.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41c87daa31feda2907abab6f5711b4b88963095b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841292"
---
# <a name="room-resource-type"></a><span data-ttu-id="e5a95-103">Тип ресурса "комната"</span><span class="sxs-lookup"><span data-stu-id="e5a95-103">room resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5a95-104">Представляет комнату в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e5a95-104">Represents a room in a tenant.</span></span> 

<span data-ttu-id="e5a95-105">В Exchange Online каждая комната связана с почтовым ящиком комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-105">In Exchange Online, each room is associated with a room mailbox.</span></span> <span data-ttu-id="e5a95-106">Производный от [позиции](place.md).</span><span class="sxs-lookup"><span data-stu-id="e5a95-106">Derived from [place](place.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e5a95-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e5a95-107">Methods</span></span>

| <span data-ttu-id="e5a95-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e5a95-108">Method</span></span>                              | <span data-ttu-id="e5a95-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5a95-109">Return Type</span></span>                  | <span data-ttu-id="e5a95-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a95-110">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="e5a95-111">Список мест</span><span class="sxs-lookup"><span data-stu-id="e5a95-111">List places</span></span>](../api/place-list.md) | <span data-ttu-id="e5a95-112">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="e5a95-112">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="e5a95-113">Получение коллекции указанного типа объекта **Place** , определенного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e5a95-113">Get a collection of the specified type of **place** object defined in the tenant.</span></span> <span data-ttu-id="e5a95-114">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e5a95-114">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span> |
| [<span data-ttu-id="e5a95-115">Получение</span><span class="sxs-lookup"><span data-stu-id="e5a95-115">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="e5a95-116">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="e5a95-116">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="e5a95-117">Получение свойств и связей указанного объекта **Place** , например комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-117">Get the properties and relationships of the specified **place** object, such as a room.</span></span> |

## <a name="properties"></a><span data-ttu-id="e5a95-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5a95-118">Properties</span></span>

| <span data-ttu-id="e5a95-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5a95-119">Property</span></span>               | <span data-ttu-id="e5a95-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e5a95-120">Type</span></span>                                              | <span data-ttu-id="e5a95-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a95-121">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="e5a95-122">address</span><span class="sxs-lookup"><span data-stu-id="e5a95-122">address</span></span>                | [<span data-ttu-id="e5a95-123">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e5a95-123">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="e5a95-124">Почтовый адрес комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-124">The street address of the room.</span></span> |
| <span data-ttu-id="e5a95-125">Аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="e5a95-125">audioDeviceName</span></span>        | <span data-ttu-id="e5a95-126">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-126">String</span></span>                                            | <span data-ttu-id="e5a95-127">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="e5a95-127">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="e5a95-128">Букингтипе</span><span class="sxs-lookup"><span data-stu-id="e5a95-128">bookingType</span></span>            | [<span data-ttu-id="e5a95-129">Букингтипе</span><span class="sxs-lookup"><span data-stu-id="e5a95-129">bookingType</span></span>](#bookingtype-values)                | <span data-ttu-id="e5a95-130">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-130">Type of room.</span></span> <span data-ttu-id="e5a95-131">Возможные значения: `standard`, `managed` и `reserved`.</span><span class="sxs-lookup"><span data-stu-id="e5a95-131">Possible values are `standard`, `managed`, and `reserved`.</span></span> |
| <span data-ttu-id="e5a95-132">создания</span><span class="sxs-lookup"><span data-stu-id="e5a95-132">building</span></span>               | <span data-ttu-id="e5a95-133">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-133">String</span></span>                                            | <span data-ttu-id="e5a95-134">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="e5a95-134">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="e5a95-135">мощности</span><span class="sxs-lookup"><span data-stu-id="e5a95-135">capacity</span></span>               | <span data-ttu-id="e5a95-136">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-136">String</span></span>                                            | <span data-ttu-id="e5a95-137">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-137">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="e5a95-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e5a95-138">displayName</span></span>            | <span data-ttu-id="e5a95-139">Строка</span><span class="sxs-lookup"><span data-stu-id="e5a95-139">String</span></span>                                            | <span data-ttu-id="e5a95-140">Имя, связанное с комнатой.</span><span class="sxs-lookup"><span data-stu-id="e5a95-140">The name associated with the room.</span></span> |
| <span data-ttu-id="e5a95-141">Дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="e5a95-141">displayDeviceName</span></span>      | <span data-ttu-id="e5a95-142">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-142">String</span></span>                                            | <span data-ttu-id="e5a95-143">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="e5a95-143">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="e5a95-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e5a95-144">emailAddress</span></span>           | <span data-ttu-id="e5a95-145">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-145">String</span></span>                                            | <span data-ttu-id="e5a95-146">Адрес электронной почты комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-146">Email address of the room.</span></span> |
| <span data-ttu-id="e5a95-147">Флурнумбер</span><span class="sxs-lookup"><span data-stu-id="e5a95-147">floorNumber</span></span>            | <span data-ttu-id="e5a95-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e5a95-148">Int32</span></span>                                             | <span data-ttu-id="e5a95-149">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="e5a95-149">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="e5a95-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="e5a95-150">geoCoordinates</span></span>         | [<span data-ttu-id="e5a95-151">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="e5a95-151">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="e5a95-152">Указывает расположение комнаты в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-152">Specifies the room location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="e5a95-153">id</span><span class="sxs-lookup"><span data-stu-id="e5a95-153">id</span></span>                     | <span data-ttu-id="e5a95-154">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-154">String</span></span>                                            | <span data-ttu-id="e5a95-155">Уникальный идентификатор комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-155">Unique identifier for the room.</span></span> <span data-ttu-id="e5a95-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5a95-156">Read-only.</span></span> |
| <span data-ttu-id="e5a95-157">Исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="e5a95-157">isWheelchairAccessible</span></span> | <span data-ttu-id="e5a95-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5a95-158">Boolean</span></span>                                           | <span data-ttu-id="e5a95-159">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="e5a95-159">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="e5a95-160">label</span><span class="sxs-lookup"><span data-stu-id="e5a95-160">label</span></span>                  | <span data-ttu-id="e5a95-161">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-161">String</span></span>                                            | <span data-ttu-id="e5a95-162">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="e5a95-162">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="e5a95-163">прозвищ</span><span class="sxs-lookup"><span data-stu-id="e5a95-163">nickname</span></span>               | <span data-ttu-id="e5a95-164">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-164">String</span></span>                                            | <span data-ttu-id="e5a95-165">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="e5a95-165">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="e5a95-166">phone</span><span class="sxs-lookup"><span data-stu-id="e5a95-166">phone</span></span>                  | <span data-ttu-id="e5a95-167">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-167">String</span></span>                                            | <span data-ttu-id="e5a95-168">Номер телефона комнаты.</span><span class="sxs-lookup"><span data-stu-id="e5a95-168">The phone number of the room.</span></span> |
| <span data-ttu-id="e5a95-169">tags</span><span class="sxs-lookup"><span data-stu-id="e5a95-169">tags</span></span>                   | <span data-ttu-id="e5a95-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5a95-170">String collection</span></span>                                 | <span data-ttu-id="e5a95-171">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="e5a95-171">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="e5a95-172">Видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="e5a95-172">videoDeviceName</span></span>        | <span data-ttu-id="e5a95-173">String</span><span class="sxs-lookup"><span data-stu-id="e5a95-173">String</span></span>                                            | <span data-ttu-id="e5a95-174">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="e5a95-174">Specifies the name of the video device in the room.</span></span> |

### <a name="bookingtype-values"></a><span data-ttu-id="e5a95-175">значения Букингтипе</span><span class="sxs-lookup"><span data-stu-id="e5a95-175">bookingType values</span></span>

| <span data-ttu-id="e5a95-176">Значение</span><span class="sxs-lookup"><span data-stu-id="e5a95-176">Value</span></span>    | <span data-ttu-id="e5a95-177">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a95-177">Description</span></span>                                               |
|:---------|:----------------------------------------------------------|
| <span data-ttu-id="e5a95-178">Стандартный</span><span class="sxs-lookup"><span data-stu-id="e5a95-178">standard</span></span> | <span data-ttu-id="e5a95-179">Комнату можно зарезервировать в соответствии с другими параметрами в этом командлете.</span><span class="sxs-lookup"><span data-stu-id="e5a95-179">The room can be reserved based on the other settings in this cmdlet.</span></span> <span data-ttu-id="e5a95-180">Для сообщений, отправляемых почтовому пользователю или почтовому контакту, используется формат, настроенный для почтового пользователя или почтового контакта.</span><span class="sxs-lookup"><span data-stu-id="e5a95-180">This is the default value.</span></span> |
| <span data-ttu-id="e5a95-181">которыми</span><span class="sxs-lookup"><span data-stu-id="e5a95-181">managed</span></span>  | <span data-ttu-id="e5a95-182">Комната управляется представителем</span><span class="sxs-lookup"><span data-stu-id="e5a95-182">The room is managed by a delegate</span></span>                         |
| <span data-ttu-id="e5a95-183">резервирования</span><span class="sxs-lookup"><span data-stu-id="e5a95-183">reserved</span></span> | <span data-ttu-id="e5a95-184">Комната доступна только в первый поступающий, первый обслуживаемый.</span><span class="sxs-lookup"><span data-stu-id="e5a95-184">The room is available only on a first come, first served basis.</span></span> <span data-ttu-id="e5a95-185">Оно не может быть зарезервировано.</span><span class="sxs-lookup"><span data-stu-id="e5a95-185">It cannot be reserved.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5a95-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="e5a95-186">Relationships</span></span>

<span data-ttu-id="e5a95-187">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5a95-187">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5a95-188">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5a95-188">JSON representation</span></span>

<span data-ttu-id="e5a95-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5a95-189">The following is a JSON representation of the resource.</span></span>

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
