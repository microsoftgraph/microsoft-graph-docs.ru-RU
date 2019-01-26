---
title: Получение identityRiskEvent
description: Извлечение свойств и связи объекта identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: e86ec77450a1b661311ba9e53b3b3591776323a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575704"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="42557-103">Получение identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="42557-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42557-104">Извлечение свойств и связи объекта identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="42557-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="42557-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42557-105">Permissions</span></span>
<span data-ttu-id="42557-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42557-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42557-108">Permission type</span></span>      | <span data-ttu-id="42557-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42557-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42557-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42557-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42557-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="42557-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="42557-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42557-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42557-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42557-113">Not supported.</span></span>    |
|<span data-ttu-id="42557-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42557-114">Application</span></span> | <span data-ttu-id="42557-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="42557-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42557-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42557-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="42557-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42557-117">Request headers</span></span>
| <span data-ttu-id="42557-118">Имя</span><span class="sxs-lookup"><span data-stu-id="42557-118">Name</span></span>      |<span data-ttu-id="42557-119">Описание</span><span class="sxs-lookup"><span data-stu-id="42557-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42557-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42557-120">Authorization</span></span>  | <span data-ttu-id="42557-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42557-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42557-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42557-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="42557-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="42557-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42557-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42557-126">Request body</span></span>
<span data-ttu-id="42557-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42557-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42557-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="42557-128">Response</span></span>

<span data-ttu-id="42557-129">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42557-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42557-130">Пример</span><span class="sxs-lookup"><span data-stu-id="42557-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42557-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42557-131">Request</span></span>
<span data-ttu-id="42557-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42557-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6
```
##### <a name="response"></a><span data-ttu-id="42557-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="42557-133">Response</span></span>
<span data-ttu-id="42557-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="42557-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
