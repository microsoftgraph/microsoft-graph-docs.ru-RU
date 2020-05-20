---
title: Обновление места
description: Обновление свойств объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3caf019dd8966ca6bbeba9f3a150b2bdbc552925
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288889"
---
# <a name="update-place"></a><span data-ttu-id="f38ed-103">Обновление места</span><span class="sxs-lookup"><span data-stu-id="f38ed-103">Update place</span></span>

<span data-ttu-id="f38ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f38ed-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="f38ed-105">Обновление свойств объекта [Place](../resources/place.md) , который может быть [комнатой](../resources/room.md) или [RoomList принимают одиночные](../resources/roomlist.md).</span><span class="sxs-lookup"><span data-stu-id="f38ed-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="f38ed-106">Можно определить **комнату** или **RoomList принимают одиночные** , указав свойство **ID** или **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="f38ed-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f38ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f38ed-107">Permissions</span></span>

<span data-ttu-id="f38ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f38ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f38ed-110">Permission type</span></span>                        | <span data-ttu-id="f38ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f38ed-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f38ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f38ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f38ed-113">Поместите. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="f38ed-113">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="f38ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f38ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f38ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f38ed-115">Not supported.</span></span> |
| <span data-ttu-id="f38ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f38ed-116">Application</span></span>                            | <span data-ttu-id="f38ed-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f38ed-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="f38ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f38ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="f38ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f38ed-119">Request headers</span></span>

| <span data-ttu-id="f38ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f38ed-120">Name</span></span>       | <span data-ttu-id="f38ed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f38ed-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f38ed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f38ed-122">Authorization</span></span>  | <span data-ttu-id="f38ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f38ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f38ed-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f38ed-125">Content-Type</span></span> | <span data-ttu-id="f38ed-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f38ed-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f38ed-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f38ed-128">Request body</span></span>

