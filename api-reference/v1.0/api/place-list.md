---
title: Места списка
description: Извлечение списка объектов места.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c6c128b9aca8f8ef455a70f92f43b27c8d325525
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053981"
---
# <a name="list-places"></a><span data-ttu-id="c708f-103">Места списка</span><span class="sxs-lookup"><span data-stu-id="c708f-103">List places</span></span>

<span data-ttu-id="c708f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c708f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="c708f-105">Получите коллекцию указанных типов объектов [места,](../resources/place.md) определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c708f-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="c708f-106">Например, вы можете получить все комнаты, все списки комнат или комнаты в определенном списке комнат в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c708f-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="c708f-107">Объект **place** может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="c708f-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="c708f-108">Комната [с](../resources/room.md) богатыми свойствами, такими как адрес электронной почты для комнаты, доступностью, емкостью и поддержкой устройств.</span><span class="sxs-lookup"><span data-stu-id="c708f-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="c708f-109">Список [номеров,](../resources/roomlist.md) который включает адрес электронной почты для списка номеров, и свойство навигации для получения коллекции экземпляров комнат в списке номеров.</span><span class="sxs-lookup"><span data-stu-id="c708f-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span>

<span data-ttu-id="c708f-110">Как **комнаты,** так **и roomList** являются производными от **объекта place.**</span><span class="sxs-lookup"><span data-stu-id="c708f-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="c708f-111">По умолчанию эта операция возвращает 100 мест на страницу.</span><span class="sxs-lookup"><span data-stu-id="c708f-111">By default, this operation returns 100 places per page.</span></span>

<span data-ttu-id="c708f-112">По сравнению с [функциями findRooms](/graph/api/user-findrooms?view=graph-rest-beta) и [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) эта операция возвращает более богатую нагрузку для комнат и списков номеров.</span><span class="sxs-lookup"><span data-stu-id="c708f-112">Compared with the [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) and [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="c708f-113">Сведения [о том,](../resources/place.md#using-the-places-api) как они сравнивают.</span><span class="sxs-lookup"><span data-stu-id="c708f-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="c708f-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c708f-114">Permissions</span></span>

<span data-ttu-id="c708f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c708f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c708f-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c708f-117">Permission type</span></span>                        | <span data-ttu-id="c708f-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c708f-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c708f-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c708f-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="c708f-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="c708f-120">Place.Read.All</span></span> |
| <span data-ttu-id="c708f-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c708f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c708f-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c708f-122">Not supported</span></span> |
| <span data-ttu-id="c708f-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="c708f-123">Application</span></span>                            | <span data-ttu-id="c708f-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="c708f-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c708f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="c708f-126">Чтобы получить все комнаты в клиенте:</span><span class="sxs-lookup"><span data-stu-id="c708f-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="c708f-127">Чтобы получить все списки комнат в клиенте:</span><span class="sxs-lookup"><span data-stu-id="c708f-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="c708f-128">Чтобы получить все комнаты в указанном списке номеров:</span><span class="sxs-lookup"><span data-stu-id="c708f-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="c708f-129">**Примечание.** Чтобы получить номера в списке номеров, необходимо указать список номеров по свойству **emailAddress,** а не **по его id.**</span><span class="sxs-lookup"><span data-stu-id="c708f-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c708f-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c708f-130">Optional query parameters</span></span>
<span data-ttu-id="c708f-131">Этот метод поддерживает следующие параметры запроса, чтобы помочь настроить ответ:</span><span class="sxs-lookup"><span data-stu-id="c708f-131">This method supports the following query parameters to help customize the response:</span></span>
- `$filter`
- `$select`
- `$top`
- `$skip`
- `$count=true`

<span data-ttu-id="c708f-132">Используйте `$top` для настройки размера страницы.</span><span class="sxs-lookup"><span data-stu-id="c708f-132">Use `$top` to customize the page size.</span></span> <span data-ttu-id="c708f-133">Размер страницы по умолчанию — 100.</span><span class="sxs-lookup"><span data-stu-id="c708f-133">The default page size is 100.</span></span>

<span data-ttu-id="c708f-134">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c708f-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c708f-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c708f-135">Request headers</span></span>

| <span data-ttu-id="c708f-136">Имя</span><span class="sxs-lookup"><span data-stu-id="c708f-136">Name</span></span>          | <span data-ttu-id="c708f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c708f-137">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c708f-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c708f-138">Authorization</span></span> | <span data-ttu-id="c708f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c708f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c708f-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c708f-141">Request body</span></span>

<span data-ttu-id="c708f-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c708f-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c708f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-143">Response</span></span>

<span data-ttu-id="c708f-144">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов-мест `200 OK` в тексте [](../resources/place.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="c708f-144">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c708f-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="c708f-145">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="c708f-146">Пример 1. Список всех комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="c708f-146">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="c708f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-147">Request</span></span>

<span data-ttu-id="c708f-148">В следующем примере показано, как получить все объекты [комнаты](../resources/room.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c708f-148">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>



# <a name="http"></a>[<span data-ttu-id="c708f-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c708f-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="c708f-150">C#</span><span class="sxs-lookup"><span data-stu-id="c708f-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c708f-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c708f-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c708f-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c708f-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c708f-153">Java</span><span class="sxs-lookup"><span data-stu-id="c708f-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c708f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-154">Response</span></span>

<span data-ttu-id="c708f-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c708f-155">The following is an example of the response.</span></span>

><span data-ttu-id="c708f-156">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c708f-156">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="c708f-157">Пример 2. Список всех списков комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="c708f-157">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="c708f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-158">Request</span></span>

<span data-ttu-id="c708f-159">В следующем примере показано, как получить все объекты [roomList](../resources/roomlist.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c708f-159">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="c708f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c708f-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="c708f-161">C#</span><span class="sxs-lookup"><span data-stu-id="c708f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c708f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c708f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c708f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c708f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c708f-164">Java</span><span class="sxs-lookup"><span data-stu-id="c708f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c708f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-165">Response</span></span>

<span data-ttu-id="c708f-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c708f-166">The following is an example of the response.</span></span>

><span data-ttu-id="c708f-167">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c708f-167">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="c708f-168">Пример 3. Списки комнат, содержащихся в списке номеров</span><span class="sxs-lookup"><span data-stu-id="c708f-168">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="c708f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-169">Request</span></span>

<span data-ttu-id="c708f-170">В следующем примере показано, как получить список объектов [комнат,](../resources/room.md) содержащихся в **списке roomList.**</span><span class="sxs-lookup"><span data-stu-id="c708f-170">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span>


# <a name="http"></a>[<span data-ttu-id="c708f-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="c708f-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="c708f-172">C#</span><span class="sxs-lookup"><span data-stu-id="c708f-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c708f-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c708f-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c708f-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c708f-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c708f-175">Java</span><span class="sxs-lookup"><span data-stu-id="c708f-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c708f-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-176">Response</span></span>

<span data-ttu-id="c708f-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c708f-177">The following is an example of the response.</span></span>

><span data-ttu-id="c708f-178">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c708f-178">**Note**: The response object shown here might be shortened for readability.</span></span>

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
  ]
}-->
