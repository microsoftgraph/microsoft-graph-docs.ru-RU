---
title: Получение элемента журнала для Рискюсер
description: Получение элемента журнала объекта Рискюсер.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba51f6524630b6dfefc4e6106a626c7a40437963
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447706"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="85368-103">Получение Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="85368-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85368-104">Получение объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) объекта [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="85368-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="85368-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="85368-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="85368-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85368-106">Permissions</span></span>
<span data-ttu-id="85368-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85368-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85368-109">Permission type</span></span>      | <span data-ttu-id="85368-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85368-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85368-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85368-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85368-112">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85368-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="85368-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85368-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85368-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85368-114">Not supported.</span></span>    |
|<span data-ttu-id="85368-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85368-115">Application</span></span> | <span data-ttu-id="85368-116">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85368-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85368-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85368-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="85368-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85368-118">Request headers</span></span>
| <span data-ttu-id="85368-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85368-119">Name</span></span>      |<span data-ttu-id="85368-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85368-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85368-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85368-121">Authorization</span></span>  | <span data-ttu-id="85368-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85368-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85368-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85368-124">Request body</span></span>
<span data-ttu-id="85368-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85368-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85368-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="85368-126">Response</span></span>

<span data-ttu-id="85368-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85368-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85368-128">Пример</span><span class="sxs-lookup"><span data-stu-id="85368-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85368-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="85368-129">Request</span></span>
<span data-ttu-id="85368-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85368-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85368-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="85368-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="85368-132">C#</span><span class="sxs-lookup"><span data-stu-id="85368-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85368-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="85368-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85368-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="85368-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85368-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="85368-135">Response</span></span>
<span data-ttu-id="85368-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85368-136">Here is an example of the response.</span></span>
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

