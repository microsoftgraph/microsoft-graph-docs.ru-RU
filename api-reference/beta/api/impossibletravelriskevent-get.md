---
title: Получение impossibleTravelRiskEvent
description: Извлечение свойств и связи объекта impossibletravelriskevent.
localization_priority: Normal
ms.openlocfilehash: e5f1d7a47c261a9524225a1308531de8cd8de27c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520720"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="c5bbf-103">Получение impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c5bbf-103">Get impossibleTravelRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5bbf-104">Извлечение свойств и связи объекта impossibletravelriskevent.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-104">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5bbf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bbf-105">Permissions</span></span>
<span data-ttu-id="c5bbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5bbf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bbf-108">Permission type</span></span>      | <span data-ttu-id="c5bbf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5bbf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5bbf-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5bbf-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="c5bbf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bbf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-113">Not supported.</span></span>    |
|<span data-ttu-id="c5bbf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5bbf-114">Application</span></span> | <span data-ttu-id="c5bbf-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5bbf-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5bbf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5bbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c5bbf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5bbf-117">Request headers</span></span>
| <span data-ttu-id="c5bbf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c5bbf-118">Name</span></span>      |<span data-ttu-id="c5bbf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c5bbf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5bbf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5bbf-120">Authorization</span></span>  | <span data-ttu-id="c5bbf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5bbf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5bbf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5bbf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5bbf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5bbf-126">Request body</span></span>
<span data-ttu-id="c5bbf-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5bbf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5bbf-128">Response</span></span>

<span data-ttu-id="c5bbf-129">Успешно завершена, этот метод возвращает `200 OK` объект [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-129">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5bbf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c5bbf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5bbf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5bbf-131">Request</span></span>
<span data-ttu-id="c5bbf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5bbf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="c5bbf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5bbf-133">Response</span></span>
<span data-ttu-id="c5bbf-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c5bbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
  "ipAddress": "176.10.104.240",
  "isAtypicalLocation": true,
  "location": "Bern, CH",
  "previousIPAddress": "95.31.18.119",
  "previousLocation": "Moskva, Russia, RU",
  "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "ImpossibleTravelRiskEvent",
  "userAgent": "Firefox 42.0.0.1",
  "userDisplayName": "Jon Doe",
  "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/impossibletravelriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
