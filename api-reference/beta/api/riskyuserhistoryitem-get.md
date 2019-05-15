---
title: Получение элемента журнала для Рискюсер
description: Получение элемента журнала объекта Рискюсер.
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b185444057349700978786f235249f6222ebfbb9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960923"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="1b6a8-103">Получение Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="1b6a8-103">Get riskyUserHistoryItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b6a8-104">Получение объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) объекта [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="1b6a8-104">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="1b6a8-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b6a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b6a8-106">Permissions</span></span>
<span data-ttu-id="1b6a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b6a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b6a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b6a8-109">Permission type</span></span>      | <span data-ttu-id="1b6a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b6a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b6a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b6a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b6a8-112">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1b6a8-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b6a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b6a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b6a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-114">Not supported.</span></span>    |
|<span data-ttu-id="1b6a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b6a8-115">Application</span></span> | <span data-ttu-id="1b6a8-116">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1b6a8-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b6a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b6a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="1b6a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b6a8-118">Request headers</span></span>
| <span data-ttu-id="1b6a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1b6a8-119">Name</span></span>      |<span data-ttu-id="1b6a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6a8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b6a8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b6a8-121">Authorization</span></span>  | <span data-ttu-id="1b6a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b6a8-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b6a8-124">Request body</span></span>
<span data-ttu-id="1b6a8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b6a8-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b6a8-126">Response</span></span>

<span data-ttu-id="1b6a8-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-127">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b6a8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1b6a8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b6a8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b6a8-129">Request</span></span>
<span data-ttu-id="1b6a8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
##### <a name="response"></a><span data-ttu-id="1b6a8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b6a8-131">Response</span></span>
<span data-ttu-id="1b6a8-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b6a8-132">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1b6a8-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1b6a8-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1b6a8-134">C#</span><span class="sxs-lookup"><span data-stu-id="1b6a8-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b6a8-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b6a8-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser_historyitem-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyuserhistoryitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

