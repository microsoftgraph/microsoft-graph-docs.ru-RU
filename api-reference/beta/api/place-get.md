---
title: Получить место
description: Извлечение свойств и связей объекта place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2a5c259d05b88a6195a76420e573d6bbff155065
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055402"
---
# <a name="get-place"></a><span data-ttu-id="04a3f-103">Получить место</span><span class="sxs-lookup"><span data-stu-id="04a3f-103">Get place</span></span>

<span data-ttu-id="04a3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04a3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="04a3f-105">Получите свойства и связи [объекта-места,](../resources/place.md) указанные его ID или адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="04a3f-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="04a3f-106">Объект **place** может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="04a3f-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="04a3f-107">Комната [с](../resources/room.md) богатыми свойствами, такими как адрес электронной почты для комнаты, доступностью, емкостью и поддержкой устройств.</span><span class="sxs-lookup"><span data-stu-id="04a3f-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="04a3f-108">Список [номеров,](../resources/roomlist.md) который включает адрес электронной почты для списка номеров, и свойство навигации для получения коллекции экземпляров комнат в этом списке комнат. </span><span class="sxs-lookup"><span data-stu-id="04a3f-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="04a3f-109">Как **комнаты,** так **и roomList** являются производными от [объекта place.](../resources/place.md)</span><span class="sxs-lookup"><span data-stu-id="04a3f-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="04a3f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04a3f-110">Permissions</span></span>

<span data-ttu-id="04a3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04a3f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04a3f-113">Permission type</span></span>                        | <span data-ttu-id="04a3f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04a3f-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04a3f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04a3f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="04a3f-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="04a3f-116">Place.Read.All</span></span> |
| <span data-ttu-id="04a3f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04a3f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04a3f-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04a3f-118">Not supported</span></span> |
| <span data-ttu-id="04a3f-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="04a3f-119">Application</span></span>                            | <span data-ttu-id="04a3f-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="04a3f-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04a3f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04a3f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04a3f-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04a3f-122">Optional query parameters</span></span>
<span data-ttu-id="04a3f-123">Используйте $select для получения **определенных свойств** места.</span><span class="sxs-lookup"><span data-stu-id="04a3f-123">Use $select to get specific **place** properties.</span></span>

<span data-ttu-id="04a3f-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="04a3f-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="04a3f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04a3f-125">Request headers</span></span>

| <span data-ttu-id="04a3f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="04a3f-126">Name</span></span>          | <span data-ttu-id="04a3f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="04a3f-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="04a3f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04a3f-128">Authorization</span></span> | <span data-ttu-id="04a3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04a3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04a3f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04a3f-131">Request body</span></span>

<span data-ttu-id="04a3f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04a3f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04a3f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a3f-133">Response</span></span>

<span data-ttu-id="04a3f-134">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [места](../resources/place.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="04a3f-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04a3f-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="04a3f-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="04a3f-136">Пример 1. Получить комнату</span><span class="sxs-lookup"><span data-stu-id="04a3f-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="04a3f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="04a3f-137">Request</span></span>

<span data-ttu-id="04a3f-138">В следующем примере **указывается id** **комнаты для** получения ее свойств.</span><span class="sxs-lookup"><span data-stu-id="04a3f-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="04a3f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="04a3f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="04a3f-140">C#</span><span class="sxs-lookup"><span data-stu-id="04a3f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04a3f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04a3f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04a3f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04a3f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04a3f-143">Java</span><span class="sxs-lookup"><span data-stu-id="04a3f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="04a3f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a3f-144">Response</span></span>

<span data-ttu-id="04a3f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04a3f-145">The following is an example of the response.</span></span>

><span data-ttu-id="04a3f-146">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04a3f-146">**Note**: The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
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
}
```

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="04a3f-147">Пример 2. Получить список номеров</span><span class="sxs-lookup"><span data-stu-id="04a3f-147">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="04a3f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="04a3f-148">Request</span></span>

<span data-ttu-id="04a3f-149">В следующем примере **указывается emailAddress** **списка roomList** для получения его свойств.</span><span class="sxs-lookup"><span data-stu-id="04a3f-149">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="04a3f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="04a3f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="04a3f-151">C#</span><span class="sxs-lookup"><span data-stu-id="04a3f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04a3f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04a3f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04a3f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04a3f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04a3f-154">Java</span><span class="sxs-lookup"><span data-stu-id="04a3f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="04a3f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a3f-155">Response</span></span>

<span data-ttu-id="04a3f-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04a3f-156">The following is an example of the response.</span></span>

><span data-ttu-id="04a3f-157">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04a3f-157">**Note**: The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
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


