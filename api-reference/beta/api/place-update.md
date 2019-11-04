---
title: Обновление места
description: Обновление свойств объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 5e89dc031802ea420079bbbbbf5dd46f4fe181fc
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949512"
---
# <a name="update-place"></a><span data-ttu-id="f1fd6-103">Обновление места</span><span class="sxs-lookup"><span data-stu-id="f1fd6-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1fd6-104">Обновление свойств объекта [Place](../resources/place.md) , который может быть [комнатой](../resources/room.md) или [RoomList принимают одиночные](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="f1fd6-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="f1fd6-105">Можно определить **комнату** или **RoomList принимают одиночные** , указав свойство **ID** или **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="f1fd6-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1fd6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1fd6-106">Permissions</span></span>

<span data-ttu-id="f1fd6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1fd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1fd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1fd6-109">Permission type</span></span>                        | <span data-ttu-id="f1fd6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1fd6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1fd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1fd6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1fd6-112">Поместите. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="f1fd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1fd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1fd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-114">Not supported.</span></span> |
| <span data-ttu-id="f1fd6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1fd6-115">Application</span></span>                            | <span data-ttu-id="f1fd6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f1fd6-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1fd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1fd6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1fd6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1fd6-118">Request headers</span></span>

| <span data-ttu-id="f1fd6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1fd6-119">Name</span></span>       | <span data-ttu-id="f1fd6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f1fd6-120">Type</span></span> | <span data-ttu-id="f1fd6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f1fd6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1fd6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1fd6-122">Authorization</span></span>  | <span data-ttu-id="f1fd6-123">string</span><span class="sxs-lookup"><span data-stu-id="f1fd6-123">string</span></span>  | <span data-ttu-id="f1fd6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1fd6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1fd6-126">Request body</span></span>

<span data-ttu-id="f1fd6-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f1fd6-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f1fd6-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1fd6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1fd6-130">Property</span></span>               | <span data-ttu-id="f1fd6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1fd6-131">Type</span></span>                                              | <span data-ttu-id="f1fd6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1fd6-132">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="f1fd6-133">address</span><span class="sxs-lookup"><span data-stu-id="f1fd6-133">address</span></span>                | [<span data-ttu-id="f1fd6-134">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f1fd6-134">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="f1fd6-135">Почтовый адрес комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-135">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="f1fd6-136">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="f1fd6-136">audioDeviceName</span></span>        | <span data-ttu-id="f1fd6-137">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-137">String</span></span>                                            | <span data-ttu-id="f1fd6-138">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-138">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="f1fd6-139">букингтипе</span><span class="sxs-lookup"><span data-stu-id="f1fd6-139">bookingType</span></span>            | [<span data-ttu-id="f1fd6-140">букингтипе</span><span class="sxs-lookup"><span data-stu-id="f1fd6-140">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="f1fd6-141">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-141">Type of room.</span></span> <span data-ttu-id="f1fd6-142">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-142">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="f1fd6-143">создания</span><span class="sxs-lookup"><span data-stu-id="f1fd6-143">building</span></span>               | <span data-ttu-id="f1fd6-144">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-144">String</span></span>                                            | <span data-ttu-id="f1fd6-145">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-145">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="f1fd6-146">мощности</span><span class="sxs-lookup"><span data-stu-id="f1fd6-146">capacity</span></span>               | <span data-ttu-id="f1fd6-147">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-147">String</span></span>                                            | <span data-ttu-id="f1fd6-148">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-148">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="f1fd6-149">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="f1fd6-149">displayDeviceName</span></span>      | <span data-ttu-id="f1fd6-150">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-150">String</span></span>                                            | <span data-ttu-id="f1fd6-151">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-151">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="f1fd6-152">флурлабел</span><span class="sxs-lookup"><span data-stu-id="f1fd6-152">floorLabel</span></span>             | <span data-ttu-id="f1fd6-153">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-153">String</span></span>                                            | <span data-ttu-id="f1fd6-154">Указывает этаж, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-154">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="f1fd6-155">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="f1fd6-155">floorNumber</span></span>            | <span data-ttu-id="f1fd6-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f1fd6-156">Int32</span></span>                                             | <span data-ttu-id="f1fd6-157">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-157">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="f1fd6-158">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f1fd6-158">geoCoordinates</span></span>         | [<span data-ttu-id="f1fd6-159">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f1fd6-159">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="f1fd6-160">Указывает место в комнате или RoomList принимают одиночные в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-160">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="f1fd6-161">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="f1fd6-161">isWheelchairAccessible</span></span> | <span data-ttu-id="f1fd6-162">Логический</span><span class="sxs-lookup"><span data-stu-id="f1fd6-162">Boolean</span></span>                                           | <span data-ttu-id="f1fd6-163">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="f1fd6-164">label</span><span class="sxs-lookup"><span data-stu-id="f1fd6-164">label</span></span>                  | <span data-ttu-id="f1fd6-165">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-165">String</span></span>                                            | <span data-ttu-id="f1fd6-166">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="f1fd6-167">прозвищ</span><span class="sxs-lookup"><span data-stu-id="f1fd6-167">nickname</span></span>               | <span data-ttu-id="f1fd6-168">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-168">String</span></span>                                            | <span data-ttu-id="f1fd6-169">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="f1fd6-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="f1fd6-170">phone</span><span class="sxs-lookup"><span data-stu-id="f1fd6-170">phone</span></span>                  | <span data-ttu-id="f1fd6-171">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-171">String</span></span>                                            | <span data-ttu-id="f1fd6-172">Номер телефона комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-172">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="f1fd6-173">tags</span><span class="sxs-lookup"><span data-stu-id="f1fd6-173">tags</span></span>                   | <span data-ttu-id="f1fd6-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-174">String collection</span></span>                                 | <span data-ttu-id="f1fd6-175">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="f1fd6-176">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="f1fd6-176">videoDeviceName</span></span>        | <span data-ttu-id="f1fd6-177">String</span><span class="sxs-lookup"><span data-stu-id="f1fd6-177">String</span></span>                                            | <span data-ttu-id="f1fd6-178">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-178">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="f1fd6-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1fd6-179">Response</span></span>

<span data-ttu-id="f1fd6-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-180">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1fd6-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1fd6-181">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="f1fd6-182">Пример 1: обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="f1fd6-182">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="f1fd6-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1fd6-183">Request</span></span>

<span data-ttu-id="f1fd6-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-184">The following is an example of the request.</span></span>


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

### <a name="response"></a><span data-ttu-id="f1fd6-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1fd6-185">Response</span></span>

<span data-ttu-id="f1fd6-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-186">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f1fd6-187">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-187">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1fd6-188">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-188">All the properties will be returned from an actual call.</span></span>

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
      "latitude": 47.640568390488626,
      "longitude": -122.1293731033803
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="f1fd6-189">Пример 2: обновление объекта RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="f1fd6-189">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="f1fd6-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1fd6-190">Request</span></span>

<span data-ttu-id="f1fd6-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-191">The following is an example of the request.</span></span>


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
  "phone":"555-555-0100"
}
```

### <a name="response"></a><span data-ttu-id="f1fd6-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1fd6-192">Response</span></span>

<span data-ttu-id="f1fd6-193">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f1fd6-194">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1fd6-195">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1fd6-195">All the properties will be returned from an actual call.</span></span>

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
  "geocoordinates": null,
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
