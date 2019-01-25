---
title: Получение anonymousIpRiskEvent
description: Извлечение свойств и связи объекта anonymousipriskevent.
localization_priority: Normal
ms.openlocfilehash: c306593d55792035377d18ad1888f5a4ca707aa6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519117"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="e17b5-103">Получение anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e17b5-103">Get anonymousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e17b5-104">Извлечение свойств и связи объекта anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="e17b5-104">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e17b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e17b5-105">Permissions</span></span>
<span data-ttu-id="e17b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e17b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e17b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e17b5-108">Permission type</span></span>      | <span data-ttu-id="e17b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e17b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e17b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e17b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e17b5-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e17b5-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e17b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e17b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e17b5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e17b5-113">Not supported.</span></span>    |
|<span data-ttu-id="e17b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e17b5-114">Application</span></span> | <span data-ttu-id="e17b5-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e17b5-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e17b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e17b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e17b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e17b5-117">Request headers</span></span>
| <span data-ttu-id="e17b5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e17b5-118">Name</span></span>      |<span data-ttu-id="e17b5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e17b5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e17b5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e17b5-120">Authorization</span></span>  | <span data-ttu-id="e17b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e17b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e17b5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e17b5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e17b5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e17b5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e17b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e17b5-126">Request body</span></span>
<span data-ttu-id="e17b5-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e17b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e17b5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e17b5-128">Response</span></span>

<span data-ttu-id="e17b5-129">Успешно завершена, этот метод возвращает `200 OK` объект [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) и кода ответа в значении тело ответа.</span><span class="sxs-lookup"><span data-stu-id="e17b5-129">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="e17b5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e17b5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e17b5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e17b5-131">Request</span></span>
<span data-ttu-id="e17b5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e17b5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="e17b5-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e17b5-133">Response</span></span>
<span data-ttu-id="e17b5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e17b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/anonymousipriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
