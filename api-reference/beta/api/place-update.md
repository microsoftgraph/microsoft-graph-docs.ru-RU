---
title: Место обновления
description: Обновление свойств объекта place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 802e29cfbaab46d3d3b8a1f7d2bbe0ad1ca031b4
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059730"
---
# <a name="update-place"></a><span data-ttu-id="51e3f-103">Место обновления</span><span class="sxs-lookup"><span data-stu-id="51e3f-103">Update place</span></span>

<span data-ttu-id="51e3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51e3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e3f-105">Обновление свойств объекта [place,](../resources/place.md) который может быть [помещением](../resources/room.md) или [списком помещений.](../resources/roomlist.md)</span><span class="sxs-lookup"><span data-stu-id="51e3f-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="51e3f-106">Вы можете определить помещение **или** **список помещений,** указав **свойство id** или **emailAddress.**</span><span class="sxs-lookup"><span data-stu-id="51e3f-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="51e3f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51e3f-107">Permissions</span></span>

<span data-ttu-id="51e3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51e3f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e3f-110">Permission type</span></span>                        | <span data-ttu-id="51e3f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e3f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51e3f-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e3f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="51e3f-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e3f-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="51e3f-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e3f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e3f-115">Not supported.</span></span> |
| <span data-ttu-id="51e3f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51e3f-116">Application</span></span>                            | <span data-ttu-id="51e3f-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="51e3f-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="51e3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e3f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="51e3f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51e3f-119">Request headers</span></span>

| <span data-ttu-id="51e3f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="51e3f-120">Name</span></span>       | <span data-ttu-id="51e3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51e3f-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="51e3f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51e3f-122">Authorization</span></span>  | <span data-ttu-id="51e3f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51e3f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51e3f-125">Content-Type</span></span> | <span data-ttu-id="51e3f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e3f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51e3f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51e3f-128">Request body</span></span>

