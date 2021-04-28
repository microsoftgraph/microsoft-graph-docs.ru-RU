---
title: Место обновления
description: Обновление свойств объекта place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 1b009f51fc095c5832ea7638f2ee4edd1ff21110
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053974"
---
# <a name="update-place"></a><span data-ttu-id="b2234-103">Место обновления</span><span class="sxs-lookup"><span data-stu-id="b2234-103">Update place</span></span>

<span data-ttu-id="b2234-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2234-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b2234-105">Обновление свойств объекта [place,](../resources/place.md) который может быть комнатой [или](../resources/room.md) [roomList.](../resources/roomlist.md)</span><span class="sxs-lookup"><span data-stu-id="b2234-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="b2234-106">Вы можете определить **номер или** **список номеров,** указав свойство **id** или **emailAddress.**</span><span class="sxs-lookup"><span data-stu-id="b2234-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2234-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2234-107">Permissions</span></span>

<span data-ttu-id="b2234-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2234-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2234-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2234-110">Permission type</span></span>                        | <span data-ttu-id="b2234-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2234-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2234-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2234-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2234-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2234-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="b2234-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2234-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2234-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2234-115">Not supported.</span></span> |
| <span data-ttu-id="b2234-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2234-116">Application</span></span>                            | <span data-ttu-id="b2234-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b2234-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2234-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2234-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="b2234-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2234-119">Request headers</span></span>

| <span data-ttu-id="b2234-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b2234-120">Name</span></span>       | <span data-ttu-id="b2234-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2234-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b2234-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2234-122">Authorization</span></span>  | <span data-ttu-id="b2234-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2234-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2234-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2234-125">Content-Type</span></span> | <span data-ttu-id="b2234-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2234-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2234-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2234-128">Request body</span></span>

