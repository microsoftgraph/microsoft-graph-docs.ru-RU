---
title: Места списка
description: Получить список объектов мест.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9c640930e29be9ba8912c1c8572ed16b37c8333e
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059555"
---
# <a name="list-places"></a><span data-ttu-id="3ec0c-103">Места списка</span><span class="sxs-lookup"><span data-stu-id="3ec0c-103">List places</span></span>

<span data-ttu-id="3ec0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec0c-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="3ec0c-105">Получите коллекцию объектов указанного типа [мест,](../resources/place.md) определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="3ec0c-106">Например, можно получить все комнаты, все списки помещений или комнаты в определенном списке помещений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="3ec0c-107">Объект **place** может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="3ec0c-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="3ec0c-108">[Комната,](../resources/room.md) которая содержит богатые свойства, такие как адрес электронной почты для комнаты, а также доступность, емкость и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="3ec0c-109">Список [помещений,](../resources/roomlist.md) который включает адрес электронной почты для списка помещений и свойство навигации для получения коллекции экземпляров помещений в списке помещений.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span>

<span data-ttu-id="3ec0c-110">И **room,** и **roomList** являются производными от **объекта place.**</span><span class="sxs-lookup"><span data-stu-id="3ec0c-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="3ec0c-111">По умолчанию эта операция возвращает 100 мест на страницу.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-111">By default, this operation returns 100 places per page.</span></span>

<span data-ttu-id="3ec0c-112">По сравнению с [функциями findRooms](/graph/api/user-findrooms?view=graph-rest-beta) и [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) эта операция возвращает более емкие полезной нагрузки для помещений и списков помещений.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-112">Compared with the [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) and [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="3ec0c-113">См. [подробные](../resources/place.md#using-the-places-api) сведения о том, как они сравнивают.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec0c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec0c-114">Permissions</span></span>

<span data-ttu-id="3ec0c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ec0c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec0c-117">Permission type</span></span>                        | <span data-ttu-id="3ec0c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec0c-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ec0c-119">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec0c-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ec0c-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec0c-120">Place.Read.All</span></span> |
| <span data-ttu-id="3ec0c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec0c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec0c-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ec0c-122">Not supported</span></span> |
| <span data-ttu-id="3ec0c-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="3ec0c-123">Application</span></span>                            | <span data-ttu-id="3ec0c-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec0c-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec0c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec0c-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3ec0c-126">Чтобы получить все комнаты в клиенте:</span><span class="sxs-lookup"><span data-stu-id="3ec0c-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="3ec0c-127">Чтобы получить все списки помещений в клиенте:</span><span class="sxs-lookup"><span data-stu-id="3ec0c-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="3ec0c-128">Чтобы получить все комнаты в указанном списке помещений:</span><span class="sxs-lookup"><span data-stu-id="3ec0c-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="3ec0c-129">**Примечание.** Чтобы получить помещения в списке помещений, необходимо указать список помещений по его свойству **emailAddress,** а не **по его ид.**</span><span class="sxs-lookup"><span data-stu-id="3ec0c-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3ec0c-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ec0c-130">Optional query parameters</span></span>
<span data-ttu-id="3ec0c-131">Этот метод поддерживает следующие параметры запроса для настройки ответа:</span><span class="sxs-lookup"><span data-stu-id="3ec0c-131">This method supports the following query parameters to help customize the response:</span></span>
- `$filter`
- `$select`
- `$top`
- `$skip`
- `$count=true`

<span data-ttu-id="3ec0c-132">Используется `$top` для настройки размера страницы.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-132">Use `$top` to customize the page size.</span></span> <span data-ttu-id="3ec0c-133">Размер страницы по умолчанию — 100.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-133">The default page size is 100.</span></span>

<span data-ttu-id="3ec0c-134">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3ec0c-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ec0c-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ec0c-135">Request headers</span></span>

| <span data-ttu-id="3ec0c-136">Имя</span><span class="sxs-lookup"><span data-stu-id="3ec0c-136">Name</span></span>          | <span data-ttu-id="3ec0c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec0c-137">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3ec0c-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ec0c-138">Authorization</span></span> | <span data-ttu-id="3ec0c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec0c-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ec0c-141">Request body</span></span>

<span data-ttu-id="3ec0c-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec0c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec0c-143">Response</span></span>

<span data-ttu-id="3ec0c-144">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов-мест](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-144">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ec0c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ec0c-145">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="3ec0c-146">Пример 1. Список всех комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="3ec0c-146">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="3ec0c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec0c-147">Request</span></span>

<span data-ttu-id="3ec0c-148">В следующем примере показано, как получить все [объекты комнаты](../resources/room.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-148">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>



# <a name="http"></a>[<span data-ttu-id="3ec0c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec0c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="3ec0c-150">C#</span><span class="sxs-lookup"><span data-stu-id="3ec0c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec0c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec0c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec0c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec0c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec0c-153">Java</span><span class="sxs-lookup"><span data-stu-id="3ec0c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ec0c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec0c-154">Response</span></span>

<span data-ttu-id="3ec0c-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-155">The following is an example of the response.</span></span>

><span data-ttu-id="3ec0c-156">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-156">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ec0c-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-157">All the properties will be returned from an actual call.</span></span>

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
      "capacity": 50,
      "building": "1",
      "floorNumber": 1,
      "isManaged": true,
      "isWheelChairAccessible": false,
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
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="3ec0c-158">Пример 2. Список всех списков помещений, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="3ec0c-158">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="3ec0c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec0c-159">Request</span></span>

<span data-ttu-id="3ec0c-160">В следующем примере показано, как получить все [объекты roomList](../resources/roomlist.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-160">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ec0c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec0c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="3ec0c-162">C#</span><span class="sxs-lookup"><span data-stu-id="3ec0c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec0c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec0c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec0c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec0c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec0c-165">Java</span><span class="sxs-lookup"><span data-stu-id="3ec0c-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ec0c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec0c-166">Response</span></span>

<span data-ttu-id="3ec0c-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-167">The following is an example of the response.</span></span>

><span data-ttu-id="3ec0c-168">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-168">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ec0c-169">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-169">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="3ec0c-170">Пример 3. Список помещений, содержащихся в списке помещений</span><span class="sxs-lookup"><span data-stu-id="3ec0c-170">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="3ec0c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec0c-171">Request</span></span>

<span data-ttu-id="3ec0c-172">В следующем примере показано, как получить список объектов [помещения,](../resources/room.md) содержащихся в **списке помещений.**</span><span class="sxs-lookup"><span data-stu-id="3ec0c-172">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ec0c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec0c-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="3ec0c-174">C#</span><span class="sxs-lookup"><span data-stu-id="3ec0c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec0c-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec0c-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec0c-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec0c-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec0c-177">Java</span><span class="sxs-lookup"><span data-stu-id="3ec0c-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ec0c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec0c-178">Response</span></span>

<span data-ttu-id="3ec0c-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-179">The following is an example of the response.</span></span>

><span data-ttu-id="3ec0c-180">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-180">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ec0c-181">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ec0c-181">All the properties will be returned from an actual call.</span></span>

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
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
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
