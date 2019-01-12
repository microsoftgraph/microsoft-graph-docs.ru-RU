---
title: Список riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: f2763a963d27bbb0a2fc1515a36aec199bd29f19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953443"
---
# <a name="list-riskyusers"></a><span data-ttu-id="2b424-103">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="2b424-103">List riskyUsers</span></span>

> <span data-ttu-id="2b424-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b424-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b424-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b424-106">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="2b424-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="2b424-107">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="2b424-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b424-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b424-108">Permissions</span></span>
<span data-ttu-id="2b424-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b424-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b424-111">Permission type</span></span>      | <span data-ttu-id="2b424-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b424-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b424-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b424-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2b424-114">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b424-114">IdentityriskyUser.Read.All</span></span>    |
|<span data-ttu-id="2b424-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b424-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b424-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b424-116">Not supported.</span></span>    |
|<span data-ttu-id="2b424-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b424-117">Application</span></span> | <span data-ttu-id="2b424-118">IdentityriskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b424-118">IdentityriskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b424-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b424-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b424-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b424-120">Optional query parameters</span></span>
<span data-ttu-id="2b424-121">Этот метод поддерживает `$filter` для настройки ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="2b424-121">This method supports `$filter` to customize the query response.</span></span> <span data-ttu-id="2b424-122">Пример далее в этом разделе, см.</span><span class="sxs-lookup"><span data-stu-id="2b424-122">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="2b424-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b424-123">Request headers</span></span>
| <span data-ttu-id="2b424-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2b424-124">Name</span></span>      |<span data-ttu-id="2b424-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2b424-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b424-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b424-126">Authorization</span></span>  | <span data-ttu-id="2b424-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b424-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b424-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b424-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b424-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2b424-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b424-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b424-132">Request body</span></span>
<span data-ttu-id="2b424-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b424-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b424-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b424-134">Response</span></span>

<span data-ttu-id="2b424-135">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b424-135">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b424-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2b424-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="2b424-137">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="2b424-137">Request 1</span></span>
<span data-ttu-id="2b424-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b424-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers
```
##### <a name="response-1"></a><span data-ttu-id="2b424-139">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="2b424-139">Response 1</span></span>
<span data-ttu-id="2b424-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b424-140">Here is an example of the response.</span></span>
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
##### <a name="request-2"></a><span data-ttu-id="2b424-141">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="2b424-141">Request 2</span></span>
<span data-ttu-id="2b424-142">Следующий пример демонстрирует использование `$filter` для получения коллекции riskyUser которого статистические риска установлен средний уровень.</span><span class="sxs-lookup"><span data-stu-id="2b424-142">The following example shows how to use `$filter` to get the collection of riskyUser whose aggregate risk level is Medium.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
##### <a name="response-2"></a><span data-ttu-id="2b424-143">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="2b424-143">Response 2</span></span>
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
