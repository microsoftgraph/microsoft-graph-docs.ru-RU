---
title: Получение элемента журнала для Рискюсер
description: Получение элемента журнала объекта Рискюсер.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14f721710acf2171a39b0f1d5d5fc9d935982b4d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871080"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="0ef32-103">Получение Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="0ef32-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ef32-104">Получение объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) объекта [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="0ef32-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="0ef32-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="0ef32-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ef32-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ef32-106">Permissions</span></span>
<span data-ttu-id="0ef32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ef32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ef32-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ef32-109">Permission type</span></span>      | <span data-ttu-id="0ef32-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ef32-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ef32-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ef32-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ef32-112">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ef32-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ef32-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ef32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ef32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ef32-114">Not supported.</span></span>    |
|<span data-ttu-id="0ef32-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ef32-115">Application</span></span> | <span data-ttu-id="0ef32-116">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ef32-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ef32-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ef32-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="0ef32-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ef32-118">Request headers</span></span>
| <span data-ttu-id="0ef32-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ef32-119">Name</span></span>      |<span data-ttu-id="0ef32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ef32-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ef32-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ef32-121">Authorization</span></span>  | <span data-ttu-id="0ef32-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ef32-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ef32-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ef32-124">Request body</span></span>
<span data-ttu-id="0ef32-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ef32-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ef32-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ef32-126">Response</span></span>

<span data-ttu-id="0ef32-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ef32-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ef32-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0ef32-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ef32-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ef32-129">Request</span></span>
<span data-ttu-id="0ef32-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ef32-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ef32-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ef32-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ef32-132">C#</span><span class="sxs-lookup"><span data-stu-id="0ef32-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ef32-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ef32-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ef32-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ef32-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ef32-135">Java</span><span class="sxs-lookup"><span data-stu-id="0ef32-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-historyitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ef32-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ef32-136">Response</span></span>
<span data-ttu-id="0ef32-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ef32-137">Here is an example of the response.</span></span>
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

