---
title: Получение riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
ms.openlocfilehash: 14a944012a8015ecf3c60f761edba680c2c7a68b
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241029"
---
# <a name="get-riskyusers"></a><span data-ttu-id="bf798-103">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="bf798-103">Get riskyUsers</span></span>

> <span data-ttu-id="bf798-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf798-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf798-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf798-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf798-106">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="bf798-106">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="bf798-107">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="bf798-107">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf798-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf798-108">Permissions</span></span>
<span data-ttu-id="bf798-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf798-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf798-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf798-111">Permission type</span></span>      | <span data-ttu-id="bf798-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf798-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf798-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf798-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bf798-114">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf798-114">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="bf798-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf798-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf798-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf798-116">Not supported.</span></span>    |
|<span data-ttu-id="bf798-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf798-117">Application</span></span> | <span data-ttu-id="bf798-118">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf798-118">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf798-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf798-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="bf798-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf798-120">Request headers</span></span>
| <span data-ttu-id="bf798-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bf798-121">Name</span></span>      |<span data-ttu-id="bf798-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bf798-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf798-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf798-123">Authorization</span></span>  | <span data-ttu-id="bf798-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf798-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf798-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf798-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf798-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf798-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf798-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf798-129">Request body</span></span>
<span data-ttu-id="bf798-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf798-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf798-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf798-131">Response</span></span>

<span data-ttu-id="bf798-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [riskyUser](../resources/riskyuser.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bf798-132">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf798-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bf798-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf798-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf798-134">Request</span></span>
<span data-ttu-id="bf798-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf798-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="bf798-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf798-136">Response</span></span>
<span data-ttu-id="bf798-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf798-137">Here is an example of the response.</span></span>
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
