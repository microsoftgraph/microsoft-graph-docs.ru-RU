---
title: размещение типа ресурса
description: Представляет место. Это базовый тип для комнаты или RoomList принимают одиночные.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3df3d2438b9f7f0413b8005da08a9e7843436adc
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290380"
---
# <a name="place-resource-type"></a><span data-ttu-id="adb01-104">размещение типа ресурса</span><span class="sxs-lookup"><span data-stu-id="adb01-104">place resource type</span></span>

<span data-ttu-id="adb01-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adb01-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adb01-106">Представляет основные атрибуты расположения, такие как имя, физический адрес и географические координаты.</span><span class="sxs-lookup"><span data-stu-id="adb01-106">Represents basic location attributes such as name, physical address, and geographic coordinates.</span></span> <span data-ttu-id="adb01-107">Это базовый тип для расширенных типов расположения, таких как [комната](room.md) и [RoomList принимают одиночные](roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="adb01-107">This is the base type for richer location types such as [room](room.md) and [roomList](roomlist.md).</span></span>

### <a name="using-the-places-api"></a><span data-ttu-id="adb01-108">Использование API мест</span><span class="sxs-lookup"><span data-stu-id="adb01-108">Using the places API</span></span>
<span data-ttu-id="adb01-109">Администраторы Exchange Online могут организовывать комнаты собраний в клиенте в списки помещений.</span><span class="sxs-lookup"><span data-stu-id="adb01-109">Exchange Online administrators can organize meeting rooms in a tenant into room lists.</span></span> <span data-ttu-id="adb01-110">С помощью API мест можно получить все списки помещений или комнаты в клиенте или получить все комнаты в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="adb01-110">Using the places API, you can get all the room lists or rooms in the tenant, or get all the rooms in a specific room list.</span></span>

<span data-ttu-id="adb01-111">Места, такие как [комната](room.md) и [RoomList принимают одиночные](roomlist.md) , содержат базовый **идентификатор**, отображаемое имя и адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="adb01-111">Places like [room](room.md) and [roomList](roomlist.md) contain the basic **id**, display name and email address.</span></span> <span data-ttu-id="adb01-112">Кроме того, они содержат сведения о переходах, такие как физический адрес и географические координаты, а также в случае комнат, а также другие релевантные сведения, такие как возможности AV, номер этажа и мощность.</span><span class="sxs-lookup"><span data-stu-id="adb01-112">In addition, they contain navigational information like physical address and geographical coordinates, and in the case of rooms, other relevant information such as AV capabilities, floor number, and capacity.</span></span>

<span data-ttu-id="adb01-113">Функции [финдрумс](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) и [финдрумлистс](https://docs.microsoft.com/en-us/graph/api/user-findroomlists?view=graph-rest-beta) поддерживают подобный Поиск комнат и списков помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="adb01-113">The [findRooms](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) and [findRoomLists](https://docs.microsoft.com/en-us/graph/api/user-findroomlists?view=graph-rest-beta) functions support similar lookup for rooms and room lists in a tenant.</span></span> <span data-ttu-id="adb01-114">Ниже приведено сравнение между API мест и этими функциями.</span><span class="sxs-lookup"><span data-stu-id="adb01-114">The following is a comparison between the places API and these functions.</span></span>  <span data-ttu-id="adb01-115">Если вы создаете рабочее приложение, выберите API "места", так как API теперь доступен в версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="adb01-115">If you are creating a production app, choose the places API as the API is now generally available in v1.0.</span></span> <span data-ttu-id="adb01-116">Запланируйте обновление существующего кода, использующего **финдрумс** или **финдрумлистс** , для использования API мест, так как **финдрумс** или **финдрумлистс** будут устаревшими, а временная шкала будет объявлена.</span><span class="sxs-lookup"><span data-stu-id="adb01-116">Plan to update any existing code that uses **findRooms** or **findRoomLists** to use the places API, because **findRooms** or **findRoomLists** will be deprecated, and a timeline will be announced.</span></span>

|<span data-ttu-id="adb01-117">API мест</span><span class="sxs-lookup"><span data-stu-id="adb01-117">Places API</span></span> |<span data-ttu-id="adb01-118">функции Финдрумс и Финдрумлистс</span><span class="sxs-lookup"><span data-stu-id="adb01-118">findRooms and findRoomLists functions</span></span>|
|:------------------------------------|:-----------------------------|
|<span data-ttu-id="adb01-119">Поддерживает извлечение всех помещений или списков помещений в клиенте, а также всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="adb01-119">Supports getting all the rooms or room lists in a tenant, and all the rooms in a room list</span></span> | <span data-ttu-id="adb01-120">Подобная поддержка — получение всех помещений или списков помещений в клиенте и всех комнат в списке помещений</span><span class="sxs-lookup"><span data-stu-id="adb01-120">Similar support - get all the rooms or room lists in a tenant, and all the rooms in a room list</span></span>|
|<span data-ttu-id="adb01-121">[Места в списке](../api/place-list.md) могут возвращать более 100 комнат в клиенте</span><span class="sxs-lookup"><span data-stu-id="adb01-121">[List places](../api/place-list.md) can return more than 100 rooms in a tenant</span></span> | <span data-ttu-id="adb01-122">[финдрумс](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) возвращает до первых 100 комнат в клиенте.</span><span class="sxs-lookup"><span data-stu-id="adb01-122">[findRooms](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) returns up to the first 100 rooms in a tenant</span></span> |
|<span data-ttu-id="adb01-123">Поддерживает [Извлечение отдельных помещений или списка помещений](../api/place-get.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="adb01-123">Supports [getting an individual room or room list](../api/place-get.md) in a tenant</span></span> | <span data-ttu-id="adb01-124">Не поддерживает извлечение отдельного помещения или списка помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="adb01-124">Does not support getting an individual room or room list in a tenant</span></span>
|<span data-ttu-id="adb01-125">Определяет конкретные объекты [комнаты](room.md) и [RoomList принимают одиночные](roomlist.md) , которые задают набор свойств с более широкими возможностями, в дополнение к ОТОБРАЖАЕМОМУ имени и SMTP-адресу.</span><span class="sxs-lookup"><span data-stu-id="adb01-125">Defines the specific entities of [room](room.md) and [roomList](roomlist.md) which specify a richer property set, in addition to the display name and SMTP address.</span></span> | <span data-ttu-id="adb01-126">Каждая комната и список помещений имеют более легкий тип [EmailAddress](emailaddress.md) , который указывает только отображаемое имя и SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="adb01-126">Each room and room list is of a lighter weight [emailAddress](emailaddress.md) type which specifies only the display name and SMTP address</span></span>|
|<span data-ttu-id="adb01-127">Поддерживает только организационные сценарии с делегированными (рабочими или учебными учетными записями) или разрешениями приложений.</span><span class="sxs-lookup"><span data-stu-id="adb01-127">Supports only organizational scenarios with delegated (work or school accounts) or application permissions</span></span> | <span data-ttu-id="adb01-128">Подобная поддержка только для организационных сценариев с делегированными разрешениями или приложениями</span><span class="sxs-lookup"><span data-stu-id="adb01-128">Similar support for only organizational scenarios with delegated or application permissions</span></span>|
|<span data-ttu-id="adb01-129">Поддерживает [обновление отдельных помещений или списка помещений](../api/place-update.md) в клиенте</span><span class="sxs-lookup"><span data-stu-id="adb01-129">Supports [updating an individual room or room list](../api/place-update.md) in a tenant</span></span> | <span data-ttu-id="adb01-130">Не поддерживает обновление отдельных помещений или списка помещений в клиенте</span><span class="sxs-lookup"><span data-stu-id="adb01-130">Does not support updating an individual room or room list in a tenant</span></span>

## <a name="methods"></a><span data-ttu-id="adb01-131">Методы</span><span class="sxs-lookup"><span data-stu-id="adb01-131">Methods</span></span>

| <span data-ttu-id="adb01-132">Метод</span><span class="sxs-lookup"><span data-stu-id="adb01-132">Method</span></span>                              | <span data-ttu-id="adb01-133">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="adb01-133">Return Type</span></span>                  | <span data-ttu-id="adb01-134">Описание</span><span class="sxs-lookup"><span data-stu-id="adb01-134">Description</span></span> |
|:------------------------------------|:-----------------------------|:--------|
| [<span data-ttu-id="adb01-135">Список мест</span><span class="sxs-lookup"><span data-stu-id="adb01-135">List places</span></span>](../api/place-list.md) | <span data-ttu-id="adb01-136">Коллекция запрошенного, производного типа [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="adb01-136">A collection of the requested, derived type of [place](place.md)</span></span> | <span data-ttu-id="adb01-137">Получение коллекции указанного типа объектов **Place** , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="adb01-137">Get a collection of the specified type of **place** objects defined in the tenant.</span></span> |
| [<span data-ttu-id="adb01-138">Получение</span><span class="sxs-lookup"><span data-stu-id="adb01-138">Get place</span></span>](../api/place-get.md)    | <span data-ttu-id="adb01-139">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="adb01-139">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="adb01-140">Получение свойств и связей указанного объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="adb01-140">Get the properties and relationships of a specified **place** object.</span></span> |
| [<span data-ttu-id="adb01-141">Обновление места</span><span class="sxs-lookup"><span data-stu-id="adb01-141">Update place</span></span>](../api/place-update.md)    | <span data-ttu-id="adb01-142">Запрошенный, производный тип [места](place.md)</span><span class="sxs-lookup"><span data-stu-id="adb01-142">The requested, derived type of [place](place.md)</span></span>            | <span data-ttu-id="adb01-143">Обновление свойств и связей указанного объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="adb01-143">Update the properties and relationships of a specified **place** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="adb01-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="adb01-144">Properties</span></span>

| <span data-ttu-id="adb01-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="adb01-145">Property</span></span>       | <span data-ttu-id="adb01-146">Тип</span><span class="sxs-lookup"><span data-stu-id="adb01-146">Type</span></span>                                              | <span data-ttu-id="adb01-147">Описание</span><span class="sxs-lookup"><span data-stu-id="adb01-147">Description</span></span> |
|:---------------|:--------------------------------------------------|:--------|
| <span data-ttu-id="adb01-148">address</span><span class="sxs-lookup"><span data-stu-id="adb01-148">address</span></span>        | [<span data-ttu-id="adb01-149">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="adb01-149">physicalAddress</span></span>](physicaladdress.md)             | <span data-ttu-id="adb01-150">Адрес в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="adb01-150">The street address of the place.</span></span> |
| <span data-ttu-id="adb01-151">displayName</span><span class="sxs-lookup"><span data-stu-id="adb01-151">displayName</span></span>    | <span data-ttu-id="adb01-152">Строка</span><span class="sxs-lookup"><span data-stu-id="adb01-152">String</span></span>                                            | <span data-ttu-id="adb01-153">Имя, связанное с местом.</span><span class="sxs-lookup"><span data-stu-id="adb01-153">The name associated with the place.</span></span> |
| <span data-ttu-id="adb01-154">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="adb01-154">geoCoordinates</span></span> | [<span data-ttu-id="adb01-155">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="adb01-155">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="adb01-156">Указывает положение места в широте, долготе и (дополнительно) координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="adb01-156">Specifies the place location in latitude, longitude and (optionally) altitude coordinates.</span></span> |
| <span data-ttu-id="adb01-157">id</span><span class="sxs-lookup"><span data-stu-id="adb01-157">id</span></span>             | <span data-ttu-id="adb01-158">String</span><span class="sxs-lookup"><span data-stu-id="adb01-158">String</span></span>                                            | <span data-ttu-id="adb01-159">Уникальный идентификатор для места.</span><span class="sxs-lookup"><span data-stu-id="adb01-159">Unique identifier for the place.</span></span> <span data-ttu-id="adb01-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adb01-160">Read-only.</span></span> |
| <span data-ttu-id="adb01-161">phone</span><span class="sxs-lookup"><span data-stu-id="adb01-161">phone</span></span>          | <span data-ttu-id="adb01-162">String</span><span class="sxs-lookup"><span data-stu-id="adb01-162">String</span></span>                                            | <span data-ttu-id="adb01-163">Номер телефона для места.</span><span class="sxs-lookup"><span data-stu-id="adb01-163">The phone number of the place.</span></span> |

## <a name="relationships"></a><span data-ttu-id="adb01-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="adb01-164">Relationships</span></span>

<span data-ttu-id="adb01-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="adb01-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adb01-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adb01-166">JSON representation</span></span>

<span data-ttu-id="adb01-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adb01-167">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="adb01-168">См. также</span><span class="sxs-lookup"><span data-stu-id="adb01-168">See also</span></span>
- <span data-ttu-id="adb01-169">Чтобы создать список помещений для администраторов, используйте командлет Exchange PowerShell [New – DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="adb01-169">For administrators to create a room list, use the Exchange PowerShell cmdlet [New-DistributionGroup](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps).</span></span>
- <span data-ttu-id="adb01-170">Чтобы добавить конференцию в список помещений, используйте командлет [Add – DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps)для Exchange PowerShell.</span><span class="sxs-lookup"><span data-stu-id="adb01-170">For administrators to add a room to a room list, use the Exchange Powershell cmdlet [Add-DistributionGroupMember](https://docs.microsoft.com/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps).</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
