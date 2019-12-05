---
title: Обновление места
description: Обновление свойств объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3e2e517d0a20384c8aaaa24e9f385cf5560c411e
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844192"
---
# <a name="update-place"></a><span data-ttu-id="22d68-103">Обновление места</span><span class="sxs-lookup"><span data-stu-id="22d68-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d68-104">Обновление свойств объекта [Place](../resources/place.md) , который может быть [комнатой](../resources/room.md) или [RoomList принимают одиночные](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="22d68-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="22d68-105">Можно определить **комнату** или **RoomList принимают одиночные** , указав свойство **ID** или **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="22d68-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="22d68-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22d68-106">Permissions</span></span>

<span data-ttu-id="22d68-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22d68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d68-109">Permission type</span></span>                        | <span data-ttu-id="22d68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d68-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22d68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d68-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22d68-112">Поместите. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="22d68-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="22d68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22d68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d68-114">Not supported.</span></span> |
| <span data-ttu-id="22d68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d68-115">Application</span></span>                            | <span data-ttu-id="22d68-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="22d68-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="22d68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d68-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="22d68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d68-118">Request headers</span></span>

| <span data-ttu-id="22d68-119">Имя</span><span class="sxs-lookup"><span data-stu-id="22d68-119">Name</span></span>       | <span data-ttu-id="22d68-120">Значение</span><span class="sxs-lookup"><span data-stu-id="22d68-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="22d68-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22d68-121">Authorization</span></span>  | <span data-ttu-id="22d68-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d68-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22d68-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22d68-124">Content-Type</span></span> | <span data-ttu-id="22d68-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d68-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22d68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22d68-127">Request body</span></span>

