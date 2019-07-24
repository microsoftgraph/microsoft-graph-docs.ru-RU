---
title: размещение типа ресурса
description: Представляет место. Это базовый тип для комнаты или RoomList принимают одиночные.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5cea04931d537c8b0bd29c49327a56afe8a7d5d5
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841299"
---
# <a name="place-resource-type"></a><span data-ttu-id="3dcaa-104">размещение типа ресурса</span><span class="sxs-lookup"><span data-stu-id="3dcaa-104">place resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dcaa-105">Представляет основные атрибуты расположения, такие как имя, физический адрес и географические координаты.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-105">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="3dcaa-106">Это базовый тип для расширенных типов расположения, таких как [комната](room.md) и [RoomList принимают одиночные](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="3dcaa-106">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="3dcaa-107">Использование API мест</span><span class="sxs-lookup"><span data-stu-id="3dcaa-107">Using the places API</span></span>
<span data-ttu-id="3dcaa-108">Администраторы Exchange Online могут организовывать комнаты собраний в клиенте в списки помещений.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-108">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="3dcaa-109">С помощью API мест можно получить все списки помещений или комнаты в клиенте или получить все комнаты в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-109">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="3dcaa-110">Места, такие как [комната](room.md) и [RoomList принимают одиночные](roomlist.md) , содержат базовый **идентификатор**, отображаемое имя и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-110">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="3dcaa-111">Кроме того, они содержат сведения о переходах, такие как физический адрес и географические координаты, а также в случае комнат, а также другие релевантные сведения, такие как возможности AV, номер этажа и мощность.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-111">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="3dcaa-112">Функции [финдрумс](../api/user-findrooms.md) и [финдрумлистс](../api/user-findroomlists.md) поддерживают подобный Поиск комнат и списков помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-112">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="3dcaa-113">Ниже приведено сравнение между API мест и этими функциями.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-113">The following is a comparison between the places API and these functions.</span></span>

|<span data-ttu-id="3dcaa-114">API мест</span><span class="sxs-lookup"><span data-stu-id="3dcaa-114">Places API</span></span> |<span data-ttu-id="3dcaa-115">функции Финдрумс и Финдрумлистс</span><span class="sxs-lookup"><span data-stu-id="3dcaa-115">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="3dcaa-116">Поддерживает извлечение всех помещений или списков помещений в клиенте, а также всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="3dcaa-116">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="3dcaa-117">Подобная поддержка — получение всех помещений или списков помещений в клиенте и всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="3dcaa-117">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="3dcaa-118">[Места в списке](../api/place-list.md) могут возвращать более 100 комнат в клиенте</span><span class="sxs-lookup"><span data-stu-id="3dcaa-118">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="3dcaa-119">[финдрумс](../api/user-findrooms.md) возвращает до первых 100 комнат в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-119">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="3dcaa-120">Поддерживает [Извлечение отдельных помещений или списка помещений](../api/place-get.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="3dcaa-120">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="3dcaa-121">Не поддерживает извлечение отдельного помещения или списка помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="3dcaa-121">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="3dcaa-122">Определяет конкретные объекты [комнаты](room.md) и [RoomList принимают одиночные](roomlist.md) , которые задают набор свойств с более широкими возможностями, в дополнение к ОТОБРАЖАЕМОМУ имени и SMTP-адресу.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-122">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="3dcaa-123">Каждая комната и список помещений имеют более легкий тип [EmailAddress](emailaddress.md) , который указывает только отображаемое имя и SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-123">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="3dcaa-124">Поддерживает только организационные сценарии с делегированными (рабочими или учебными учетными записями) или разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-124">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="3dcaa-125">Подобная поддержка только для организационных сценариев с делегированными разрешениями или приложениями</span><span class="sxs-lookup"><span data-stu-id="3dcaa-125">Similar support for only organizational scenarios with delegated or application permissions</span></span>|

