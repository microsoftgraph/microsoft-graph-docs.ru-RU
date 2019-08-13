---
title: Получение Рискюсер
description: Получение свойств и связей объекта **рискюсер** .
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db46cd2218aea8cae5c8638bc1b2a426d42359bf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358197"
---
# <a name="get-riskyuser"></a><span data-ttu-id="ebda5-103">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="ebda5-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebda5-104">Получение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="ebda5-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="ebda5-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="ebda5-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebda5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebda5-106">Permissions</span></span>
<span data-ttu-id="ebda5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebda5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebda5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebda5-109">Permission type</span></span>      | <span data-ttu-id="ebda5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebda5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebda5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebda5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebda5-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebda5-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="ebda5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebda5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebda5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebda5-114">Not supported.</span></span>    |
|<span data-ttu-id="ebda5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebda5-115">Application</span></span> | <span data-ttu-id="ebda5-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebda5-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebda5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebda5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="ebda5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebda5-118">Request headers</span></span>
| <span data-ttu-id="ebda5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ebda5-119">Name</span></span>      |<span data-ttu-id="ebda5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ebda5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ebda5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebda5-121">Authorization</span></span>  | <span data-ttu-id="ebda5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebda5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebda5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebda5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebda5-125">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="ebda5-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="ebda5-126">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ebda5-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebda5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebda5-127">Request body</span></span>
<span data-ttu-id="ebda5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebda5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebda5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebda5-129">Response</span></span>

<span data-ttu-id="ebda5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebda5-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebda5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ebda5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebda5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebda5-132">Request</span></span>
<span data-ttu-id="ebda5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebda5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ebda5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebda5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ebda5-135">C#</span><span class="sxs-lookup"><span data-stu-id="ebda5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebda5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebda5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ebda5-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ebda5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ebda5-138">Java</span><span class="sxs-lookup"><span data-stu-id="ebda5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebda5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebda5-139">Response</span></span>
<span data-ttu-id="ebda5-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebda5-140">Here is an example of the response.</span></span>
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
  "isGuest": true,
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