<span data-ttu-id="22d68-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="22d68-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="22d68-129">За один раз можно обновить только один экземпляр ресурса "помещение" (**комната** или **RoomList принимают одиночные**).</span><span class="sxs-lookup"><span data-stu-id="22d68-129">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="22d68-130">В тексте `@odata.type` запроса укажите тип размещения и включите свойства этого типа для обновления.</span><span class="sxs-lookup"><span data-stu-id="22d68-130">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="22d68-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="22d68-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="22d68-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="22d68-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="22d68-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="22d68-133">Property</span></span>               | <span data-ttu-id="22d68-134">Тип</span><span class="sxs-lookup"><span data-stu-id="22d68-134">Type</span></span>                                              | <span data-ttu-id="22d68-135">Описание</span><span class="sxs-lookup"><span data-stu-id="22d68-135">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="22d68-136">address</span><span class="sxs-lookup"><span data-stu-id="22d68-136">address</span></span>                | [<span data-ttu-id="22d68-137">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="22d68-137">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="22d68-138">Почтовый адрес комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="22d68-138">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="22d68-139">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="22d68-139">audioDeviceName</span></span>        | <span data-ttu-id="22d68-140">String</span><span class="sxs-lookup"><span data-stu-id="22d68-140">String</span></span>                                            | <span data-ttu-id="22d68-141">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="22d68-141">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="22d68-142">букингтипе</span><span class="sxs-lookup"><span data-stu-id="22d68-142">bookingType</span></span>            | [<span data-ttu-id="22d68-143">букингтипе</span><span class="sxs-lookup"><span data-stu-id="22d68-143">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="22d68-144">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="22d68-144">Type of room.</span></span> <span data-ttu-id="22d68-145">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="22d68-145">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="22d68-146">создания</span><span class="sxs-lookup"><span data-stu-id="22d68-146">building</span></span>               | <span data-ttu-id="22d68-147">String</span><span class="sxs-lookup"><span data-stu-id="22d68-147">String</span></span>                                            | <span data-ttu-id="22d68-148">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="22d68-148">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="22d68-149">мощности</span><span class="sxs-lookup"><span data-stu-id="22d68-149">capacity</span></span>               | <span data-ttu-id="22d68-150">String</span><span class="sxs-lookup"><span data-stu-id="22d68-150">String</span></span>                                            | <span data-ttu-id="22d68-151">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="22d68-151">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="22d68-152">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="22d68-152">displayDeviceName</span></span>      | <span data-ttu-id="22d68-153">String</span><span class="sxs-lookup"><span data-stu-id="22d68-153">String</span></span>                                            | <span data-ttu-id="22d68-154">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="22d68-154">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="22d68-155">флурлабел</span><span class="sxs-lookup"><span data-stu-id="22d68-155">floorLabel</span></span>             | <span data-ttu-id="22d68-156">String</span><span class="sxs-lookup"><span data-stu-id="22d68-156">String</span></span>                                            | <span data-ttu-id="22d68-157">Указывает этаж, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="22d68-157">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="22d68-158">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="22d68-158">floorNumber</span></span>            | <span data-ttu-id="22d68-159">Int32</span><span class="sxs-lookup"><span data-stu-id="22d68-159">Int32</span></span>                                             | <span data-ttu-id="22d68-160">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="22d68-160">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="22d68-161">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="22d68-161">geoCoordinates</span></span>         | [<span data-ttu-id="22d68-162">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="22d68-162">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="22d68-163">Указывает место в комнате или RoomList принимают одиночные в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="22d68-163">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="22d68-164">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="22d68-164">isWheelchairAccessible</span></span> | <span data-ttu-id="22d68-165">Логический</span><span class="sxs-lookup"><span data-stu-id="22d68-165">Boolean</span></span>                                           | <span data-ttu-id="22d68-166">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="22d68-166">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="22d68-167">label</span><span class="sxs-lookup"><span data-stu-id="22d68-167">label</span></span>                  | <span data-ttu-id="22d68-168">String</span><span class="sxs-lookup"><span data-stu-id="22d68-168">String</span></span>                                            | <span data-ttu-id="22d68-169">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="22d68-169">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="22d68-170">прозвищ</span><span class="sxs-lookup"><span data-stu-id="22d68-170">nickname</span></span>               | <span data-ttu-id="22d68-171">String</span><span class="sxs-lookup"><span data-stu-id="22d68-171">String</span></span>                                            | <span data-ttu-id="22d68-172">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="22d68-172">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="22d68-173">phone</span><span class="sxs-lookup"><span data-stu-id="22d68-173">phone</span></span>                  | <span data-ttu-id="22d68-174">String</span><span class="sxs-lookup"><span data-stu-id="22d68-174">String</span></span>                                            | <span data-ttu-id="22d68-175">Номер телефона комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="22d68-175">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="22d68-176">tags</span><span class="sxs-lookup"><span data-stu-id="22d68-176">tags</span></span>                   | <span data-ttu-id="22d68-177">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="22d68-177">String collection</span></span>                                 | <span data-ttu-id="22d68-178">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="22d68-178">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="22d68-179">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="22d68-179">videoDeviceName</span></span>        | <span data-ttu-id="22d68-180">String</span><span class="sxs-lookup"><span data-stu-id="22d68-180">String</span></span>                                            | <span data-ttu-id="22d68-181">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="22d68-181">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="22d68-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d68-182">Response</span></span>

<span data-ttu-id="22d68-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22d68-183">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22d68-184">Примеры</span><span class="sxs-lookup"><span data-stu-id="22d68-184">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="22d68-185">Пример 1: обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="22d68-185">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="22d68-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d68-186">Request</span></span>

<span data-ttu-id="22d68-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d68-187">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="22d68-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d68-188">HTTP</span></span>](#tab/http)
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
  "capacity": "50",
  "isWheelchairAccessible": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22d68-189">C#</span><span class="sxs-lookup"><span data-stu-id="22d68-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22d68-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22d68-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22d68-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22d68-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22d68-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d68-192">Response</span></span>

<span data-ttu-id="22d68-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22d68-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="22d68-194">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22d68-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="22d68-195">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22d68-195">All the properties will be returned from an actual call.</span></span>

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
    "capacity": "50",
    "building": "1",
    "floorLabel": "1P",
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="22d68-196">Пример 2: обновление объекта RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="22d68-196">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="22d68-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d68-197">Request</span></span>

<span data-ttu-id="22d68-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d68-198">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="22d68-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="22d68-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomlist",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="22d68-200">C#</span><span class="sxs-lookup"><span data-stu-id="22d68-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22d68-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22d68-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22d68-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22d68-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22d68-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d68-203">Response</span></span>

<span data-ttu-id="22d68-204">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22d68-204">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="22d68-205">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="22d68-205">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="22d68-206">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22d68-206">All the properties will be returned from an actual call.</span></span>

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
