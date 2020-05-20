---
title: Список мест
description: Получение списка объектов Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5344d1ffda70a9b2e9dd23d950319acbacc5482a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290274"
---
# <a name="list-places"></a><span data-ttu-id="1ef44-103">Список мест</span><span class="sxs-lookup"><span data-stu-id="1ef44-103">List places</span></span>

<span data-ttu-id="1ef44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef44-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="1ef44-105">Получение коллекции указанного типа объектов [Place](../resources/place.md) , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1ef44-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="1ef44-106">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1ef44-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="1ef44-107">Объект **Place** может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="1ef44-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="1ef44-108">[Комната](../resources/room.md) , включающая в себя обширные свойства, такие как адрес электронной почты для комнаты, Специальные возможности, мощность и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="1ef44-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="1ef44-109">[Список помещений](../resources/roomlist.md) , включающий адрес электронной почты для списка помещений, и свойство навигации для получения коллекции экземпляров комнаты в списке помещений.</span><span class="sxs-lookup"><span data-stu-id="1ef44-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="1ef44-110">**Комната** и **RoomList принимают одиночные** являются производными от объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="1ef44-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="1ef44-111">По умолчанию эта операция возвращает число почтовых мест в 100 на страницу.</span><span class="sxs-lookup"><span data-stu-id="1ef44-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="1ef44-112">В сравнении с функциями [финдрумс](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) и [финдрумлистс](https://docs.microsoft.com/graph/api/user-findroomlists?view=graph-rest-beta) эта операция возвращает расширенные полезные данные для комнат и списков помещений.</span><span class="sxs-lookup"><span data-stu-id="1ef44-112">Compared with the [findRooms](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) and [findRoomLists](https://docs.microsoft.com/graph/api/user-findroomlists?view=graph-rest-beta) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="1ef44-113">Подробнее [о](../resources/place.md#using-the-places-api) том, как они сравниваются.</span><span class="sxs-lookup"><span data-stu-id="1ef44-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef44-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef44-114">Permissions</span></span>

<span data-ttu-id="1ef44-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ef44-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef44-117">Permission type</span></span>                        | <span data-ttu-id="1ef44-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ef44-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ef44-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ef44-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ef44-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ef44-120">Place.Read.All</span></span> |
| <span data-ttu-id="1ef44-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ef44-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef44-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1ef44-122">Not supported</span></span> |
| <span data-ttu-id="1ef44-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ef44-123">Application</span></span>                            | <span data-ttu-id="1ef44-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ef44-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef44-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ef44-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="1ef44-126">Чтобы получить все комнаты в клиенте, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1ef44-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="1ef44-127">Получение всех списков помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="1ef44-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="1ef44-128">Чтобы получить все комнаты в указанном списке помещений, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="1ef44-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="1ef44-129">**Note**: для получения комнат в списке помещений необходимо указать список помещений по свойству **EmailAddress** , а не по **идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="1ef44-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="1ef44-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ef44-130">Optional query parameters</span></span>
<span data-ttu-id="1ef44-131">Этот метод поддерживает следующие параметры запроса, помогающие настроить ответ:</span><span class="sxs-lookup"><span data-stu-id="1ef44-131">This method supports the following query parameters to help customize the response:</span></span>
- `$filter`
- `$select`
- `$top`
- `$skip`
- `$count=true`

<span data-ttu-id="1ef44-132">Используется `$top` для настройки размера страницы.</span><span class="sxs-lookup"><span data-stu-id="1ef44-132">Use `$top` to customize the page size.</span></span> <span data-ttu-id="1ef44-133">Размер страницы по умолчанию — 100.</span><span class="sxs-lookup"><span data-stu-id="1ef44-133">The default page size is 100.</span></span>

<span data-ttu-id="1ef44-134">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1ef44-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ef44-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ef44-135">Request headers</span></span>

| <span data-ttu-id="1ef44-136">Имя</span><span class="sxs-lookup"><span data-stu-id="1ef44-136">Name</span></span>          | <span data-ttu-id="1ef44-137">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef44-137">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1ef44-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ef44-138">Authorization</span></span> | <span data-ttu-id="1ef44-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ef44-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef44-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ef44-141">Request body</span></span>

<span data-ttu-id="1ef44-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ef44-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ef44-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef44-143">Response</span></span>

<span data-ttu-id="1ef44-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ef44-144">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ef44-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ef44-145">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="1ef44-146">Пример 1: список всех комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="1ef44-146">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1ef44-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef44-147">Request</span></span>

<span data-ttu-id="1ef44-148">В приведенном ниже примере показано, как получить все объекты [комнаты](../resources/room.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1ef44-148">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.room
```

#### <a name="response"></a><span data-ttu-id="1ef44-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef44-149">Response</span></span>

<span data-ttu-id="1ef44-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ef44-150">The following is an example of the response.</span></span>

><span data-ttu-id="1ef44-151">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ef44-151">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ef44-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ef44-152">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_rooms",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.room",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
      "emailAddress": "cf100@contoso.com",
      "displayName": "Conf Room 100",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488626,
        "longitude": -122.1293731033803
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "100",
      "capacity": "50",
      "building": "1",
      "floorNumber": 1,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "bean bags"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    },
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="1ef44-153">Пример 2: список всех списков помещений, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="1ef44-153">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1ef44-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef44-154">Request</span></span>

<span data-ttu-id="1ef44-155">В приведенном ниже примере показано, как получить все объекты [RoomList принимают одиночные](../resources/roomlist.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1ef44-155">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.roomlist
```

#### <a name="response"></a><span data-ttu-id="1ef44-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef44-156">Response</span></span>

<span data-ttu-id="1ef44-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ef44-157">The following is an example of the response.</span></span>

><span data-ttu-id="1ef44-158">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ef44-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ef44-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ef44-159">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_roomlists",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.roomList",
  "value": [
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
      "displayName": "Building 1",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg1@contoso.com"
    },
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1706",
      "displayName": "Building 2",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg2@contoso.com"
    }
  ]
}
```

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="1ef44-160">Пример 3: список комнат, включенных в список помещений</span><span class="sxs-lookup"><span data-stu-id="1ef44-160">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="1ef44-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef44-161">Request</span></span>

<span data-ttu-id="1ef44-162">В приведенном ниже примере показано, как получить список объектов [комнаты](../resources/room.md) , содержащийся в элементе **RoomList принимают одиночные**.</span><span class="sxs-lookup"><span data-stu-id="1ef44-162">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```

#### <a name="response"></a><span data-ttu-id="1ef44-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef44-163">Response</span></span>

<span data-ttu-id="1ef44-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ef44-164">The following is an example of the response.</span></span>

><span data-ttu-id="1ef44-165">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ef44-165">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ef44-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ef44-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_rooms_in_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List places",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Malformed function params 'id-of-roomlist'"
  ]
}-->
