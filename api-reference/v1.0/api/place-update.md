---
title: Обновление места
description: Обновление свойств объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: d9d966a0fd901ccb040e0a15bbff88c247032bd3
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336392"
---
# <a name="update-place"></a><span data-ttu-id="31051-103">Обновление места</span><span class="sxs-lookup"><span data-stu-id="31051-103">Update place</span></span>

<span data-ttu-id="31051-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31051-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="31051-105">Обновление свойств объекта [Place](../resources/place.md) , который может быть [комнатой](../resources/room.md) или [RoomList принимают одиночные](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="31051-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="31051-106">Можно определить **комнату** или **RoomList принимают одиночные** , указав свойство **ID** или **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="31051-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="31051-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31051-107">Permissions</span></span>

<span data-ttu-id="31051-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31051-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31051-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31051-110">Permission type</span></span>                        | <span data-ttu-id="31051-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31051-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31051-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31051-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31051-113">Поместите. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="31051-113">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="31051-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31051-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31051-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31051-115">Not supported.</span></span> |
| <span data-ttu-id="31051-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31051-116">Application</span></span>                            | <span data-ttu-id="31051-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31051-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="31051-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31051-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="31051-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31051-119">Request headers</span></span>

| <span data-ttu-id="31051-120">Имя</span><span class="sxs-lookup"><span data-stu-id="31051-120">Name</span></span>       | <span data-ttu-id="31051-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31051-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="31051-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31051-122">Authorization</span></span>  | <span data-ttu-id="31051-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31051-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31051-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31051-125">Content-Type</span></span> | <span data-ttu-id="31051-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31051-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31051-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31051-128">Request body</span></span>

