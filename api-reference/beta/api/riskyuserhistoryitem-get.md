---
title: Получение элемента журнала для Рискюсер
description: Получение элемента журнала объекта Рискюсер.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db2743525ecb291f4d07afe6ea6ce379b938bfe4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863525"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="c9f26-103">Получение Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="c9f26-103">Get riskyUserHistoryItem</span></span>

<span data-ttu-id="c9f26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9f26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9f26-105">Получение объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) объекта [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="c9f26-105">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="c9f26-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c9f26-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9f26-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9f26-107">Permissions</span></span>
<span data-ttu-id="c9f26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9f26-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9f26-110">Permission type</span></span>      | <span data-ttu-id="c9f26-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9f26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9f26-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9f26-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9f26-113">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c9f26-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9f26-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9f26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9f26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f26-115">Not supported.</span></span>    |
|<span data-ttu-id="c9f26-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9f26-116">Application</span></span> | <span data-ttu-id="c9f26-117">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c9f26-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9f26-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9f26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
GET /identityProtection/riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="c9f26-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9f26-119">Request headers</span></span>
| <span data-ttu-id="c9f26-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c9f26-120">Name</span></span>      |<span data-ttu-id="c9f26-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c9f26-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9f26-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9f26-122">Authorization</span></span>  | <span data-ttu-id="c9f26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9f26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9f26-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9f26-125">Request body</span></span>
<span data-ttu-id="c9f26-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9f26-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9f26-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9f26-127">Response</span></span>

<span data-ttu-id="c9f26-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9f26-128">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9f26-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9f26-129">Examples</span></span>
### <a name="example-1-get-history-of-a-risky-user"></a><span data-ttu-id="c9f26-130">Пример 1: получение журнала опасного пользователя</span><span class="sxs-lookup"><span data-stu-id="c9f26-130">Example 1: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="c9f26-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9f26-131">Request</span></span>
<span data-ttu-id="c9f26-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9f26-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9f26-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9f26-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="c9f26-134">C#</span><span class="sxs-lookup"><span data-stu-id="c9f26-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9f26-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9f26-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9f26-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9f26-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c9f26-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9f26-137">Response</span></span>
<span data-ttu-id="c9f26-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9f26-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
        "eventTypes": [],
        "detail": "userPerformedSecuredPasswordReset"
    }
}
```

### <a name="example-2-get-history-of-a-risky-user"></a><span data-ttu-id="c9f26-139">Пример 2: получение истории опасного пользователя</span><span class="sxs-lookup"><span data-stu-id="c9f26-139">Example 2: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="c9f26-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9f26-140">Request</span></span>
<span data-ttu-id="c9f26-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9f26-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9f26-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9f26-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="c9f26-143">C#</span><span class="sxs-lookup"><span data-stu-id="c9f26-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9f26-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9f26-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9f26-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9f26-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c9f26-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9f26-146">Response</span></span>
<span data-ttu-id="c9f26-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9f26-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
        "eventTypes": [],
        "detail": "userPerformedSecuredPasswordReset"
    }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

