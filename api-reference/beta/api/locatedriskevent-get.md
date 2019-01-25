---
title: Получение locatedRiskEvent
description: Извлечение свойств и связи объекта locatedriskevent.
localization_priority: Normal
ms.openlocfilehash: aee63e3f9cbb90f839d3eaebf5ec37b2f5b53042
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509233"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="2e6a4-103">Получение locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2e6a4-103">Get locatedRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e6a4-104">Извлечение свойств и связи объекта locatedriskevent.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-104">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e6a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e6a4-105">Permissions</span></span>
<span data-ttu-id="2e6a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e6a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e6a4-108">Permission type</span></span>      | <span data-ttu-id="2e6a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e6a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e6a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e6a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e6a4-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e6a4-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="2e6a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e6a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e6a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-113">Not supported.</span></span>    |
|<span data-ttu-id="2e6a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e6a4-114">Application</span></span> | <span data-ttu-id="2e6a4-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e6a4-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e6a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e6a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e6a4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e6a4-117">Request headers</span></span>
| <span data-ttu-id="2e6a4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2e6a4-118">Name</span></span>      |<span data-ttu-id="2e6a4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2e6a4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e6a4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e6a4-120">Authorization</span></span>  | <span data-ttu-id="2e6a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e6a4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2e6a4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e6a4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e6a4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e6a4-126">Request body</span></span>
<span data-ttu-id="2e6a4-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e6a4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e6a4-128">Response</span></span>

<span data-ttu-id="2e6a4-129">Успешно завершена, этот метод возвращает `200 OK` объект [locatedRiskEvent](../resources/locatedriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-129">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e6a4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2e6a4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e6a4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e6a4-131">Request</span></span>
<span data-ttu-id="2e6a4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e6a4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="2e6a4-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e6a4-133">Response</span></span>
<span data-ttu-id="2e6a4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2e6a4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.locatedRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "a6653179-3c7b-4e99-bb4c-dddeb18adfc1",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/locatedriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
