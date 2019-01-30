---
title: Получение riskyUsers
description: Извлечение свойств и связи объекта **riskyUsers** .
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 586e76cd57e720741c6a63bc00374cd0973a1cf3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642347"
---
# <a name="get-riskyusers"></a><span data-ttu-id="688f5-103">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="688f5-103">Get riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688f5-104">Извлечение свойств и связи объекта **riskyUsers** .</span><span class="sxs-lookup"><span data-stu-id="688f5-104">Retrieve the properties and relationships of a **riskyUsers** object.</span></span>

> <span data-ttu-id="688f5-105">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="688f5-105">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="688f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="688f5-106">Permissions</span></span>
<span data-ttu-id="688f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="688f5-109">Permission type</span></span>      | <span data-ttu-id="688f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="688f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="688f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="688f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="688f5-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="688f5-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="688f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="688f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="688f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="688f5-114">Not supported.</span></span>    |
|<span data-ttu-id="688f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="688f5-115">Application</span></span> | <span data-ttu-id="688f5-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="688f5-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="688f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="688f5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{query}
```


## <a name="request-headers"></a><span data-ttu-id="688f5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="688f5-118">Request headers</span></span>
| <span data-ttu-id="688f5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="688f5-119">Name</span></span>      |<span data-ttu-id="688f5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="688f5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="688f5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="688f5-121">Authorization</span></span>  | <span data-ttu-id="688f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="688f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="688f5-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="688f5-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="688f5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="688f5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="688f5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="688f5-127">Request body</span></span>
<span data-ttu-id="688f5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="688f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="688f5-129">Response</span></span>

<span data-ttu-id="688f5-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [riskyUser](../resources/riskyuser.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="688f5-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="688f5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="688f5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="688f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="688f5-132">Request</span></span>
<span data-ttu-id="688f5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="688f5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/{id}
```
##### <a name="response"></a><span data-ttu-id="688f5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="688f5-134">Response</span></span>
<span data-ttu-id="688f5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="688f5-135">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
