---
title: Список riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
ms.openlocfilehash: 152171ff098bb58e8cbb247ca687841e77594ead
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082798"
---
# <a name="list-riskyusers"></a><span data-ttu-id="7b630-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="7b630-103">List riskyUsers</span></span>

> <span data-ttu-id="7b630-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b630-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b630-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b630-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b630-106">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="7b630-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b630-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b630-107">Permissions</span></span>
<span data-ttu-id="7b630-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b630-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b630-110">Permission type</span></span>      | <span data-ttu-id="7b630-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b630-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b630-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b630-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b630-113">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b630-113">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="7b630-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b630-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b630-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b630-115">Not supported.</span></span>    |
|<span data-ttu-id="7b630-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7b630-116">Application</span></span> | <span data-ttu-id="7b630-117">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b630-117">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b630-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b630-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b630-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b630-119">Optional query parameters</span></span>
<span data-ttu-id="7b630-120">Этот метод поддерживает `$filter` для настройки ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="7b630-120">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="7b630-121">Пример далее в этом разделе, см.</span><span class="sxs-lookup"><span data-stu-id="7b630-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="7b630-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b630-122">Request headers</span></span>
| <span data-ttu-id="7b630-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7b630-123">Name</span></span>      |<span data-ttu-id="7b630-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7b630-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b630-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b630-125">Authorization</span></span>  | <span data-ttu-id="7b630-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b630-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b630-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7b630-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="7b630-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7b630-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b630-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b630-131">Request body</span></span>
<span data-ttu-id="7b630-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b630-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b630-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b630-133">Response</span></span>

<span data-ttu-id="7b630-134">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7b630-134">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b630-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7b630-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7b630-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7b630-136">Request 1</span></span>
<span data-ttu-id="7b630-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b630-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="7b630-138">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="7b630-138">Response 1</span></span>
<span data-ttu-id="7b630-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b630-139">Here is an example of the response.</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
##### <a name="request-2"></a><span data-ttu-id="7b630-140">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7b630-140">Request 2</span></span>
<span data-ttu-id="7b630-141">Следующий пример демонстрирует использование `$filter` для получения коллекции riskyUser которого статистические риска установлен средний уровень.</span><span class="sxs-lookup"><span data-stu-id="7b630-141">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="7b630-142">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="7b630-142">Response 2</span></span>
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
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
