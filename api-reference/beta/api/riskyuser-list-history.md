---
title: Список истории riskyUser
description: Извлечение истории рисков
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 28f10f6181d3bfa5091fdb2c98fb584c9bf26452
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440852"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="db3ae-103">Список истории riskyUser</span><span class="sxs-lookup"><span data-stu-id="db3ae-103">List history of riskyUser</span></span>

<span data-ttu-id="db3ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db3ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3ae-105">Получите историю рисков ресурса [riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="db3ae-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="db3ae-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="db3ae-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="db3ae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db3ae-107">Permissions</span></span>
<span data-ttu-id="db3ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db3ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db3ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db3ae-110">Permission type</span></span>      | <span data-ttu-id="db3ae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db3ae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db3ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db3ae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db3ae-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3ae-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="db3ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db3ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db3ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db3ae-115">Not supported.</span></span>    |
|<span data-ttu-id="db3ae-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="db3ae-116">Application</span></span> | <span data-ttu-id="db3ae-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3ae-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db3ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db3ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
GET /identityProtection/riskyUsers/{id}/history/
```


## <a name="request-headers"></a><span data-ttu-id="db3ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db3ae-119">Request headers</span></span>
| <span data-ttu-id="db3ae-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db3ae-120">Name</span></span>      |<span data-ttu-id="db3ae-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db3ae-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db3ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db3ae-122">Authorization</span></span>  | <span data-ttu-id="db3ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db3ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db3ae-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db3ae-125">Request body</span></span>
<span data-ttu-id="db3ae-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db3ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db3ae-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="db3ae-127">Response</span></span>

<span data-ttu-id="db3ae-128">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db3ae-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db3ae-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="db3ae-129">Examples</span></span>
### <a name="example-1-list-history-of-a-specific-user"></a><span data-ttu-id="db3ae-130">Пример 1. История списка определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="db3ae-130">Example 1: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="db3ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db3ae-131">Request</span></span>
<span data-ttu-id="db3ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db3ae-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db3ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db3ae-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="db3ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="db3ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db3ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db3ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db3ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db3ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db3ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="db3ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userriskhitsory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="db3ae-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db3ae-138">Response</span></span>
<span data-ttu-id="db3ae-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db3ae-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
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
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```
### <a name="example-2-list-history-of-a-specific-user"></a><span data-ttu-id="db3ae-140">Пример 2. История списка определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="db3ae-140">Example 2: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="db3ae-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="db3ae-141">Request</span></span>
<span data-ttu-id="db3ae-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db3ae-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db3ae-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="db3ae-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="db3ae-144">C#</span><span class="sxs-lookup"><span data-stu-id="db3ae-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db3ae-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db3ae-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db3ae-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db3ae-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db3ae-147">Java</span><span class="sxs-lookup"><span data-stu-id="db3ae-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userriskhitsory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="db3ae-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="db3ae-148">Response</span></span>
<span data-ttu-id="db3ae-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db3ae-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "isDeleted": false,
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
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



