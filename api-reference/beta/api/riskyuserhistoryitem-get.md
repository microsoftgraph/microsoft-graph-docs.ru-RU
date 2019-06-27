---
title: Получение элемента журнала для Рискюсер
description: Получение элемента журнала объекта Рискюсер.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37ab3b0598ce54bec38fbd3feb719b1b0b2047bf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265004"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="fa238-103">Получение Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="fa238-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa238-104">Получение объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) объекта [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="fa238-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="fa238-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="fa238-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa238-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa238-106">Permissions</span></span>
<span data-ttu-id="fa238-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa238-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa238-109">Permission type</span></span>      | <span data-ttu-id="fa238-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa238-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa238-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa238-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa238-112">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa238-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa238-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa238-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa238-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa238-114">Not supported.</span></span>    |
|<span data-ttu-id="fa238-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa238-115">Application</span></span> | <span data-ttu-id="fa238-116">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa238-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa238-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa238-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="fa238-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa238-118">Request headers</span></span>
| <span data-ttu-id="fa238-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fa238-119">Name</span></span>      |<span data-ttu-id="fa238-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa238-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa238-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa238-121">Authorization</span></span>  | <span data-ttu-id="fa238-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa238-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa238-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa238-124">Request body</span></span>
<span data-ttu-id="fa238-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa238-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa238-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa238-126">Response</span></span>

<span data-ttu-id="fa238-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa238-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa238-128">Пример</span><span class="sxs-lookup"><span data-stu-id="fa238-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa238-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa238-129">Request</span></span>
<span data-ttu-id="fa238-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa238-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
##### <a name="response"></a><span data-ttu-id="fa238-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa238-131">Response</span></span>
<span data-ttu-id="fa238-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa238-132">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa238-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fa238-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fa238-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa238-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa238-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa238-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fa238-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa238-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

