---
title: Получение
description: Получение свойств и связей объекта Place.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b53f6b1cb89bb4c5b3d02d5b32154877a5de706
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841068"
---
# <a name="get-place"></a><span data-ttu-id="31177-103">Получение</span><span class="sxs-lookup"><span data-stu-id="31177-103">Get place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="31177-104">Получение свойств и связей объекта [Place](../resources/place.md) , указанных с помощью его идентификатора или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="31177-104">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="31177-105">Объект **Place** может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="31177-105">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="31177-106">[Комната](../resources/room.md) , включающая в себя обширные свойства, такие как адрес электронной почты для комнаты, Специальные возможности, мощность и поддержка устройств.</span><span class="sxs-lookup"><span data-stu-id="31177-106">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="31177-107">[Список помещений](../resources/roomlist.md) , включающий адрес электронной почты для списка помещений, и свойство навигации для получения коллекции экземпляров **комнаты** в этом списке.</span><span class="sxs-lookup"><span data-stu-id="31177-107">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="31177-108">**Комната** и **RoomList принимают одиночные** являются производными от объекта [Place](../resources/place.md) .</span><span class="sxs-lookup"><span data-stu-id="31177-108">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="31177-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31177-109">Permissions</span></span>

<span data-ttu-id="31177-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31177-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31177-112">Permission type</span></span>                        | <span data-ttu-id="31177-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31177-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31177-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31177-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="31177-115">Размещение. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="31177-115">Place.Read.All</span></span> |
| <span data-ttu-id="31177-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31177-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31177-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31177-117">Not supported</span></span> |
| <span data-ttu-id="31177-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31177-118">Application</span></span>                            | <span data-ttu-id="31177-119">Размещение. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="31177-119">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31177-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31177-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31177-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31177-121">Optional query parameters</span></span>

<span data-ttu-id="31177-122">Этот метод поддерживает следующие параметры запроса, помогающие настроить ответ:</span><span class="sxs-lookup"><span data-stu-id="31177-122">This method supports the following query parameters to help customize the response:</span></span>
* <span data-ttu-id="31177-123">$filter</span><span class="sxs-lookup"><span data-stu-id="31177-123">$filter</span></span>
* <span data-ttu-id="31177-124">$select</span><span class="sxs-lookup"><span data-stu-id="31177-124">$select</span></span>
* <span data-ttu-id="31177-125">$top</span><span class="sxs-lookup"><span data-stu-id="31177-125">$top</span></span>

<span data-ttu-id="31177-126">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="31177-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31177-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31177-127">Request headers</span></span>

| <span data-ttu-id="31177-128">Имя</span><span class="sxs-lookup"><span data-stu-id="31177-128">Name</span></span>          | <span data-ttu-id="31177-129">Описание</span><span class="sxs-lookup"><span data-stu-id="31177-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="31177-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31177-130">Authorization</span></span> | <span data-ttu-id="31177-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31177-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31177-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31177-133">Request body</span></span>

<span data-ttu-id="31177-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31177-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31177-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="31177-135">Response</span></span>

<span data-ttu-id="31177-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Place](../resources/place.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31177-136">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31177-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="31177-137">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="31177-138">Пример 1: получение комнаты</span><span class="sxs-lookup"><span data-stu-id="31177-138">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="31177-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="31177-139">Request</span></span>

<span data-ttu-id="31177-140">В следующем примере задается **идентификатор** **комнаты** для получения ее свойств.</span><span class="sxs-lookup"><span data-stu-id="31177-140">The following example specifies the **id** of a **room** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```http
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```

#### <a name="response"></a><span data-ttu-id="31177-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="31177-141">Response</span></span>

<span data-ttu-id="31177-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="31177-142">The following is an example of the response.</span></span>

><span data-ttu-id="31177-143">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31177-143">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31177-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31177-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="31177-145">Пример 2: получение списка помещений</span><span class="sxs-lookup"><span data-stu-id="31177-145">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="31177-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="31177-146">Request</span></span>

<span data-ttu-id="31177-147">В следующем примере задается значение **EmailAddress** объекта **RoomList принимают одиночные** для получения его свойств.</span><span class="sxs-lookup"><span data-stu-id="31177-147">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```

#### <a name="response"></a><span data-ttu-id="31177-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="31177-148">Response</span></span>

<span data-ttu-id="31177-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="31177-149">The following is an example of the response.</span></span>

><span data-ttu-id="31177-150">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31177-150">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31177-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31177-151">All the properties will be returned from an actual call.</span></span>

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