<span data-ttu-id="b2234-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b2234-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b2234-130">Только один экземпляр ресурса места **(комната или** **roomList)** может обновляться одновременно.</span><span class="sxs-lookup"><span data-stu-id="b2234-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="b2234-131">В теле запроса используйте для указания типа места и включаем свойства этого типа `@odata.type` для обновления.</span><span class="sxs-lookup"><span data-stu-id="b2234-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="b2234-132">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="b2234-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b2234-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b2234-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b2234-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2234-134">Property</span></span>               | <span data-ttu-id="b2234-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b2234-135">Type</span></span>                                              | <span data-ttu-id="b2234-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b2234-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="b2234-137">address</span><span class="sxs-lookup"><span data-stu-id="b2234-137">address</span></span>                | [<span data-ttu-id="b2234-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b2234-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="b2234-139">Адрес улицы комнаты или списка номеров.</span><span class="sxs-lookup"><span data-stu-id="b2234-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="b2234-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2234-140">audioDeviceName</span></span>        | <span data-ttu-id="b2234-141">String</span><span class="sxs-lookup"><span data-stu-id="b2234-141">String</span></span>                                            | <span data-ttu-id="b2234-142">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="b2234-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="b2234-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="b2234-143">bookingType</span></span>            | [<span data-ttu-id="b2234-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="b2234-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="b2234-145">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="b2234-145">Type of room.</span></span> <span data-ttu-id="b2234-146">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="b2234-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="b2234-147">здание</span><span class="sxs-lookup"><span data-stu-id="b2234-147">building</span></span>               | <span data-ttu-id="b2234-148">String</span><span class="sxs-lookup"><span data-stu-id="b2234-148">String</span></span>                                            | <span data-ttu-id="b2234-149">Указывает имя здания или номер здания, в который находится комната.</span><span class="sxs-lookup"><span data-stu-id="b2234-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="b2234-150">емкость</span><span class="sxs-lookup"><span data-stu-id="b2234-150">capacity</span></span>               | <span data-ttu-id="b2234-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b2234-151">Int32</span></span>                                             | <span data-ttu-id="b2234-152">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="b2234-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="b2234-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2234-153">displayDeviceName</span></span>      | <span data-ttu-id="b2234-154">String</span><span class="sxs-lookup"><span data-stu-id="b2234-154">String</span></span>                                            | <span data-ttu-id="b2234-155">Указывает имя отображаемого устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="b2234-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="b2234-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="b2234-156">floorLabel</span></span>             | <span data-ttu-id="b2234-157">String</span><span class="sxs-lookup"><span data-stu-id="b2234-157">String</span></span>                                            | <span data-ttu-id="b2234-158">Указывает напольное письмо, в котором находится номер.</span><span class="sxs-lookup"><span data-stu-id="b2234-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="b2234-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="b2234-159">floorNumber</span></span>            | <span data-ttu-id="b2234-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b2234-160">Int32</span></span>                                             | <span data-ttu-id="b2234-161">Указывает номер пола, на который находится номер.</span><span class="sxs-lookup"><span data-stu-id="b2234-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="b2234-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b2234-162">geoCoordinates</span></span>         | [<span data-ttu-id="b2234-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b2234-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="b2234-164">Указывает расположение комнаты или списка номеров в широте, долготе и необязательных координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="b2234-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="b2234-165">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="b2234-165">isWheelChairAccessible</span></span> | <span data-ttu-id="b2234-166">Логический</span><span class="sxs-lookup"><span data-stu-id="b2234-166">Boolean</span></span>                                           | <span data-ttu-id="b2234-167">Указывает, доступна ли комната для инвалидных колясок.</span><span class="sxs-lookup"><span data-stu-id="b2234-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="b2234-168">label</span><span class="sxs-lookup"><span data-stu-id="b2234-168">label</span></span>                  | <span data-ttu-id="b2234-169">String</span><span class="sxs-lookup"><span data-stu-id="b2234-169">String</span></span>                                            | <span data-ttu-id="b2234-170">Указывает описательный метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="b2234-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="b2234-171">nickname</span><span class="sxs-lookup"><span data-stu-id="b2234-171">nickname</span></span>               | <span data-ttu-id="b2234-172">String</span><span class="sxs-lookup"><span data-stu-id="b2234-172">String</span></span>                                            | <span data-ttu-id="b2234-173">Указывает псевдоним для комнаты, например " conf room".</span><span class="sxs-lookup"><span data-stu-id="b2234-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="b2234-174">phone</span><span class="sxs-lookup"><span data-stu-id="b2234-174">phone</span></span>                  | <span data-ttu-id="b2234-175">String</span><span class="sxs-lookup"><span data-stu-id="b2234-175">String</span></span>                                            | <span data-ttu-id="b2234-176">Номер телефона комнаты или списка номеров.</span><span class="sxs-lookup"><span data-stu-id="b2234-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="b2234-177">tags</span><span class="sxs-lookup"><span data-stu-id="b2234-177">tags</span></span>                   | <span data-ttu-id="b2234-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b2234-178">String collection</span></span>                                 | <span data-ttu-id="b2234-179">Указывает дополнительные функции комнаты, например, такие сведения, как тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="b2234-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="b2234-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2234-180">videoDeviceName</span></span>        | <span data-ttu-id="b2234-181">String</span><span class="sxs-lookup"><span data-stu-id="b2234-181">String</span></span>                                            | <span data-ttu-id="b2234-182">Указывает имя видео устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="b2234-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="b2234-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2234-183">Response</span></span>

<span data-ttu-id="b2234-184">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [места](../resources/place.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2234-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2234-185">Примеры</span><span class="sxs-lookup"><span data-stu-id="b2234-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="b2234-186">Пример 1. Обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="b2234-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="b2234-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2234-187">Request</span></span>

<span data-ttu-id="b2234-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2234-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="b2234-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2234-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/cf100@contoso.com
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
# <a name="c"></a>[<span data-ttu-id="b2234-190">C#</span><span class="sxs-lookup"><span data-stu-id="b2234-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2234-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2234-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2234-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2234-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2234-193">Java</span><span class="sxs-lookup"><span data-stu-id="b2234-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2234-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2234-194">Response</span></span>

<span data-ttu-id="b2234-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b2234-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b2234-196">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2234-196">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="b2234-197">Пример 2. Обновление списка номеров</span><span class="sxs-lookup"><span data-stu-id="b2234-197">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="b2234-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2234-198">Request</span></span>

<span data-ttu-id="b2234-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2234-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2234-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2234-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
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
# <a name="c"></a>[<span data-ttu-id="b2234-201">C#</span><span class="sxs-lookup"><span data-stu-id="b2234-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2234-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2234-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2234-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2234-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2234-204">Java</span><span class="sxs-lookup"><span data-stu-id="b2234-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b2234-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2234-205">Response</span></span>

<span data-ttu-id="b2234-206">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b2234-206">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b2234-207">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2234-207">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
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

