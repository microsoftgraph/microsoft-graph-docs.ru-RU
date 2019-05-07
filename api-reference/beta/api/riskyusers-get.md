---
title: Получение Рискюсер
description: Получение свойств и связей объекта **рискюсер** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82eb470bf977321def10b66c0ec8199a3bec07a5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639027"
---
# <a name="get-riskyuser"></a><span data-ttu-id="44042-103">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="44042-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44042-104">Получение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="44042-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="44042-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="44042-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="44042-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44042-106">Permissions</span></span>
<span data-ttu-id="44042-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44042-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44042-109">Permission type</span></span>      | <span data-ttu-id="44042-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44042-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44042-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44042-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44042-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="44042-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="44042-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44042-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44042-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44042-114">Not supported.</span></span>    |
|<span data-ttu-id="44042-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44042-115">Application</span></span> | <span data-ttu-id="44042-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="44042-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44042-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44042-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="44042-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44042-118">Request headers</span></span>
| <span data-ttu-id="44042-119">Имя</span><span class="sxs-lookup"><span data-stu-id="44042-119">Name</span></span>      |<span data-ttu-id="44042-120">Описание</span><span class="sxs-lookup"><span data-stu-id="44042-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44042-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44042-121">Authorization</span></span>  | <span data-ttu-id="44042-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44042-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44042-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44042-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="44042-125">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="44042-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="44042-126">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="44042-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44042-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44042-127">Request body</span></span>
<span data-ttu-id="44042-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44042-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44042-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="44042-129">Response</span></span>

<span data-ttu-id="44042-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсер](../resources/riskyUser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44042-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44042-131">Пример</span><span class="sxs-lookup"><span data-stu-id="44042-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44042-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="44042-132">Request</span></span>
<span data-ttu-id="44042-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44042-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a><span data-ttu-id="44042-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="44042-134">Response</span></span>
<span data-ttu-id="44042-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44042-135">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="44042-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="44042-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="44042-137">Языках</span><span class="sxs-lookup"><span data-stu-id="44042-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44042-138">Язык</span><span class="sxs-lookup"><span data-stu-id="44042-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

