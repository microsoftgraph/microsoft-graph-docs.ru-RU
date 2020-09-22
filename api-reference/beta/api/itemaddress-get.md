---
title: Получение Итемаддресс
description: Чтение свойств и связей объекта Итемаддресс.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4f284921536827b2c005cde1b938b1ecbaf60ef4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980008"
---
# <a name="get-itemaddress"></a><span data-ttu-id="fa093-103">Получение Итемаддресс</span><span class="sxs-lookup"><span data-stu-id="fa093-103">Get itemAddress</span></span>
<span data-ttu-id="fa093-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa093-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa093-105">Чтение свойств и связей объекта [итемаддресс](../resources/itemaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="fa093-105">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa093-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa093-106">Permissions</span></span>

<span data-ttu-id="fa093-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa093-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa093-109">Permission type</span></span>                        | <span data-ttu-id="fa093-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa093-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="fa093-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa093-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa093-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa093-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fa093-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa093-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa093-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa093-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fa093-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa093-115">Application</span></span>                            | <span data-ttu-id="fa093-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa093-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="fa093-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa093-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/addresses/{id}
GET /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa093-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa093-118">Optional query parameters</span></span>

<span data-ttu-id="fa093-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="fa093-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="fa093-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="fa093-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="fa093-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="fa093-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa093-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa093-122">Request headers</span></span>
|<span data-ttu-id="fa093-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fa093-123">Name</span></span>|<span data-ttu-id="fa093-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fa093-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa093-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa093-125">Authorization</span></span>|<span data-ttu-id="fa093-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa093-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa093-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa093-128">Request body</span></span>
<span data-ttu-id="fa093-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa093-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa093-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa093-130">Response</span></span>

<span data-ttu-id="fa093-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итемаддресс](../resources/itemaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa093-131">If successful, this method returns a `200 OK` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa093-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa093-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa093-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa093-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="fa093-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa093-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemaddress"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="fa093-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa093-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa093-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa093-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa093-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa093-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fa093-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa093-138">Response</span></span>

<span data-ttu-id="fa093-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa093-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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


