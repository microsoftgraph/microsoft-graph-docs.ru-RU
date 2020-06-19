---
title: Получение Рискюсер
description: Получение свойств и связей объекта **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: edbbfc520ac40ca5532f6d44c503c61dab808e5a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791113"
---
# <a name="get-riskyuser"></a><span data-ttu-id="66c86-103">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="66c86-103">Get riskyUser</span></span>

<span data-ttu-id="66c86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66c86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66c86-105">Получение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="66c86-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="66c86-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="66c86-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="66c86-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66c86-107">Permissions</span></span>
<span data-ttu-id="66c86-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="66c86-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="66c86-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66c86-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66c86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66c86-110">Permission type</span></span>      | <span data-ttu-id="66c86-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66c86-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66c86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66c86-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66c86-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="66c86-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="66c86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66c86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66c86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66c86-115">Not supported.</span></span>    |
|<span data-ttu-id="66c86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66c86-116">Application</span></span> | <span data-ttu-id="66c86-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="66c86-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66c86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66c86-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="66c86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66c86-119">Request headers</span></span>
| <span data-ttu-id="66c86-120">Имя</span><span class="sxs-lookup"><span data-stu-id="66c86-120">Name</span></span>      |<span data-ttu-id="66c86-121">Описание</span><span class="sxs-lookup"><span data-stu-id="66c86-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66c86-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66c86-122">Authorization</span></span>  | <span data-ttu-id="66c86-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="66c86-123">Bearer {token}.</span></span> <span data-ttu-id="66c86-124">Required.</span><span class="sxs-lookup"><span data-stu-id="66c86-124">Required.</span></span> |
| <span data-ttu-id="66c86-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66c86-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="66c86-126">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="66c86-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="66c86-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="66c86-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66c86-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66c86-128">Request body</span></span>
<span data-ttu-id="66c86-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66c86-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66c86-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="66c86-130">Response</span></span>

<span data-ttu-id="66c86-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66c86-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66c86-132">Пример</span><span class="sxs-lookup"><span data-stu-id="66c86-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66c86-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="66c86-133">Request</span></span>
<span data-ttu-id="66c86-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66c86-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66c86-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="66c86-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="66c86-136">C#</span><span class="sxs-lookup"><span data-stu-id="66c86-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66c86-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66c86-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66c86-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66c86-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66c86-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="66c86-139">Response</span></span>
<span data-ttu-id="66c86-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66c86-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

