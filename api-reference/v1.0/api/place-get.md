---
title: Получение
description: Получение свойств и связей объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fe5a3a26b22d8c2497011c84d49d87e869964a0f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978876"
---
# <a name="get-place"></a><span data-ttu-id="366c4-103">Получение</span><span class="sxs-lookup"><span data-stu-id="366c4-103">Get place</span></span>

<span data-ttu-id="366c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="366c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="366c4-105">Получение свойств и связей объекта [Place](../resources/place.md) , указанных с помощью его идентификатора или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="366c4-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span>

<span data-ttu-id="366c4-106">Объект **Place** может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="366c4-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="366c4-107">[Комната](../resources/room.md) , включающая в себя обширные свойства, такие как адрес электронной почты для комнаты, Специальные возможности, мощность и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="366c4-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="366c4-108">[Список помещений](../resources/roomlist.md) , включающий адрес электронной почты для списка помещений, и свойство навигации для получения коллекции экземпляров **комнаты** в этом списке.</span><span class="sxs-lookup"><span data-stu-id="366c4-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="366c4-109">**Комната** и **RoomList принимают одиночные** являются производными от объекта [Place](../resources/place.md) .</span><span class="sxs-lookup"><span data-stu-id="366c4-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="366c4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="366c4-110">Permissions</span></span>

<span data-ttu-id="366c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="366c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="366c4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="366c4-113">Permission type</span></span>                        | <span data-ttu-id="366c4-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="366c4-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="366c4-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="366c4-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="366c4-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="366c4-116">Place.Read.All</span></span> |
| <span data-ttu-id="366c4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="366c4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="366c4-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="366c4-118">Not supported</span></span> |
| <span data-ttu-id="366c4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="366c4-119">Application</span></span>                            | <span data-ttu-id="366c4-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="366c4-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="366c4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="366c4-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="366c4-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="366c4-122">Optional query parameters</span></span>
<span data-ttu-id="366c4-123">Используется `$select` для получения свойств конкретного **места** .</span><span class="sxs-lookup"><span data-stu-id="366c4-123">Use `$select` to get specific **place** properties.</span></span>

<span data-ttu-id="366c4-124">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="366c4-124">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="366c4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="366c4-125">Request headers</span></span>

| <span data-ttu-id="366c4-126">Имя</span><span class="sxs-lookup"><span data-stu-id="366c4-126">Name</span></span>          | <span data-ttu-id="366c4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="366c4-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="366c4-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="366c4-128">Authorization</span></span> | <span data-ttu-id="366c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="366c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="366c4-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="366c4-131">Request body</span></span>

<span data-ttu-id="366c4-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="366c4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="366c4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="366c4-133">Response</span></span>

<span data-ttu-id="366c4-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="366c4-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="366c4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="366c4-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="366c4-136">Пример 1: получение комнаты</span><span class="sxs-lookup"><span data-stu-id="366c4-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="366c4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="366c4-137">Request</span></span>

<span data-ttu-id="366c4-138">В следующем примере задается **идентификатор** **комнаты** для получения ее свойств.</span><span class="sxs-lookup"><span data-stu-id="366c4-138">The following example specifies the **id** of a **room** to get its properties.</span></span>


# <a name="http"></a>[<span data-ttu-id="366c4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="366c4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="366c4-140">C#</span><span class="sxs-lookup"><span data-stu-id="366c4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="366c4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="366c4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="366c4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="366c4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="366c4-143">Java</span><span class="sxs-lookup"><span data-stu-id="366c4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="366c4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="366c4-144">Response</span></span>

<span data-ttu-id="366c4-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="366c4-145">The following is an example of the response.</span></span>

><span data-ttu-id="366c4-146">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="366c4-146">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="366c4-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="366c4-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_room",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
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
}
```

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="366c4-148">Пример 2: получение списка помещений</span><span class="sxs-lookup"><span data-stu-id="366c4-148">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="366c4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="366c4-149">Request</span></span>

<span data-ttu-id="366c4-150">В следующем примере задается значение **EmailAddress** объекта **RoomList принимают одиночные** для получения его свойств.</span><span class="sxs-lookup"><span data-stu-id="366c4-150">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>


# <a name="http"></a>[<span data-ttu-id="366c4-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="366c4-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="366c4-152">C#</span><span class="sxs-lookup"><span data-stu-id="366c4-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="366c4-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="366c4-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="366c4-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="366c4-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="366c4-155">Java</span><span class="sxs-lookup"><span data-stu-id="366c4-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="366c4-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="366c4-156">Response</span></span>

<span data-ttu-id="366c4-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="366c4-157">The following is an example of the response.</span></span>

><span data-ttu-id="366c4-158">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="366c4-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="366c4-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="366c4-159">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

