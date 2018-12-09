---
title: Получение riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
ms.openlocfilehash: 7212e99e53d990df9cd9fea7dae754a693edc745
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209686"
---
# <a name="get-riskyusers"></a><span data-ttu-id="bc916-103">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="bc916-103">Get riskyUsers</span></span>

> <span data-ttu-id="bc916-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc916-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc916-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc916-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc916-106">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="bc916-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc916-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc916-107">Permissions</span></span>
<span data-ttu-id="bc916-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc916-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc916-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc916-110">Permission type</span></span>      | <span data-ttu-id="bc916-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc916-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc916-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc916-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc916-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc916-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="bc916-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc916-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc916-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc916-115">Not supported.</span></span>    |
|<span data-ttu-id="bc916-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc916-116">Application</span></span> | <span data-ttu-id="bc916-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc916-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc916-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc916-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="bc916-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc916-119">Request headers</span></span>
| <span data-ttu-id="bc916-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bc916-120">Name</span></span>      |<span data-ttu-id="bc916-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bc916-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc916-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc916-122">Authorization</span></span>  | <span data-ttu-id="bc916-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc916-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc916-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc916-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc916-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bc916-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc916-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc916-128">Request body</span></span>
<span data-ttu-id="bc916-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc916-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc916-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc916-130">Response</span></span>

<span data-ttu-id="bc916-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [riskyUser](../resources/riskyuser.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc916-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc916-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bc916-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc916-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc916-133">Request</span></span>
<span data-ttu-id="bc916-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc916-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="bc916-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc916-135">Response</span></span>
<span data-ttu-id="bc916-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc916-136">Here is an example of the response.</span></span>
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
