---
title: Создание адресов
description: Создайте новый объект Addresses.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f84daa0eb3fbe594ec561af8e1a0b1a0f293fe19
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978935"
---
# <a name="create-addresses"></a><span data-ttu-id="8a06d-103">Создание адресов</span><span class="sxs-lookup"><span data-stu-id="8a06d-103">Create addresses</span></span>
<span data-ttu-id="8a06d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a06d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a06d-105">Создание нового объекта [итемаддресс](../resources/itemaddress.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a06d-105">Create a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a06d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a06d-106">Permissions</span></span>

<span data-ttu-id="8a06d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a06d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a06d-109">Permission type</span></span>                        | <span data-ttu-id="8a06d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a06d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8a06d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a06d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a06d-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8a06d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8a06d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a06d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a06d-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8a06d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8a06d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a06d-115">Application</span></span>                            | <span data-ttu-id="8a06d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a06d-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="8a06d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a06d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/addresses
POST /users/{id | userPrincipalName}/profile/addresses
```

## <a name="request-headers"></a><span data-ttu-id="8a06d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a06d-118">Request headers</span></span>
|<span data-ttu-id="8a06d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8a06d-119">Name</span></span>|<span data-ttu-id="8a06d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8a06d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a06d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a06d-121">Authorization</span></span>|<span data-ttu-id="8a06d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a06d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a06d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a06d-124">Content-Type</span></span>|<span data-ttu-id="8a06d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a06d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a06d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a06d-127">Request body</span></span>
<span data-ttu-id="8a06d-128">В тексте запроса добавьте представление объекта [итемаддресс](../resources/itemaddress.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a06d-128">In the request body, supply a JSON representation of the [itemAddress](../resources/itemaddress.md) object.</span></span>

<span data-ttu-id="8a06d-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемаддресс](../resources/itemaddress.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a06d-129">The following table shows the properties that are possible to set when creating a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="8a06d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a06d-130">Property</span></span>|<span data-ttu-id="8a06d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a06d-131">Type</span></span>|<span data-ttu-id="8a06d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a06d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a06d-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="8a06d-133">allowedAudiences</span></span>|<span data-ttu-id="8a06d-134">String</span><span class="sxs-lookup"><span data-stu-id="8a06d-134">String</span></span>|<span data-ttu-id="8a06d-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="8a06d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8a06d-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a06d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8a06d-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8a06d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8a06d-138">описаны</span><span class="sxs-lookup"><span data-stu-id="8a06d-138">detail</span></span>|[<span data-ttu-id="8a06d-139">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8a06d-139">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8a06d-140">Сведения о самом адресе.</span><span class="sxs-lookup"><span data-stu-id="8a06d-140">Details about the address itself.</span></span>|
|<span data-ttu-id="8a06d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8a06d-141">displayName</span></span>|<span data-ttu-id="8a06d-142">String</span><span class="sxs-lookup"><span data-stu-id="8a06d-142">String</span></span>|<span data-ttu-id="8a06d-143">Понятное имя, назначенное пользователю для этого адреса.</span><span class="sxs-lookup"><span data-stu-id="8a06d-143">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="8a06d-144">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8a06d-144">geoCoordinates</span></span>|[<span data-ttu-id="8a06d-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8a06d-145">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="8a06d-146">Геокоординаты адреса.</span><span class="sxs-lookup"><span data-stu-id="8a06d-146">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="8a06d-147">выводов</span><span class="sxs-lookup"><span data-stu-id="8a06d-147">inference</span></span>|[<span data-ttu-id="8a06d-148">инференцедата</span><span class="sxs-lookup"><span data-stu-id="8a06d-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8a06d-149">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="8a06d-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8a06d-150">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a06d-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8a06d-151">source</span><span class="sxs-lookup"><span data-stu-id="8a06d-151">source</span></span>|[<span data-ttu-id="8a06d-152">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="8a06d-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8a06d-153">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="8a06d-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8a06d-154">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8a06d-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
## <a name="response"></a><span data-ttu-id="8a06d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a06d-155">Response</span></span>

<span data-ttu-id="8a06d-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемаддресс](../resources/itemaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a06d-156">If successful, this method returns a `201 Created` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a06d-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a06d-157">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="8a06d-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a06d-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemaddress_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/addresses
Content-Type: application/json
Content-length: 497

{
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8a06d-159">C#</span><span class="sxs-lookup"><span data-stu-id="8a06d-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemaddress-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a06d-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a06d-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemaddress-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a06d-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a06d-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemaddress-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a06d-162">Java</span><span class="sxs-lookup"><span data-stu-id="8a06d-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itemaddress-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8a06d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a06d-163">Response</span></span>
<span data-ttu-id="8a06d-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a06d-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
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
  "displayName": "Home",
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


