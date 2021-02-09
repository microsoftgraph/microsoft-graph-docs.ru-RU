---
title: Тип ресурса place
description: Представляет место. Это базовый тип для помещения или roomList.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8b9f7d21212c6551201b7ce83ba6c8f11edffa98
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161133"
---
# <a name="place-resource-type"></a><span data-ttu-id="6eb58-104">Тип ресурса place</span><span class="sxs-lookup"><span data-stu-id="6eb58-104">place resource type</span></span>

<span data-ttu-id="6eb58-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb58-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb58-106">Представляет базовые атрибуты расположения, такие как имя, физический адрес и географические координаты.</span><span class="sxs-lookup"><span data-stu-id="6eb58-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="6eb58-107">Это базовый тип для более богатых типов расположения, таких как [room](room.md) и [roomList.](roomlist.md)</span><span class="sxs-lookup"><span data-stu-id="6eb58-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="6eb58-108">Использование API мест</span><span class="sxs-lookup"><span data-stu-id="6eb58-108">Using the places API</span></span>
<span data-ttu-id="6eb58-109">Администраторы Exchange Online могут упорядоизировать комнаты для собраний в клиенте в списки помещений.</span><span class="sxs-lookup"><span data-stu-id="6eb58-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="6eb58-110">С помощью API мест можно получить все списки помещений или помещения в клиенте или получить все комнаты в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="6eb58-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="6eb58-111">Такие [места, как помещение](room.md) [и список помещений,](roomlist.md) содержат базовый **ид,** отображаемую и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6eb58-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="6eb58-112">Кроме того, они содержат навигационную информацию, например физический адрес и географические координаты, а в случае помещений — другую релевантную информацию, например возможности av, номер этажа и емкость.</span><span class="sxs-lookup"><span data-stu-id="6eb58-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="6eb58-113">Функции [findRooms](../api/user-findrooms.md) и [findRoomLists](../api/user-findroomlists.md) поддерживают аналогичный поиск помещений и списков помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6eb58-113">The [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="6eb58-114">Ниже приводится сравнение API мест и этих функций.</span><span class="sxs-lookup"><span data-stu-id="6eb58-114">The following is a comparison between the places API and these functions.</span></span>  <span data-ttu-id="6eb58-115">Если вы создаете производственное приложение, выберите API мест, так как API теперь общедоступн в v1.0.</span><span class="sxs-lookup"><span data-stu-id="6eb58-115">If you are creating a production app, choose the places API as the API is now generally available in v1.0.</span></span> <span data-ttu-id="6eb58-116">Запланируйте обновление существующего кода, который использует **findRooms** или **findRoomLists** для использования API мест, так как **findRooms** или **findRoomLists** будут объявлены как неподготовленные, а временная шкала будет объявлена.</span><span class="sxs-lookup"><span data-stu-id="6eb58-116">Plan to update any existing code that uses **findRooms** or **findRoomLists** to use the places API, because **findRooms** or **findRoomLists** will be deprecated, and a timeline will be announced.</span></span>

|<span data-ttu-id="6eb58-117">API Мест</span><span class="sxs-lookup"><span data-stu-id="6eb58-117">Places API</span></span> |<span data-ttu-id="6eb58-118">Функции findRooms и findRoomLists</span><span class="sxs-lookup"><span data-stu-id="6eb58-118">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="6eb58-119">Поддерживает получение всех помещений или списков помещений в клиенте и всех помещений в списке помещений</span><span class="sxs-lookup"><span data-stu-id="6eb58-119">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="6eb58-120">Аналогичная поддержка — получить все комнаты или списки помещений в клиенте и все комнаты в списке помещений</span><span class="sxs-lookup"><span data-stu-id="6eb58-120">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="6eb58-121">[Список мест](../api/place-list.md) может возвращать более 100 помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-121">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="6eb58-122">[FindRooms](../api/user-findrooms.md) возвращает до первых 100 помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-122">[findRooms](../api/user-findrooms.md) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="6eb58-123">Поддерживает получение [отдельного списка помещений или помещений](../api/place-get.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-123">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="6eb58-124">Не поддерживает получение отдельного списка помещений или помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-124">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="6eb58-125">Определяет конкретные сущности объекта [room](room.md) и [roomList,](roomlist.md) которые указывают более богатый набор свойств в дополнение к отображаемого имени и SMTP-адресу.</span><span class="sxs-lookup"><span data-stu-id="6eb58-125">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="6eb58-126">Каждый список помещений и помещений имеет облегченный тип [emailAddress,](emailaddress.md) который указывает только отображаемую и SMTP-адрес</span><span class="sxs-lookup"><span data-stu-id="6eb58-126">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="6eb58-127">Поддерживает только организационные сценарии с делегными (учетными записями для работы или учебного заведения) или разрешениями приложения</span><span class="sxs-lookup"><span data-stu-id="6eb58-127">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="6eb58-128">Аналогичная поддержка только организационных сценариев с делегными разрешениями или разрешениями приложений</span><span class="sxs-lookup"><span data-stu-id="6eb58-128">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="6eb58-129">Поддерживает обновление [отдельного списка помещений](../api/place-update.md) или помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-129">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="6eb58-130">Не поддерживает обновление отдельного списка помещений или помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="6eb58-130">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="6eb58-131">Методы</span><span class="sxs-lookup"><span data-stu-id="6eb58-131">Methods</span></span>

| <span data-ttu-id="6eb58-132">Метод</span><span class="sxs-lookup"><span data-stu-id="6eb58-132">Method</span></span>                              | <span data-ttu-id="6eb58-133">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6eb58-133">Return Type</span></span>                  | <span data-ttu-id="6eb58-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb58-134">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="6eb58-135">Места списка</span><span class="sxs-lookup"><span data-stu-id="6eb58-135">List places</span></span>](../api/place-list.md) | <span data-ttu-id="6eb58-136">Коллекция запрашиваемого производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="6eb58-136">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="6eb58-137">Получите коллекцию объектов указанного типа **мест,** определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6eb58-137">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="6eb58-138">Получить место</span><span class="sxs-lookup"><span data-stu-id="6eb58-138">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="6eb58-139">Запрашиваемая производная тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="6eb58-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="6eb58-140">Получить свойства и связи объекта **указанного** места.</span><span class="sxs-lookup"><span data-stu-id="6eb58-140">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="6eb58-141">Место обновления</span><span class="sxs-lookup"><span data-stu-id="6eb58-141">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="6eb58-142">Запрашиваемая производная тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="6eb58-142">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="6eb58-143">Обновление свойств и связей объекта **указанного** места.</span><span class="sxs-lookup"><span data-stu-id="6eb58-143">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6eb58-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb58-144">Properties</span></span>

| <span data-ttu-id="6eb58-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb58-145">Property</span></span>       | <span data-ttu-id="6eb58-146">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb58-146">Type</span></span>                                              | <span data-ttu-id="6eb58-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb58-147">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="6eb58-148">address</span><span class="sxs-lookup"><span data-stu-id="6eb58-148">address</span></span>        | [<span data-ttu-id="6eb58-149">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6eb58-149">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="6eb58-150">Адрес улицы.</span><span class="sxs-lookup"><span data-stu-id="6eb58-150">The street address of the place.</span></span> |
| <span data-ttu-id="6eb58-151">displayName</span><span class="sxs-lookup"><span data-stu-id="6eb58-151">displayName</span></span>    | <span data-ttu-id="6eb58-152">String</span><span class="sxs-lookup"><span data-stu-id="6eb58-152">String</span></span>                                            | <span data-ttu-id="6eb58-153">Имя, связанное с местом.</span><span class="sxs-lookup"><span data-stu-id="6eb58-153">The name associated with the place.</span></span> |
| <span data-ttu-id="6eb58-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6eb58-154">geoCoordinates</span></span> | [<span data-ttu-id="6eb58-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6eb58-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="6eb58-156">Указывает расположение в широте, долготе и (необязательно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="6eb58-156">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="6eb58-157">id</span><span class="sxs-lookup"><span data-stu-id="6eb58-157">id</span></span>             | <span data-ttu-id="6eb58-158">String</span><span class="sxs-lookup"><span data-stu-id="6eb58-158">String</span></span>                                            | <span data-ttu-id="6eb58-159">Уникальный идентификатор для места.</span><span class="sxs-lookup"><span data-stu-id="6eb58-159">Unique identifier for the place.</span></span> <span data-ttu-id="6eb58-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6eb58-160">Read-only.</span></span> |
| <span data-ttu-id="6eb58-161">phone</span><span class="sxs-lookup"><span data-stu-id="6eb58-161">phone</span></span>          | <span data-ttu-id="6eb58-162">String</span><span class="sxs-lookup"><span data-stu-id="6eb58-162">String</span></span>                                            | <span data-ttu-id="6eb58-163">Номер телефона места.</span><span class="sxs-lookup"><span data-stu-id="6eb58-163">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6eb58-164">Связи</span><span class="sxs-lookup"><span data-stu-id="6eb58-164">Relationships</span></span>

<span data-ttu-id="6eb58-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6eb58-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eb58-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6eb58-166">JSON representation</span></span>

<span data-ttu-id="6eb58-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb58-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place"
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

## <a name="see-also"></a><span data-ttu-id="6eb58-168">См. также</span><span class="sxs-lookup"><span data-stu-id="6eb58-168">See also</span></span>
- <span data-ttu-id="6eb58-169">Чтобы администраторы создали список помещений, используйте в Exchange PowerShell cmdlet [New-DistributionGroup.](/powershell/module/exchange/users-and-groups/new-distributiongroup)</span><span class="sxs-lookup"><span data-stu-id="6eb58-169">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup).</span></span>
- <span data-ttu-id="6eb58-170">Чтобы администраторы добавили комнату в список помещений, используйте с помощью cmdlet Exchange Powershell [Add-DistributionGroupMember.](/powershell/module/exchange/users-and-groups/add-distributiongroupmember)</span><span class="sxs-lookup"><span data-stu-id="6eb58-170">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
