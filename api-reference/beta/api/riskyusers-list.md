---
title: Список riskyUsers
description: Получение свойств и связей объекта **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a902daf00f80470e1ac9a83a287eac507d55e171
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003729"
---
# <a name="list-riskyusers"></a><span data-ttu-id="9fcff-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="9fcff-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fcff-104">Получение свойств и связей объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="9fcff-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

><span data-ttu-id="9fcff-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="9fcff-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fcff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fcff-106">Permissions</span></span>
<span data-ttu-id="9fcff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fcff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fcff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fcff-109">Permission type</span></span>      | <span data-ttu-id="9fcff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fcff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fcff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fcff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9fcff-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fcff-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="9fcff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fcff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fcff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fcff-114">Not supported.</span></span>    |
|<span data-ttu-id="9fcff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fcff-115">Application</span></span> | <span data-ttu-id="9fcff-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fcff-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fcff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fcff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9fcff-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9fcff-118">Optional query parameters</span></span>
<span data-ttu-id="9fcff-119">Этот метод поддерживает `$filter` настройку ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="9fcff-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="9fcff-120">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="9fcff-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="9fcff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fcff-121">Request headers</span></span>
| <span data-ttu-id="9fcff-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9fcff-122">Name</span></span>      |<span data-ttu-id="9fcff-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9fcff-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9fcff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fcff-124">Authorization</span></span>  | <span data-ttu-id="9fcff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fcff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fcff-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9fcff-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="9fcff-128">Идентификатор сеанса книги, который определяет, сохраняются ли изменения.</span><span class="sxs-lookup"><span data-stu-id="9fcff-128">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="9fcff-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9fcff-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fcff-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fcff-130">Request body</span></span>
<span data-ttu-id="9fcff-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fcff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fcff-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fcff-132">Response</span></span>

<span data-ttu-id="9fcff-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [идентитирискевент](../resources/identityriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fcff-133">If successful, this method returns a `200 OK` response code and an [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9fcff-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9fcff-134">Examples</span></span>
#### <a name="example-1-list-risky-users"></a><span data-ttu-id="9fcff-135">Пример 1: список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="9fcff-135">Example 1: List risky users</span></span>
<span data-ttu-id="9fcff-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fcff-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```

<span data-ttu-id="9fcff-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fcff-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": "true",
  "isProcessing": true,
  "isDeleted": "true",
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk"
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
#### <a name="example-2-list-risky-users-and-filter-the-results"></a><span data-ttu-id="9fcff-138">Пример 2: список рискованных пользователей и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="9fcff-138">Example 2: List risky users and filter the results</span></span>
<span data-ttu-id="9fcff-139">В приведенном ниже примере показано, `$filter` как получить коллекцию рискюсер с уровнем агрегированного риска среднего размера.</span><span class="sxs-lookup"><span data-stu-id="9fcff-139">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
<span data-ttu-id="9fcff-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fcff-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 200 OK
{
      "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isProcessing": true,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com",
      }
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