<span data-ttu-id="f38ed-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f38ed-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f38ed-130">За один раз можно обновить только один экземпляр ресурса "помещение" (**комната** или **RoomList принимают одиночные**).</span><span class="sxs-lookup"><span data-stu-id="f38ed-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="f38ed-131">В тексте запроса `@odata.type` Укажите тип размещения и включите свойства этого типа для обновления.</span><span class="sxs-lookup"><span data-stu-id="f38ed-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="f38ed-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f38ed-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f38ed-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f38ed-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f38ed-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="f38ed-134">Property</span></span>               | <span data-ttu-id="f38ed-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f38ed-135">Type</span></span>                                              | <span data-ttu-id="f38ed-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f38ed-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="f38ed-137">address</span><span class="sxs-lookup"><span data-stu-id="f38ed-137">address</span></span>                | [<span data-ttu-id="f38ed-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f38ed-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="f38ed-139">Почтовый адрес комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="f38ed-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="f38ed-140">аудиодевиценаме</span><span class="sxs-lookup"><span data-stu-id="f38ed-140">audioDeviceName</span></span>        | <span data-ttu-id="f38ed-141">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-141">String</span></span>                                            | <span data-ttu-id="f38ed-142">Указывает имя звукового устройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="f38ed-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="f38ed-143">букингтипе</span><span class="sxs-lookup"><span data-stu-id="f38ed-143">bookingType</span></span>            | [<span data-ttu-id="f38ed-144">букингтипе</span><span class="sxs-lookup"><span data-stu-id="f38ed-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="f38ed-145">Тип комнаты.</span><span class="sxs-lookup"><span data-stu-id="f38ed-145">Type of room.</span></span> <span data-ttu-id="f38ed-146">Возможные значения: `Standard` и `Reserved`.</span><span class="sxs-lookup"><span data-stu-id="f38ed-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="f38ed-147">создания</span><span class="sxs-lookup"><span data-stu-id="f38ed-147">building</span></span>               | <span data-ttu-id="f38ed-148">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-148">String</span></span>                                            | <span data-ttu-id="f38ed-149">Задает имя здания или номер здания, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f38ed-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="f38ed-150">мощности</span><span class="sxs-lookup"><span data-stu-id="f38ed-150">capacity</span></span>               | <span data-ttu-id="f38ed-151">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-151">String</span></span>                                            | <span data-ttu-id="f38ed-152">Указывает емкость комнаты.</span><span class="sxs-lookup"><span data-stu-id="f38ed-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="f38ed-153">дисплайдевиценаме</span><span class="sxs-lookup"><span data-stu-id="f38ed-153">displayDeviceName</span></span>      | <span data-ttu-id="f38ed-154">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-154">String</span></span>                                            | <span data-ttu-id="f38ed-155">Задает имя устройства отображения в комнате.</span><span class="sxs-lookup"><span data-stu-id="f38ed-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="f38ed-156">флурлабел</span><span class="sxs-lookup"><span data-stu-id="f38ed-156">floorLabel</span></span>             | <span data-ttu-id="f38ed-157">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-157">String</span></span>                                            | <span data-ttu-id="f38ed-158">Указывает этаж, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f38ed-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="f38ed-159">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="f38ed-159">floorNumber</span></span>            | <span data-ttu-id="f38ed-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f38ed-160">Int32</span></span>                                             | <span data-ttu-id="f38ed-161">Указывает номер этажа, в котором находится комната.</span><span class="sxs-lookup"><span data-stu-id="f38ed-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="f38ed-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f38ed-162">geoCoordinates</span></span>         | [<span data-ttu-id="f38ed-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f38ed-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="f38ed-164">Указывает место в комнате или RoomList принимают одиночные в широте, долготе и дополнительном координатах высоты.</span><span class="sxs-lookup"><span data-stu-id="f38ed-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="f38ed-165">исвхилчаиракцессибле</span><span class="sxs-lookup"><span data-stu-id="f38ed-165">isWheelchairAccessible</span></span> | <span data-ttu-id="f38ed-166">Логический</span><span class="sxs-lookup"><span data-stu-id="f38ed-166">Boolean</span></span>                                           | <span data-ttu-id="f38ed-167">Указывает, является ли комната вхилчаир доступным.</span><span class="sxs-lookup"><span data-stu-id="f38ed-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="f38ed-168">label</span><span class="sxs-lookup"><span data-stu-id="f38ed-168">label</span></span>                  | <span data-ttu-id="f38ed-169">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-169">String</span></span>                                            | <span data-ttu-id="f38ed-170">Задает описательную метку для комнаты, например номер или имя.</span><span class="sxs-lookup"><span data-stu-id="f38ed-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="f38ed-171">прозвищ</span><span class="sxs-lookup"><span data-stu-id="f38ed-171">nickname</span></span>               | <span data-ttu-id="f38ed-172">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-172">String</span></span>                                            | <span data-ttu-id="f38ed-173">Задает псевдоним для комнаты, например "назначение комнаты".</span><span class="sxs-lookup"><span data-stu-id="f38ed-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="f38ed-174">phone</span><span class="sxs-lookup"><span data-stu-id="f38ed-174">phone</span></span>                  | <span data-ttu-id="f38ed-175">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-175">String</span></span>                                            | <span data-ttu-id="f38ed-176">Номер телефона комнаты или RoomList принимают одиночные.</span><span class="sxs-lookup"><span data-stu-id="f38ed-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="f38ed-177">tags</span><span class="sxs-lookup"><span data-stu-id="f38ed-177">tags</span></span>                   | <span data-ttu-id="f38ed-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f38ed-178">String collection</span></span>                                 | <span data-ttu-id="f38ed-179">Задает дополнительные функции комнаты, например, сведения, например тип представления или тип мебели.</span><span class="sxs-lookup"><span data-stu-id="f38ed-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="f38ed-180">видеодевиценаме</span><span class="sxs-lookup"><span data-stu-id="f38ed-180">videoDeviceName</span></span>        | <span data-ttu-id="f38ed-181">String</span><span class="sxs-lookup"><span data-stu-id="f38ed-181">String</span></span>                                            | <span data-ttu-id="f38ed-182">Задает имя видеоустройства в комнате.</span><span class="sxs-lookup"><span data-stu-id="f38ed-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="f38ed-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38ed-183">Response</span></span>

<span data-ttu-id="f38ed-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f38ed-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f38ed-185">Примеры</span><span class="sxs-lookup"><span data-stu-id="f38ed-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="f38ed-186">Пример 1: обновление комнаты</span><span class="sxs-lookup"><span data-stu-id="f38ed-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="f38ed-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="f38ed-187">Request</span></span>

<span data-ttu-id="f38ed-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f38ed-188">The following is an example of the request.</span></span>


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

### <a name="response"></a><span data-ttu-id="f38ed-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38ed-189">Response</span></span>

<span data-ttu-id="f38ed-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f38ed-190">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f38ed-191">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f38ed-191">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f38ed-192">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f38ed-192">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="f38ed-193">Пример 2: обновление объекта RoomList принимают одиночные</span><span class="sxs-lookup"><span data-stu-id="f38ed-193">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="f38ed-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="f38ed-194">Request</span></span>

<span data-ttu-id="f38ed-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f38ed-195">The following is an example of the request.</span></span>

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


### <a name="response"></a><span data-ttu-id="f38ed-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38ed-196">Response</span></span>

<span data-ttu-id="f38ed-197">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f38ed-197">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f38ed-198">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f38ed-198">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f38ed-199">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f38ed-199">All the properties will be returned from an actual call.</span></span>

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
