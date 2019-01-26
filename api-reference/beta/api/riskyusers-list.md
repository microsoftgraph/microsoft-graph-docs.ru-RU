---
title: Список riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 0987a45aafdb31cad17728851ce1ac1ddb066aa0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576376"
---
# <a name="list-riskyusers"></a><span data-ttu-id="cb3d7-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="cb3d7-103">List riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb3d7-104">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="cb3d7-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="cb3d7-105">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb3d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3d7-106">Permissions</span></span>
<span data-ttu-id="cb3d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3d7-109">Permission type</span></span>      | <span data-ttu-id="cb3d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb3d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb3d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb3d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cb3d7-112">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb3d7-112">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="cb3d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb3d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb3d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-114">Not supported.</span></span>    |
|<span data-ttu-id="cb3d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb3d7-115">Application</span></span> | <span data-ttu-id="cb3d7-116">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb3d7-116">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb3d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb3d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb3d7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb3d7-118">Optional query parameters</span></span>
<span data-ttu-id="cb3d7-119">Этот метод поддерживает `$filter` для настройки ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-119">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="cb3d7-120">Пример далее в этом разделе, см.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="cb3d7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb3d7-121">Request headers</span></span>
| <span data-ttu-id="cb3d7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cb3d7-122">Name</span></span>      |<span data-ttu-id="cb3d7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cb3d7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb3d7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb3d7-124">Authorization</span></span>  | <span data-ttu-id="cb3d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb3d7-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cb3d7-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="cb3d7-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3d7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb3d7-130">Request body</span></span>
<span data-ttu-id="cb3d7-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3d7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb3d7-132">Response</span></span>

<span data-ttu-id="cb3d7-133">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-133">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cb3d7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cb3d7-134">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="cb3d7-135">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="cb3d7-135">Request 1</span></span>
<span data-ttu-id="cb3d7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="cb3d7-137">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="cb3d7-137">Response 1</span></span>
<span data-ttu-id="cb3d7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-138">Here is an example of the response.</span></span>
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
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Jon Doe",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="cb3d7-139">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="cb3d7-139">Request 2</span></span>
<span data-ttu-id="cb3d7-140">Следующий пример демонстрирует использование `$filter` для получения коллекции riskyUser которого статистические риска установлен средний уровень.</span><span class="sxs-lookup"><span data-stu-id="cb3d7-140">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="cb3d7-141">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="cb3d7-141">Response 2</span></span>
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
      "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
      "isGuest": false,
      "isDeleted": false,
      "riskDetail": "none",
      "riskLevel": "medium",
      "riskState": "atRisk",
      "userDisplayName": "Jon Doe",
      "userPrincipalName": "jon@contoso.com"
      
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