<span data-ttu-id="51e3f-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="51e3f-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="51e3f-130">Одновременно можно обновить только один экземпляр ресурса place **(room** или **roomList).**</span><span class="sxs-lookup"><span data-stu-id="51e3f-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="51e3f-131">В теле запроса укажите тип места и включив свойства этого типа для `@odata.type` обновления.</span><span class="sxs-lookup"><span data-stu-id="51e3f-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="51e3f-132">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="51e3f-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="51e3f-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="51e3f-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="51e3f-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e3f-134">Property</span></span>               | <span data-ttu-id="51e3f-135">Тип</span><span class="sxs-lookup"><span data-stu-id="51e3f-135">Type</span></span>                                              | <span data-ttu-id="51e3f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="51e3f-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="51e3f-137">address</span><span class="sxs-lookup"><span data-stu-id="51e3f-137">address</span></span>                | [<span data-ttu-id="51e3f-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="51e3f-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="51e3f-139">Адрес помещения или списка помещений.</span><span class="sxs-lookup"><span data-stu-id="51e3f-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="51e3f-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="51e3f-140">audioDeviceName</span></span>        | <span data-ttu-id="51e3f-141">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-141">String</span></span>                                            | <span data-ttu-id="51e3f-142">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="51e3f-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="51e3f-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="51e3f-143">bookingType</span></span>            | [<span data-ttu-id="51e3f-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="51e3f-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="51e3f-145">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="51e3f-145">Type of room.</span></span> <span data-ttu-id="51e3f-146">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="51e3f-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="51e3f-147">building</span><span class="sxs-lookup"><span data-stu-id="51e3f-147">building</span></span>               | <span data-ttu-id="51e3f-148">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-148">String</span></span>                                            | <span data-ttu-id="51e3f-149">Указывает название здания или номер здания, в который находится помещение.</span><span class="sxs-lookup"><span data-stu-id="51e3f-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="51e3f-150">capacity</span><span class="sxs-lookup"><span data-stu-id="51e3f-150">capacity</span></span>               | <span data-ttu-id="51e3f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="51e3f-151">Int32</span></span>                                             | <span data-ttu-id="51e3f-152">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="51e3f-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="51e3f-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="51e3f-153">displayDeviceName</span></span>      | <span data-ttu-id="51e3f-154">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-154">String</span></span>                                            | <span data-ttu-id="51e3f-155">Указывает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="51e3f-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="51e3f-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="51e3f-156">floorLabel</span></span>             | <span data-ttu-id="51e3f-157">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-157">String</span></span>                                            | <span data-ttu-id="51e3f-158">Указывает букву этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="51e3f-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="51e3f-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="51e3f-159">floorNumber</span></span>            | <span data-ttu-id="51e3f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="51e3f-160">Int32</span></span>                                             | <span data-ttu-id="51e3f-161">Указывает номер этажа, на который находится комната.</span><span class="sxs-lookup"><span data-stu-id="51e3f-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="51e3f-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="51e3f-162">geoCoordinates</span></span>         | [<span data-ttu-id="51e3f-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="51e3f-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="51e3f-164">Указывает расположение помещения или списка помещений в широте, долготе и при желании координат высоты.</span><span class="sxs-lookup"><span data-stu-id="51e3f-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="51e3f-165">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="51e3f-165">isWheelChairAccessible</span></span> | <span data-ttu-id="51e3f-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="51e3f-166">Boolean</span></span>                                           | <span data-ttu-id="51e3f-167">Указывает, доступна ли комната.</span><span class="sxs-lookup"><span data-stu-id="51e3f-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="51e3f-168">label</span><span class="sxs-lookup"><span data-stu-id="51e3f-168">label</span></span>                  | <span data-ttu-id="51e3f-169">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-169">String</span></span>                                            | <span data-ttu-id="51e3f-170">Указывает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="51e3f-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="51e3f-171">nickname</span><span class="sxs-lookup"><span data-stu-id="51e3f-171">nickname</span></span>               | <span data-ttu-id="51e3f-172">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-172">String</span></span>                                            | <span data-ttu-id="51e3f-173">Указывает псевдоним для комнаты, например "conf room".</span><span class="sxs-lookup"><span data-stu-id="51e3f-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="51e3f-174">phone</span><span class="sxs-lookup"><span data-stu-id="51e3f-174">phone</span></span>                  | <span data-ttu-id="51e3f-175">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-175">String</span></span>                                            | <span data-ttu-id="51e3f-176">Номер телефона комнаты или списка помещений.</span><span class="sxs-lookup"><span data-stu-id="51e3f-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="51e3f-177">tags</span><span class="sxs-lookup"><span data-stu-id="51e3f-177">tags</span></span>                   | <span data-ttu-id="51e3f-178">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="51e3f-178">String collection</span></span>                                 | <span data-ttu-id="51e3f-179">Указывает дополнительные функции комнаты, например такие сведения, как тип представления или тип ветвя.</span><span class="sxs-lookup"><span data-stu-id="51e3f-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="51e3f-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="51e3f-180">videoDeviceName</span></span>        | <span data-ttu-id="51e3f-181">String</span><span class="sxs-lookup"><span data-stu-id="51e3f-181">String</span></span>                                            | <span data-ttu-id="51e3f-182">Указывает имя видео устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="51e3f-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="51e3f-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e3f-183">Response</span></span>

<span data-ttu-id="51e3f-184">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51e3f-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51e3f-185">Примеры</span><span class="sxs-lookup"><span data-stu-id="51e3f-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="51e3f-186">Пример 1. Обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="51e3f-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="51e3f-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e3f-187">Request</span></span>

<span data-ttu-id="51e3f-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e3f-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="51e3f-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="51e3f-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": 50,
  "isWheelChairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="51e3f-190">C#</span><span class="sxs-lookup"><span data-stu-id="51e3f-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51e3f-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51e3f-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51e3f-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51e3f-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51e3f-193">Java</span><span class="sxs-lookup"><span data-stu-id="51e3f-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51e3f-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e3f-194">Response</span></span>

<span data-ttu-id="51e3f-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51e3f-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="51e3f-196">Показанный здесь объект ответа может быть сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="51e3f-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51e3f-197">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51e3f-197">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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
      "latitude": 47.0,
      "longitude": -122.0
    },
    "phone": "555-555-0100",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": 50,
    "building": "1",
    "floorLabel": "1P",
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="51e3f-198">Пример 2. Обновление списка помещений</span><span class="sxs-lookup"><span data-stu-id="51e3f-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="51e3f-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e3f-199">Request</span></span>

<span data-ttu-id="51e3f-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e3f-200">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="51e3f-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="51e3f-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomList",
  "displayName": "Building 1",
  "phone":"555-555-0100",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 }
}
```
# <a name="c"></a>[<span data-ttu-id="51e3f-202">C#</span><span class="sxs-lookup"><span data-stu-id="51e3f-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51e3f-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51e3f-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51e3f-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51e3f-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51e3f-205">Java</span><span class="sxs-lookup"><span data-stu-id="51e3f-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51e3f-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e3f-206">Response</span></span>

<span data-ttu-id="51e3f-207">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51e3f-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="51e3f-208">Показанный здесь объект ответа может быть сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="51e3f-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51e3f-209">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51e3f-209">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 },
  "phone": "555-555-0100",
  "emailAddress": "bldg1@contoso.com"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


