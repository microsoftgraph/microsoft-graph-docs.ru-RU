---
title: Получение Итемпатент
description: Чтение свойств и связей объекта Итемпатент.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c287bcb4b77e6c997696006105f248e79c4b2dc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090000"
---
# <a name="get-itempatent"></a><span data-ttu-id="40df3-103">Получение Итемпатент</span><span class="sxs-lookup"><span data-stu-id="40df3-103">Get itemPatent</span></span>

<span data-ttu-id="40df3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40df3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40df3-105">Чтение свойств и связей объекта [итемпатент](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="40df3-105">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40df3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40df3-106">Permissions</span></span>

<span data-ttu-id="40df3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40df3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40df3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40df3-109">Permission type</span></span>                        | <span data-ttu-id="40df3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40df3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="40df3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40df3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40df3-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="40df3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="40df3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40df3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40df3-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="40df3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="40df3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40df3-115">Application</span></span>                            | <span data-ttu-id="40df3-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="40df3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="40df3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40df3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/patents/{id}
GET /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40df3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40df3-118">Optional query parameters</span></span>

<span data-ttu-id="40df3-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="40df3-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="40df3-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="40df3-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="40df3-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="40df3-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40df3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40df3-122">Request headers</span></span>
|<span data-ttu-id="40df3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="40df3-123">Name</span></span>|<span data-ttu-id="40df3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="40df3-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40df3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40df3-125">Authorization</span></span>|<span data-ttu-id="40df3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40df3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40df3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40df3-128">Request body</span></span>
<span data-ttu-id="40df3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40df3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40df3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="40df3-130">Response</span></span>

<span data-ttu-id="40df3-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итемпатент](../resources/itempatent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40df3-131">If successful, this method returns a `200 OK` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40df3-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="40df3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40df3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="40df3-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="40df3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40df3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempatent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="40df3-135">C#</span><span class="sxs-lookup"><span data-stu-id="40df3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40df3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40df3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40df3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40df3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="40df3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="40df3-138">Response</span></span>

<span data-ttu-id="40df3-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="40df3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```


