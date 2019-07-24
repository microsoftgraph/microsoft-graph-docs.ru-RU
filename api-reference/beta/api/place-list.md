---
title: Список мест
description: Получение списка объектов Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 173273bac942e8c2b2084109a1a50af3da579a53
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841054"
---
# <a name="list-places"></a><span data-ttu-id="d567a-103">Список мест</span><span class="sxs-lookup"><span data-stu-id="d567a-103">List places</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d567a-104">Получение коллекции указанного типа объектов [Place](../resources/place.md) , определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d567a-104">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="d567a-105">Например, вы можете получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d567a-105">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="d567a-106">Объект **Place** может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="d567a-106">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="d567a-107">[Комната](../resources/room.md) , включающая в себя обширные свойства, такие как адрес электронной почты для комнаты, Специальные возможности, мощность и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="d567a-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="d567a-108">[Список помещений](../resources/roomlist.md) , включающий адрес электронной почты для списка помещений, и свойство навигации для получения коллекции экземпляров комнаты в списке помещений.</span><span class="sxs-lookup"><span data-stu-id="d567a-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="d567a-109">**Комната** и **RoomList принимают одиночные** являются производными от объекта **Place** .</span><span class="sxs-lookup"><span data-stu-id="d567a-109">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="d567a-110">В сравнении с функциями [финдрумс](../api/user-findrooms.md) и [финдрумлистс](../api/user-findroomlists.md) эта операция возвращает расширенные полезные данные для комнат и списков помещений.</span><span class="sxs-lookup"><span data-stu-id="d567a-110">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="d567a-111">Подробнее [](../resources/place.md#using-the-places-api) о том, как они сравниваются.</span><span class="sxs-lookup"><span data-stu-id="d567a-111">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="d567a-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d567a-112">Permissions</span></span>

<span data-ttu-id="d567a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d567a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d567a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d567a-115">Permission type</span></span>                        | <span data-ttu-id="d567a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d567a-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d567a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d567a-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d567a-118">Размещение. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d567a-118">Place.Read.All</span></span> |
| <span data-ttu-id="d567a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d567a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d567a-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d567a-120">Not supported</span></span> |
| <span data-ttu-id="d567a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d567a-121">Application</span></span>                            | <span data-ttu-id="d567a-122">Размещение. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d567a-122">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d567a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d567a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d567a-124">Чтобы получить все комнаты в клиенте, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="d567a-124">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="d567a-125">Получение всех списков помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="d567a-125">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="d567a-126">Чтобы получить все комнаты в указанном списке помещений, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="d567a-126">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="d567a-127">**Note**: для получения комнат в списке помещений необходимо указать список помещений по свойству **EmailAddress** , а не по **идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="d567a-127">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="d567a-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d567a-128">Optional query parameters</span></span>

<span data-ttu-id="d567a-129">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d567a-129">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d567a-130">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d567a-130">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d567a-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d567a-131">Request headers</span></span>

| <span data-ttu-id="d567a-132">Имя</span><span class="sxs-lookup"><span data-stu-id="d567a-132">Name</span></span>          | <span data-ttu-id="d567a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d567a-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d567a-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d567a-134">Authorization</span></span> | <span data-ttu-id="d567a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d567a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d567a-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d567a-137">Request body</span></span>

<span data-ttu-id="d567a-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d567a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d567a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d567a-139">Response</span></span>

<span data-ttu-id="d567a-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d567a-140">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d567a-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="d567a-141">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="d567a-142">Пример 1: список всех комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="d567a-142">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d567a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d567a-143">Request</span></span>

<span data-ttu-id="d567a-144">В приведенном ниже примере показано, как получить все объекты [комнаты](../resources/room.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d567a-144">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```

#### <a name="response"></a><span data-ttu-id="d567a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d567a-145">Response</span></span>

<span data-ttu-id="d567a-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d567a-146">The following is an example of the response.</span></span>

><span data-ttu-id="d567a-147">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d567a-147">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d567a-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d567a-148">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.room",
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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="d567a-149">Пример 2: список всех списков помещений, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="d567a-149">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="d567a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="d567a-150">Request</span></span>

<span data-ttu-id="d567a-151">В приведенном ниже примере показано, как получить все объекты [RoomList принимают одиночные](../resources/roomlist.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d567a-151">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```http
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```

#### <a name="response"></a><span data-ttu-id="d567a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d567a-152">Response</span></span>

<span data-ttu-id="d567a-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d567a-153">The following is an example of the response.</span></span>

><span data-ttu-id="d567a-154">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d567a-154">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d567a-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d567a-155">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.roomList",
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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="d567a-156">Пример 3: список комнат, включенных в список помещений</span><span class="sxs-lookup"><span data-stu-id="d567a-156">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="d567a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d567a-157">Request</span></span>

<span data-ttu-id="d567a-158">В приведенном ниже примере показано, как получить список объектов [комнаты](../resources/room.md) , содержащийся в элементе **RoomList принимают одиночные**.</span><span class="sxs-lookup"><span data-stu-id="d567a-158">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```

#### <a name="response"></a><span data-ttu-id="d567a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d567a-159">Response</span></span>

<span data-ttu-id="d567a-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d567a-160">The following is an example of the response.</span></span>

><span data-ttu-id="d567a-161">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d567a-161">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d567a-162">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d567a-162">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
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
