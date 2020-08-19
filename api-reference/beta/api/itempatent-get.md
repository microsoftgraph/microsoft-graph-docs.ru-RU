---
title: Получение Итемпатент
description: Чтение свойств и связей объекта Итемпатент.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8a431414c31844173f3609f81cc972e04adeb11d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809749"
---
# <a name="get-itempatent"></a><span data-ttu-id="24019-103">Получение Итемпатент</span><span class="sxs-lookup"><span data-stu-id="24019-103">Get itemPatent</span></span>

<span data-ttu-id="24019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24019-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24019-105">Чтение свойств и связей объекта [итемпатент](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="24019-105">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24019-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24019-106">Permissions</span></span>

<span data-ttu-id="24019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24019-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24019-109">Permission type</span></span>                        | <span data-ttu-id="24019-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24019-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="24019-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24019-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24019-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24019-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="24019-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24019-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24019-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24019-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="24019-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="24019-115">Application</span></span>                            | <span data-ttu-id="24019-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24019-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="24019-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24019-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/patents/{id}
GET /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24019-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24019-118">Optional query parameters</span></span>

<span data-ttu-id="24019-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="24019-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="24019-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="24019-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="24019-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="24019-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24019-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24019-122">Request headers</span></span>
|<span data-ttu-id="24019-123">Имя</span><span class="sxs-lookup"><span data-stu-id="24019-123">Name</span></span>|<span data-ttu-id="24019-124">Описание</span><span class="sxs-lookup"><span data-stu-id="24019-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24019-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24019-125">Authorization</span></span>|<span data-ttu-id="24019-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24019-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24019-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24019-128">Request body</span></span>
<span data-ttu-id="24019-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24019-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24019-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="24019-130">Response</span></span>

<span data-ttu-id="24019-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итемпатент](../resources/itempatent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24019-131">If successful, this method returns a `200 OK` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24019-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="24019-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24019-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="24019-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="24019-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="24019-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempatent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="24019-135">C#</span><span class="sxs-lookup"><span data-stu-id="24019-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24019-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24019-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24019-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24019-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="24019-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="24019-138">Response</span></span>

<span data-ttu-id="24019-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="24019-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
