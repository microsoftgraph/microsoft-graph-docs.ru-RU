---
title: Журнал списка Рискюсер
description: Получение журнала рисков
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3199528b297394ca7fc282bbf0a4346a52d185fe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791120"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="4e4a2-103">Журнал списка Рискюсер</span><span class="sxs-lookup"><span data-stu-id="4e4a2-103">List history of riskyUser</span></span>

<span data-ttu-id="4e4a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e4a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e4a2-105">Получение журнала рисков ресурса [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="4e4a2-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="4e4a2-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e4a2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4a2-107">Permissions</span></span>
<span data-ttu-id="4e4a2-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4e4a2-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e4a2-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e4a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e4a2-110">Permission type</span></span>      | <span data-ttu-id="4e4a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e4a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e4a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e4a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e4a2-113">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e4a2-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e4a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e4a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e4a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-115">Not supported.</span></span>    |
|<span data-ttu-id="4e4a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e4a2-116">Application</span></span> | <span data-ttu-id="4e4a2-117">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e4a2-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e4a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e4a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="4e4a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e4a2-119">Request headers</span></span>
| <span data-ttu-id="4e4a2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4e4a2-120">Name</span></span>      |<span data-ttu-id="4e4a2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e4a2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e4a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e4a2-122">Authorization</span></span>  | <span data-ttu-id="4e4a2-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-123">Bearer {token}.</span></span> <span data-ttu-id="4e4a2-124">Required.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e4a2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e4a2-125">Request body</span></span>
<span data-ttu-id="4e4a2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e4a2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4a2-127">Response</span></span>

<span data-ttu-id="4e4a2-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсершисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e4a2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4e4a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e4a2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e4a2-130">Request</span></span>
<span data-ttu-id="4e4a2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e4a2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e4a2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="4e4a2-133">C#</span><span class="sxs-lookup"><span data-stu-id="4e4a2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e4a2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e4a2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e4a2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e4a2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e4a2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e4a2-136">Response</span></span>
<span data-ttu-id="4e4a2-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e4a2-137">Here is an example of the response.</span></span>
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

