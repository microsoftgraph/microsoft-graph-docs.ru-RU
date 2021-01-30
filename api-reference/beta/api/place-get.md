---
title: Получить место
description: Извлечение свойств и связей объекта place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 71e876bbce1fc185aa866624867995584767e3df
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059695"
---
# <a name="get-place"></a><span data-ttu-id="e775b-103">Получить место</span><span class="sxs-lookup"><span data-stu-id="e775b-103">Get place</span></span>

<span data-ttu-id="e775b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e775b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="e775b-105">Получите свойства и связи объекта [place,](../resources/place.md) указанного по его ИД или адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e775b-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="e775b-106">Объект **place** может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="e775b-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="e775b-107">[Комната,](../resources/room.md) которая включает в себя богатые свойства, такие как адрес электронной почты для комнаты, а также доступность, емкость и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="e775b-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="e775b-108">Список [помещений,](../resources/roomlist.md) который включает адрес электронной почты для списка помещений и свойство навигации для получения коллекции экземпляров помещений в этом списке помещений. </span><span class="sxs-lookup"><span data-stu-id="e775b-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="e775b-109">И **room,** и **roomList** являются производными от [объекта place.](../resources/place.md)</span><span class="sxs-lookup"><span data-stu-id="e775b-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e775b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e775b-110">Permissions</span></span>

<span data-ttu-id="e775b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e775b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e775b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e775b-113">Permission type</span></span>                        | <span data-ttu-id="e775b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e775b-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e775b-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e775b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e775b-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="e775b-116">Place.Read.All</span></span> |
| <span data-ttu-id="e775b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e775b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e775b-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e775b-118">Not supported</span></span> |
| <span data-ttu-id="e775b-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="e775b-119">Application</span></span>                            | <span data-ttu-id="e775b-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="e775b-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e775b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e775b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e775b-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e775b-122">Optional query parameters</span></span>
<span data-ttu-id="e775b-123">Используйте $select для получения свойств **определенного** места.</span><span class="sxs-lookup"><span data-stu-id="e775b-123">Use $select to get specific **place** properties.</span></span>

<span data-ttu-id="e775b-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e775b-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e775b-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e775b-125">Request headers</span></span>

| <span data-ttu-id="e775b-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e775b-126">Name</span></span>          | <span data-ttu-id="e775b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e775b-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e775b-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e775b-128">Authorization</span></span> | <span data-ttu-id="e775b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e775b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e775b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e775b-131">Request body</span></span>

<span data-ttu-id="e775b-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e775b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e775b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e775b-133">Response</span></span>

<span data-ttu-id="e775b-134">В случае успеха этот метод возвращает код отклика и объект запрашиваемого места `200 OK` в тексте [](../resources/place.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="e775b-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e775b-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="e775b-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="e775b-136">Пример 1. Получить комнату</span><span class="sxs-lookup"><span data-stu-id="e775b-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="e775b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e775b-137">Request</span></span>

<span data-ttu-id="e775b-138">В следующем примере **указывается ид** комнаты **для** получения ее свойств.</span><span class="sxs-lookup"><span data-stu-id="e775b-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="e775b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e775b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="e775b-140">C#</span><span class="sxs-lookup"><span data-stu-id="e775b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e775b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e775b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e775b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e775b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e775b-143">Java</span><span class="sxs-lookup"><span data-stu-id="e775b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e775b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e775b-144">Response</span></span>

<span data-ttu-id="e775b-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e775b-145">The following is an example of the response.</span></span>

><span data-ttu-id="e775b-146">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e775b-146">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e775b-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e775b-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="e775b-148">Пример 2. Получить список помещений</span><span class="sxs-lookup"><span data-stu-id="e775b-148">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="e775b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e775b-149">Request</span></span>

<span data-ttu-id="e775b-150">В следующем примере **указывается адрес emailAddress** объекта **roomList для** получения его свойств.</span><span class="sxs-lookup"><span data-stu-id="e775b-150">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="e775b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e775b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="e775b-152">C#</span><span class="sxs-lookup"><span data-stu-id="e775b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e775b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e775b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e775b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e775b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e775b-155">Java</span><span class="sxs-lookup"><span data-stu-id="e775b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e775b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e775b-156">Response</span></span>

<span data-ttu-id="e775b-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e775b-157">The following is an example of the response.</span></span>

><span data-ttu-id="e775b-158">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e775b-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e775b-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e775b-159">All the properties will be returned from an actual call.</span></span>

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


