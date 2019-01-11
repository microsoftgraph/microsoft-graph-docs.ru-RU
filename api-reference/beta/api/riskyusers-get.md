---
title: Получение riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
localization_priority: Normal
ms.openlocfilehash: da26be10b5a1aa631bd55f977ead806ed89c1406
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891128"
---
# <a name="get-riskyusers"></a><span data-ttu-id="562a3-103">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="562a3-103">Get riskyUsers</span></span>

> <span data-ttu-id="562a3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="562a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="562a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="562a3-106">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="562a3-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="562a3-107">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="562a3-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="562a3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="562a3-108">Permissions</span></span>
<span data-ttu-id="562a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="562a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562a3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="562a3-111">Permission type</span></span>      | <span data-ttu-id="562a3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="562a3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="562a3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="562a3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="562a3-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="562a3-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="562a3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="562a3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="562a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562a3-116">Not supported.</span></span>    |
|<span data-ttu-id="562a3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="562a3-117">Application</span></span> | <span data-ttu-id="562a3-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="562a3-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="562a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="562a3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="562a3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="562a3-120">Request headers</span></span>
| <span data-ttu-id="562a3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="562a3-121">Name</span></span>      |<span data-ttu-id="562a3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="562a3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="562a3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="562a3-123">Authorization</span></span>  | <span data-ttu-id="562a3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="562a3-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="562a3-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="562a3-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="562a3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="562a3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="562a3-129">Request body</span></span>
<span data-ttu-id="562a3-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="562a3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="562a3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="562a3-131">Response</span></span>

<span data-ttu-id="562a3-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [riskyUser](../resources/riskyuser.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="562a3-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="562a3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="562a3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="562a3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="562a3-134">Request</span></span>
<span data-ttu-id="562a3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562a3-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="562a3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="562a3-136">Response</span></span>
<span data-ttu-id="562a3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="562a3-137">Here is an example of the response.</span></span>
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
