---
title: Места списка
description: Извлечение списка объектов места.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 019198d0173155c673e12a266bcf41922e040f81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055395"
---
# <a name="list-places"></a><span data-ttu-id="1df98-103">Места списка</span><span class="sxs-lookup"><span data-stu-id="1df98-103">List places</span></span>

<span data-ttu-id="1df98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df98-105">Получите коллекцию указанных типов объектов [места,](../resources/place.md) определенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1df98-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="1df98-106">Например, вы можете получить все комнаты, все списки комнат или комнаты в определенном списке комнат в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1df98-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="1df98-107">Объект **place** может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="1df98-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="1df98-108">Комната [с](../resources/room.md) богатыми свойствами, такими как адрес электронной почты для комнаты, доступностью, емкостью и поддержкой устройств.</span><span class="sxs-lookup"><span data-stu-id="1df98-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="1df98-109">Список [номеров,](../resources/roomlist.md) который включает адрес электронной почты для списка номеров, и свойство навигации для получения коллекции экземпляров комнат в списке номеров.</span><span class="sxs-lookup"><span data-stu-id="1df98-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="1df98-110">Как **комнаты,** так **и roomList** являются производными от **объекта place.**</span><span class="sxs-lookup"><span data-stu-id="1df98-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="1df98-111">По умолчанию эта операция возвращает 100 мест на страницу.</span><span class="sxs-lookup"><span data-stu-id="1df98-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="1df98-112">По сравнению с [функциями findRooms](../api/user-findrooms.md) и [findRoomLists](../api/user-findroomlists.md) эта операция возвращает более богатую нагрузку для комнат и списков номеров.</span><span class="sxs-lookup"><span data-stu-id="1df98-112">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="1df98-113">Сведения [о том,](../resources/place.md#using-the-places-api) как они сравнивают.</span><span class="sxs-lookup"><span data-stu-id="1df98-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="1df98-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1df98-114">Permissions</span></span>

<span data-ttu-id="1df98-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1df98-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1df98-117">Permission type</span></span>                        | <span data-ttu-id="1df98-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1df98-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1df98-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1df98-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="1df98-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="1df98-120">Place.Read.All</span></span> |
| <span data-ttu-id="1df98-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1df98-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1df98-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1df98-122">Not supported</span></span> |
| <span data-ttu-id="1df98-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="1df98-123">Application</span></span>                            | <span data-ttu-id="1df98-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="1df98-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1df98-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1df98-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="1df98-126">Чтобы получить все комнаты в клиенте:</span><span class="sxs-lookup"><span data-stu-id="1df98-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="1df98-127">Чтобы получить все списки комнат в клиенте:</span><span class="sxs-lookup"><span data-stu-id="1df98-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="1df98-128">Чтобы получить все комнаты в указанном списке номеров:</span><span class="sxs-lookup"><span data-stu-id="1df98-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="1df98-129">**Примечание.** Чтобы получить номера в списке номеров, необходимо указать список номеров по свойству **emailAddress,** а не **по его id.**</span><span class="sxs-lookup"><span data-stu-id="1df98-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="1df98-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1df98-130">Optional query parameters</span></span>
<span data-ttu-id="1df98-131">Этот метод поддерживает следующие параметры запроса, чтобы помочь настроить ответ:</span><span class="sxs-lookup"><span data-stu-id="1df98-131">This method supports the following query parameters to help customize the response:</span></span>
- <span data-ttu-id="1df98-132">$filter</span><span class="sxs-lookup"><span data-stu-id="1df98-132">$filter</span></span>
- <span data-ttu-id="1df98-133">$select</span><span class="sxs-lookup"><span data-stu-id="1df98-133">$select</span></span>
- <span data-ttu-id="1df98-134">$top</span><span class="sxs-lookup"><span data-stu-id="1df98-134">$top</span></span>
- <span data-ttu-id="1df98-135">$skip</span><span class="sxs-lookup"><span data-stu-id="1df98-135">$skip</span></span>
- <span data-ttu-id="1df98-136">$count=true</span><span class="sxs-lookup"><span data-stu-id="1df98-136">$count=true</span></span>

<span data-ttu-id="1df98-137">Используйте $top для настройки размера страницы.</span><span class="sxs-lookup"><span data-stu-id="1df98-137">Use $top to customize the page size.</span></span> <span data-ttu-id="1df98-138">Размер страницы по умолчанию — 100.</span><span class="sxs-lookup"><span data-stu-id="1df98-138">The default page size is 100.</span></span>

<span data-ttu-id="1df98-139">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1df98-139">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1df98-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1df98-140">Request headers</span></span>

| <span data-ttu-id="1df98-141">Имя</span><span class="sxs-lookup"><span data-stu-id="1df98-141">Name</span></span>          | <span data-ttu-id="1df98-142">Описание</span><span class="sxs-lookup"><span data-stu-id="1df98-142">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1df98-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1df98-143">Authorization</span></span> | <span data-ttu-id="1df98-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1df98-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1df98-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1df98-146">Request body</span></span>

<span data-ttu-id="1df98-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1df98-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1df98-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df98-148">Response</span></span>

<span data-ttu-id="1df98-149">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов-мест `200 OK` в тексте [](../resources/place.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="1df98-149">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1df98-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="1df98-150">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="1df98-151">Пример 1. Список всех комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="1df98-151">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1df98-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df98-152">Request</span></span>

<span data-ttu-id="1df98-153">В следующем примере показано, как получить все объекты [комнаты](../resources/room.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1df98-153">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="1df98-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df98-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="1df98-155">C#</span><span class="sxs-lookup"><span data-stu-id="1df98-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df98-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df98-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df98-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df98-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df98-158">Java</span><span class="sxs-lookup"><span data-stu-id="1df98-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1df98-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df98-159">Response</span></span>

<span data-ttu-id="1df98-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1df98-160">The following is an example of the response.</span></span>

><span data-ttu-id="1df98-161">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1df98-161">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="1df98-162">Пример 2. Список всех списков комнат, определенных в клиенте</span><span class="sxs-lookup"><span data-stu-id="1df98-162">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="1df98-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df98-163">Request</span></span>

<span data-ttu-id="1df98-164">В следующем примере показано, как получить все объекты [roomList](../resources/roomlist.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1df98-164">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="1df98-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df98-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="1df98-166">C#</span><span class="sxs-lookup"><span data-stu-id="1df98-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df98-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df98-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df98-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df98-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df98-169">Java</span><span class="sxs-lookup"><span data-stu-id="1df98-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1df98-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df98-170">Response</span></span>

<span data-ttu-id="1df98-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1df98-171">The following is an example of the response.</span></span>

><span data-ttu-id="1df98-172">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1df98-172">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="1df98-173">Пример 3. Списки комнат, содержащихся в списке номеров</span><span class="sxs-lookup"><span data-stu-id="1df98-173">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="1df98-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df98-174">Request</span></span>

<span data-ttu-id="1df98-175">В следующем примере показано, как получить список объектов [комнат,](../resources/room.md) содержащихся в **списке roomList.**</span><span class="sxs-lookup"><span data-stu-id="1df98-175">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="1df98-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="1df98-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="1df98-177">C#</span><span class="sxs-lookup"><span data-stu-id="1df98-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1df98-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1df98-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1df98-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1df98-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1df98-180">Java</span><span class="sxs-lookup"><span data-stu-id="1df98-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1df98-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df98-181">Response</span></span>

<span data-ttu-id="1df98-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1df98-182">The following is an example of the response.</span></span>

><span data-ttu-id="1df98-183">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1df98-183">**Note**: The response object shown here might be shortened for readability.</span></span>

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


