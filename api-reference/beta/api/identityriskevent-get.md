---
title: Получение identityRiskEvent
description: Извлечение свойств и связи объекта identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 54bb5a43971fd4108178a7cace6821e4369ec6a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510731"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="9a93a-103">Получение identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="9a93a-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a93a-104">Извлечение свойств и связи объекта identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="9a93a-104">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a93a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a93a-105">Permissions</span></span>
<span data-ttu-id="9a93a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a93a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a93a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a93a-108">Permission type</span></span>      | <span data-ttu-id="9a93a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a93a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a93a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a93a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a93a-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a93a-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="9a93a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a93a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a93a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a93a-113">Not supported.</span></span>    |
|<span data-ttu-id="9a93a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a93a-114">Application</span></span> | <span data-ttu-id="9a93a-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a93a-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a93a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a93a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9a93a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a93a-117">Request headers</span></span>
| <span data-ttu-id="9a93a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9a93a-118">Name</span></span>      |<span data-ttu-id="9a93a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9a93a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a93a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a93a-120">Authorization</span></span>  | <span data-ttu-id="9a93a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a93a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a93a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a93a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a93a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9a93a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a93a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a93a-126">Request body</span></span>
<span data-ttu-id="9a93a-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a93a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a93a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a93a-128">Response</span></span>

<span data-ttu-id="9a93a-129">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9a93a-129">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a93a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9a93a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a93a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a93a-131">Request</span></span>
<span data-ttu-id="9a93a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a93a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="9a93a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a93a-133">Response</span></span>
<span data-ttu-id="9a93a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9a93a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
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