## <a name="methods"></a><span data-ttu-id="3dcaa-126">Методы</span><span class="sxs-lookup"><span data-stu-id="3dcaa-126">Methods</span></span>

| <span data-ttu-id="3dcaa-127">Метод</span><span class="sxs-lookup"><span data-stu-id="3dcaa-127">Method</span></span>                              | <span data-ttu-id="3dcaa-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3dcaa-128">Return Type</span></span>                  | <span data-ttu-id="3dcaa-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3dcaa-129">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="3dcaa-130">Список мест</span><span class="sxs-lookup"><span data-stu-id="3dcaa-130">List places</span></span>](../api/place-list.md) | <span data-ttu-id="3dcaa-131">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="3dcaa-131">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="3dcaa-132">Получение коллекции указанного типа объектов **Place** , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-132">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="3dcaa-133">Получение</span><span class="sxs-lookup"><span data-stu-id="3dcaa-133">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="3dcaa-134">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="3dcaa-134">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="3dcaa-135">Получение свойств и связей указанного объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="3dcaa-135">Get the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3dcaa-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="3dcaa-136">Properties</span></span>

| <span data-ttu-id="3dcaa-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dcaa-137">Property</span></span>       | <span data-ttu-id="3dcaa-138">Тип</span><span class="sxs-lookup"><span data-stu-id="3dcaa-138">Type</span></span>                                              | <span data-ttu-id="3dcaa-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3dcaa-139">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="3dcaa-140">address</span><span class="sxs-lookup"><span data-stu-id="3dcaa-140">address</span></span>        | [<span data-ttu-id="3dcaa-141">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3dcaa-141">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="3dcaa-142">Адрес в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-142">The street address of the place.</span></span> |
| <span data-ttu-id="3dcaa-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3dcaa-143">displayName</span></span>    | <span data-ttu-id="3dcaa-144">Строка</span><span class="sxs-lookup"><span data-stu-id="3dcaa-144">String</span></span>                                            | <span data-ttu-id="3dcaa-145">Имя, связанное с местом.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-145">The name associated with the place.</span></span> |
| <span data-ttu-id="3dcaa-146">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3dcaa-146">geoCoordinates</span></span> | [<span data-ttu-id="3dcaa-147">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3dcaa-147">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="3dcaa-148">Указывает положение места в широте, долготе и (дополнительно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-148">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="3dcaa-149">id</span><span class="sxs-lookup"><span data-stu-id="3dcaa-149">id</span></span>             | <span data-ttu-id="3dcaa-150">String</span><span class="sxs-lookup"><span data-stu-id="3dcaa-150">String</span></span>                                            | <span data-ttu-id="3dcaa-151">Уникальный идентификатор для места.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-151">Unique identifier for the place.</span></span> <span data-ttu-id="3dcaa-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-152">Read-only.</span></span> |
| <span data-ttu-id="3dcaa-153">phone</span><span class="sxs-lookup"><span data-stu-id="3dcaa-153">phone</span></span>          | <span data-ttu-id="3dcaa-154">String</span><span class="sxs-lookup"><span data-stu-id="3dcaa-154">String</span></span>                                            | <span data-ttu-id="3dcaa-155">Номер телефона для места.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-155">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3dcaa-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="3dcaa-156">Relationships</span></span>

<span data-ttu-id="3dcaa-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dcaa-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3dcaa-158">JSON representation</span></span>

<span data-ttu-id="3dcaa-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-159">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3dcaa-160">См. также</span><span class="sxs-lookup"><span data-stu-id="3dcaa-160">See also</span></span>
- <span data-ttu-id="3dcaa-161">Чтобы создать список помещений для администраторов, используйте командлет Exchange PowerShell [New – DistributionGroup](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="3dcaa-161">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="3dcaa-162">Чтобы добавить конференцию в список помещений, используйте командлет [Add – DistributionGroupMember](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)для Exchange PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3dcaa-162">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/en-us/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
