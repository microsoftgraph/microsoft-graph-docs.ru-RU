---
title: Журнал списка Рискюсер
description: Получение журнала рисков
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e8799e8f5bf2de0f2745a1dc5b09ab17a8066e62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871094"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="4ae92-103">Журнал списка Рискюсер</span><span class="sxs-lookup"><span data-stu-id="4ae92-103">List history of riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae92-104">Получение журнала рисков ресурса [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="4ae92-104">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="4ae92-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="4ae92-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ae92-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae92-106">Permissions</span></span>
<span data-ttu-id="4ae92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ae92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae92-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae92-109">Permission type</span></span>      | <span data-ttu-id="4ae92-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ae92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ae92-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ae92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ae92-112">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ae92-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ae92-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ae92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ae92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ae92-114">Not supported.</span></span>    |
|<span data-ttu-id="4ae92-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ae92-115">Application</span></span> | <span data-ttu-id="4ae92-116">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ae92-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ae92-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ae92-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="4ae92-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ae92-118">Request headers</span></span>
| <span data-ttu-id="4ae92-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4ae92-119">Name</span></span>      |<span data-ttu-id="4ae92-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae92-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ae92-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ae92-121">Authorization</span></span>  | <span data-ttu-id="4ae92-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ae92-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ae92-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ae92-124">Request body</span></span>
<span data-ttu-id="4ae92-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ae92-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ae92-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae92-126">Response</span></span>

<span data-ttu-id="4ae92-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсершисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae92-127">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae92-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4ae92-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ae92-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ae92-129">Request</span></span>
<span data-ttu-id="4ae92-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ae92-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4ae92-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ae92-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ae92-132">C#</span><span class="sxs-lookup"><span data-stu-id="4ae92-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ae92-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="4ae92-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ae92-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4ae92-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4ae92-135">Java</span><span class="sxs-lookup"><span data-stu-id="4ae92-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userriskhitsory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4ae92-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae92-136">Response</span></span>
<span data-ttu-id="4ae92-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae92-137">Here is an example of the response.</span></span>
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

