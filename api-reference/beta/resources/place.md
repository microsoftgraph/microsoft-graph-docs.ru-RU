---
title: размещение типа ресурса
description: Представляет место. Это базовый тип для комнаты или RoomList принимают одиночные.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ea1736e0215b411673f8c458f79c57181312a25a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521844"
---
# <a name="place-resource-type"></a><span data-ttu-id="2c8e3-104">размещение типа ресурса</span><span class="sxs-lookup"><span data-stu-id="2c8e3-104">place resource type</span></span>

<span data-ttu-id="2c8e3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c8e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c8e3-106">Представляет основные атрибуты расположения, такие как имя, физический адрес и географические координаты.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="2c8e3-107">Это базовый тип для расширенных типов расположения, таких как [комната](room.md) и [RoomList принимают одиночные](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="2c8e3-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="2c8e3-108">Использование API мест</span><span class="sxs-lookup"><span data-stu-id="2c8e3-108">Using the places API</span></span>
<span data-ttu-id="2c8e3-109">Администраторы Exchange Online могут организовывать комнаты собраний в клиенте в списки помещений.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="2c8e3-110">С помощью API мест можно получить все списки помещений или комнаты в клиенте или получить все комнаты в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="2c8e3-111">Места, такие как [комната](room.md) и [RoomList принимают одиночные](roomlist.md) , содержат базовый **идентификатор**, отображаемое имя и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="2c8e3-112">Кроме того, они содержат сведения о переходах, такие как физический адрес и географические координаты, а также в случае комнат, а также другие релевантные сведения, такие как возможности AV, номер этажа и мощность.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="2c8e3-113">Функции [финдрумс](../api/user-findrooms.md) и [финдрумлистс](../api/user-findroomlists.md) поддерживают подобный Поиск комнат и списков помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-113">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="2c8e3-114">Ниже приведено сравнение между API мест и этими функциями.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-114">The following is a comparison between the places API and these functions.</span></span>

|<span data-ttu-id="2c8e3-115">API мест</span><span class="sxs-lookup"><span data-stu-id="2c8e3-115">Places API</span></span> |<span data-ttu-id="2c8e3-116">функции Финдрумс и Финдрумлистс</span><span class="sxs-lookup"><span data-stu-id="2c8e3-116">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="2c8e3-117">Поддерживает извлечение всех помещений или списков помещений в клиенте, а также всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="2c8e3-117">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="2c8e3-118">Подобная поддержка — получение всех помещений или списков помещений в клиенте и всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="2c8e3-118">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="2c8e3-119">[Места в списке](../api/place-list.md) могут возвращать более 100 комнат в клиенте</span><span class="sxs-lookup"><span data-stu-id="2c8e3-119">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="2c8e3-120">[финдрумс](../api/user-findrooms.md) возвращает до первых 100 комнат в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-120">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="2c8e3-121">Поддерживает [Извлечение отдельных помещений или списка помещений](../api/place-get.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="2c8e3-121">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="2c8e3-122">Не поддерживает извлечение отдельного помещения или списка помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="2c8e3-122">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="2c8e3-123">Определяет конкретные объекты [комнаты](room.md) и [RoomList принимают одиночные](roomlist.md) , которые задают набор свойств с более широкими возможностями, в дополнение к ОТОБРАЖАЕМОМУ имени и SMTP-адресу.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-123">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="2c8e3-124">Каждая комната и список помещений имеют более легкий тип [EmailAddress](emailaddress.md) , который указывает только отображаемое имя и SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-124">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="2c8e3-125">Поддерживает только организационные сценарии с делегированными (рабочими или учебными учетными записями) или разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-125">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="2c8e3-126">Подобная поддержка только для организационных сценариев с делегированными разрешениями или приложениями</span><span class="sxs-lookup"><span data-stu-id="2c8e3-126">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="2c8e3-127">Поддерживает [обновление отдельных помещений или списка помещений](../api/place-update.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="2c8e3-127">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="2c8e3-128">Не поддерживает обновление отдельных помещений или списка помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="2c8e3-128">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="2c8e3-129">Методы</span><span class="sxs-lookup"><span data-stu-id="2c8e3-129">Methods</span></span>

| <span data-ttu-id="2c8e3-130">Метод</span><span class="sxs-lookup"><span data-stu-id="2c8e3-130">Method</span></span>                              | <span data-ttu-id="2c8e3-131">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c8e3-131">Return Type</span></span>                  | <span data-ttu-id="2c8e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c8e3-132">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="2c8e3-133">Список мест</span><span class="sxs-lookup"><span data-stu-id="2c8e3-133">List places</span></span>](../api/place-list.md) | <span data-ttu-id="2c8e3-134">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="2c8e3-134">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="2c8e3-135">Получение коллекции указанного типа объектов **Place** , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-135">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="2c8e3-136">Получение</span><span class="sxs-lookup"><span data-stu-id="2c8e3-136">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="2c8e3-137">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="2c8e3-137">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="2c8e3-138">Получение свойств и связей указанного объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="2c8e3-138">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="2c8e3-139">Обновление места</span><span class="sxs-lookup"><span data-stu-id="2c8e3-139">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="2c8e3-140">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="2c8e3-140">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="2c8e3-141">Обновление свойств и связей указанного объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="2c8e3-141">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c8e3-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c8e3-142">Properties</span></span>

| <span data-ttu-id="2c8e3-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c8e3-143">Property</span></span>       | <span data-ttu-id="2c8e3-144">Тип</span><span class="sxs-lookup"><span data-stu-id="2c8e3-144">Type</span></span>                                              | <span data-ttu-id="2c8e3-145">Описание</span><span class="sxs-lookup"><span data-stu-id="2c8e3-145">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="2c8e3-146">address</span><span class="sxs-lookup"><span data-stu-id="2c8e3-146">address</span></span>        | [<span data-ttu-id="2c8e3-147">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2c8e3-147">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="2c8e3-148">Адрес в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-148">The street address of the place.</span></span> |
| <span data-ttu-id="2c8e3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2c8e3-149">displayName</span></span>    | <span data-ttu-id="2c8e3-150">Строка</span><span class="sxs-lookup"><span data-stu-id="2c8e3-150">String</span></span>                                            | <span data-ttu-id="2c8e3-151">Имя, связанное с местом.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-151">The name associated with the place.</span></span> |
| <span data-ttu-id="2c8e3-152">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2c8e3-152">geoCoordinates</span></span> | [<span data-ttu-id="2c8e3-153">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2c8e3-153">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="2c8e3-154">Указывает положение места в широте, долготе и (дополнительно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-154">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="2c8e3-155">id</span><span class="sxs-lookup"><span data-stu-id="2c8e3-155">id</span></span>             | <span data-ttu-id="2c8e3-156">String</span><span class="sxs-lookup"><span data-stu-id="2c8e3-156">String</span></span>                                            | <span data-ttu-id="2c8e3-157">Уникальный идентификатор для места.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-157">Unique identifier for the place.</span></span> <span data-ttu-id="2c8e3-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-158">Read-only.</span></span> |
| <span data-ttu-id="2c8e3-159">phone</span><span class="sxs-lookup"><span data-stu-id="2c8e3-159">phone</span></span>          | <span data-ttu-id="2c8e3-160">String</span><span class="sxs-lookup"><span data-stu-id="2c8e3-160">String</span></span>                                            | <span data-ttu-id="2c8e3-161">Номер телефона для места.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-161">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c8e3-162">Связи</span><span class="sxs-lookup"><span data-stu-id="2c8e3-162">Relationships</span></span>

<span data-ttu-id="2c8e3-163">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-163">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8e3-164">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2c8e3-164">JSON representation</span></span>

<span data-ttu-id="2c8e3-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a><span data-ttu-id="2c8e3-166">См. также</span><span class="sxs-lookup"><span data-stu-id="2c8e3-166">See also</span></span>
- <span data-ttu-id="2c8e3-167">Чтобы создать список помещений для администраторов, используйте командлет Exchange PowerShell [New – DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="2c8e3-167">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="2c8e3-168">Чтобы добавить конференцию в список помещений, используйте командлет [Add – DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)для Exchange PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2c8e3-168">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