<span data-ttu-id="31051-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="31051-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="31051-130">За один раз можно обновить только один экземпляр ресурса "помещение" (**комната** или **RoomList принимают одиночные**).</span><span class="sxs-lookup"><span data-stu-id="31051-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="31051-131">В тексте запроса `@odata.type` Укажите тип размещения и включите свойства этого типа для обновления.</span><span class="sxs-lookup"><span data-stu-id="31051-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="31051-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="31051-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="31051-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="31051-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="31051-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="31051-134">Property</span></span>               | <span data-ttu-id="31051-135">Тип</span><span class="sxs-lookup"><span data-stu-id="31051-135">Type</span></span>                                              | <span data-ttu-id="31051-136">Описание</span><span class="sxs-lookup"><span data-stu-id="31051-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="31051-137">address</span><span class="sxs-lookup"><span data-stu-id="31051-137">address</span></span>                | [<span data-ttu-id="31051-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="31051-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="31051-139">Почтовый адрес комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="31051-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="31051-140">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="31051-140">audioDeviceName</span></span>        | <span data-ttu-id="31051-141">String</span><span class="sxs-lookup"><span data-stu-id="31051-141">String</span></span>                                            | <span data-ttu-id="31051-142">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="31051-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="31051-143">букингтипе</span><span class="sxs-lookup"><span data-stu-id="31051-143">bookingType</span></span>            | [<span data-ttu-id="31051-144">букингтипе</span><span class="sxs-lookup"><span data-stu-id="31051-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="31051-145">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="31051-145">Type of room.</span></span> <span data-ttu-id="31051-146">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="31051-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="31051-147">создания</span><span class="sxs-lookup"><span data-stu-id="31051-147">building</span></span>               | <span data-ttu-id="31051-148">String</span><span class="sxs-lookup"><span data-stu-id="31051-148">String</span></span>                                            | <span data-ttu-id="31051-149">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="31051-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="31051-150">мощности</span><span class="sxs-lookup"><span data-stu-id="31051-150">capacity</span></span>               | <span data-ttu-id="31051-151">String</span><span class="sxs-lookup"><span data-stu-id="31051-151">String</span></span>                                            | <span data-ttu-id="31051-152">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="31051-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="31051-153">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="31051-153">displayDeviceName</span></span>      | <span data-ttu-id="31051-154">String</span><span class="sxs-lookup"><span data-stu-id="31051-154">String</span></span>                                            | <span data-ttu-id="31051-155">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="31051-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="31051-156">флурлабел</span><span class="sxs-lookup"><span data-stu-id="31051-156">floorLabel</span></span>             | <span data-ttu-id="31051-157">String</span><span class="sxs-lookup"><span data-stu-id="31051-157">String</span></span>                                            | <span data-ttu-id="31051-158">Указывает этаж, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="31051-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="31051-159">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="31051-159">floorNumber</span></span>            | <span data-ttu-id="31051-160">Int32</span><span class="sxs-lookup"><span data-stu-id="31051-160">Int32</span></span>                                             | <span data-ttu-id="31051-161">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="31051-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="31051-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="31051-162">geoCoordinates</span></span>         | [<span data-ttu-id="31051-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="31051-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="31051-164">Указывает место в комнате или RoomList принимают одиночные в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="31051-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="31051-165">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="31051-165">isWheelchairAccessible</span></span> | <span data-ttu-id="31051-166">Логический</span><span class="sxs-lookup"><span data-stu-id="31051-166">Boolean</span></span>                                           | <span data-ttu-id="31051-167">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="31051-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="31051-168">label</span><span class="sxs-lookup"><span data-stu-id="31051-168">label</span></span>                  | <span data-ttu-id="31051-169">String</span><span class="sxs-lookup"><span data-stu-id="31051-169">String</span></span>                                            | <span data-ttu-id="31051-170">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="31051-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="31051-171">прозвищ</span><span class="sxs-lookup"><span data-stu-id="31051-171">nickname</span></span>               | <span data-ttu-id="31051-172">String</span><span class="sxs-lookup"><span data-stu-id="31051-172">String</span></span>                                            | <span data-ttu-id="31051-173">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="31051-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="31051-174">phone</span><span class="sxs-lookup"><span data-stu-id="31051-174">phone</span></span>                  | <span data-ttu-id="31051-175">String</span><span class="sxs-lookup"><span data-stu-id="31051-175">String</span></span>                                            | <span data-ttu-id="31051-176">Номер телефона комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="31051-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="31051-177">tags</span><span class="sxs-lookup"><span data-stu-id="31051-177">tags</span></span>                   | <span data-ttu-id="31051-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31051-178">String collection</span></span>                                 | <span data-ttu-id="31051-179">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="31051-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="31051-180">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="31051-180">videoDeviceName</span></span>        | <span data-ttu-id="31051-181">String</span><span class="sxs-lookup"><span data-stu-id="31051-181">String</span></span>                                            | <span data-ttu-id="31051-182">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="31051-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="31051-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="31051-183">Response</span></span>

<span data-ttu-id="31051-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31051-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31051-185">Примеры</span><span class="sxs-lookup"><span data-stu-id="31051-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="31051-186">Пример 1: обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="31051-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="31051-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="31051-187">Request</span></span>

<span data-ttu-id="31051-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31051-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="31051-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="31051-189">HTTP</span></span>](#tab/http)
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
  "capacity": "50",
  "isWheelchairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="31051-190">C#</span><span class="sxs-lookup"><span data-stu-id="31051-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31051-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31051-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31051-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31051-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31051-193">Java</span><span class="sxs-lookup"><span data-stu-id="31051-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31051-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="31051-194">Response</span></span>

<span data-ttu-id="31051-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31051-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="31051-196">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31051-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31051-197">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31051-197">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="31051-198">Пример 2: обновление объекта RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="31051-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="31051-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="31051-199">Request</span></span>

<span data-ttu-id="31051-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31051-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31051-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="31051-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
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
# <a name="c"></a>[<span data-ttu-id="31051-202">C#</span><span class="sxs-lookup"><span data-stu-id="31051-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31051-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31051-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31051-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31051-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31051-205">Java</span><span class="sxs-lookup"><span data-stu-id="31051-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="31051-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="31051-206">Response</span></span>

<span data-ttu-id="31051-207">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31051-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="31051-208">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31051-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31051-209">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31051-209">All the properties will be returned from an actual call.</span></span>

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
