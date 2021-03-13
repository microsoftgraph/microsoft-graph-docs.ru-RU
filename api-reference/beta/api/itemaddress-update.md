---
title: Обновление itemAddress
description: Обновление свойств объекта itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6b761de97ba3c39917f42c0bb110c949f5e6185b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774659"
---
# <a name="update-itemaddress"></a><span data-ttu-id="a4f0b-103">Обновление itemAddress</span><span class="sxs-lookup"><span data-stu-id="a4f0b-103">Update itemAddress</span></span>
<span data-ttu-id="a4f0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4f0b-105">Обновление свойств объекта [itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a4f0b-105">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f0b-106">Permissions</span></span>

<span data-ttu-id="a4f0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4f0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f0b-109">Permission type</span></span>                        | <span data-ttu-id="a4f0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4f0b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a4f0b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4f0b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f0b-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a4f0b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4f0b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f0b-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a4f0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4f0b-115">Application</span></span>                            | <span data-ttu-id="a4f0b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f0b-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="a4f0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f0b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/addresses/{id}
PATCH /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4f0b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4f0b-118">Request headers</span></span>
|<span data-ttu-id="a4f0b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4f0b-119">Name</span></span>|<span data-ttu-id="a4f0b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f0b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4f0b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f0b-121">Authorization</span></span>|<span data-ttu-id="a4f0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4f0b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4f0b-124">Content-Type</span></span>|<span data-ttu-id="a4f0b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4f0b-127">Request body</span></span>

<span data-ttu-id="a4f0b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a4f0b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a4f0b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="a4f0b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4f0b-131">Property</span></span>|<span data-ttu-id="a4f0b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f0b-132">Type</span></span>|<span data-ttu-id="a4f0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f0b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4f0b-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a4f0b-134">allowedAudiences</span></span>|<span data-ttu-id="a4f0b-135">String</span><span class="sxs-lookup"><span data-stu-id="a4f0b-135">String</span></span>|<span data-ttu-id="a4f0b-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a4f0b-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a4f0b-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a4f0b-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a4f0b-139">подробные</span><span class="sxs-lookup"><span data-stu-id="a4f0b-139">detail</span></span>|[<span data-ttu-id="a4f0b-140">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a4f0b-140">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a4f0b-141">Сведения о самом адресе.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-141">Details about the address itself.</span></span>|
|<span data-ttu-id="a4f0b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a4f0b-142">displayName</span></span>|<span data-ttu-id="a4f0b-143">String</span><span class="sxs-lookup"><span data-stu-id="a4f0b-143">String</span></span>|<span data-ttu-id="a4f0b-144">Удобное имя, назначенное пользователю по этому адресу.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-144">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="a4f0b-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a4f0b-145">geoCoordinates</span></span>|[<span data-ttu-id="a4f0b-146">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a4f0b-146">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="a4f0b-147">Геокоординирует адрес.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-147">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="a4f0b-148">вывод</span><span class="sxs-lookup"><span data-stu-id="a4f0b-148">inference</span></span>|[<span data-ttu-id="a4f0b-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a4f0b-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a4f0b-150">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a4f0b-151">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a4f0b-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a4f0b-152">source</span><span class="sxs-lookup"><span data-stu-id="a4f0b-152">source</span></span>|[<span data-ttu-id="a4f0b-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a4f0b-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a4f0b-154">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a4f0b-155">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="a4f0b-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a4f0b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f0b-156">Response</span></span>

<span data-ttu-id="a4f0b-157">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект itemAddress](../resources/itemaddress.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-157">If successful, this method returns a `200 OK` response code and an updated [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4f0b-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4f0b-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4f0b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f0b-159">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="a4f0b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f0b-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemaddress"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
Content-Type: application/json
Content-length: 497

{
  "allowedAudiences": "me",
  "displayName": "Secret Hideout",
}
```
# <a name="c"></a>[<span data-ttu-id="a4f0b-161">C#</span><span class="sxs-lookup"><span data-stu-id="a4f0b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4f0b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4f0b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4f0b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4f0b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4f0b-164">Java</span><span class="sxs-lookup"><span data-stu-id="a4f0b-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-itemaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a4f0b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f0b-165">Response</span></span>
<span data-ttu-id="a4f0b-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4f0b-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "displayName": "Secret Hideout",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```



