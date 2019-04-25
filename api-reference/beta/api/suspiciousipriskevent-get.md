---
title: Получение объекта suspiciousIpRiskEvent
description: Получение свойств и связей объекта суспиЦиаусиприскевент.
localization_priority: Normal
ms.openlocfilehash: 64218e000eb32065a65d68d69e3735caa11b3ca0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545379"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="ee30b-103">Получение объекта suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ee30b-103">Get suspiciousIpRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee30b-104">Получение свойств и связей объекта суспиЦиаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="ee30b-104">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee30b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee30b-105">Permissions</span></span>
<span data-ttu-id="ee30b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee30b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee30b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee30b-108">Permission type</span></span>      | <span data-ttu-id="ee30b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee30b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee30b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee30b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee30b-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee30b-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="ee30b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee30b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee30b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee30b-113">Not supported.</span></span>    |
|<span data-ttu-id="ee30b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee30b-114">Application</span></span> | <span data-ttu-id="ee30b-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee30b-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee30b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee30b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ee30b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee30b-117">Request headers</span></span>
| <span data-ttu-id="ee30b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ee30b-118">Name</span></span>      |<span data-ttu-id="ee30b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ee30b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee30b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee30b-120">Authorization</span></span>  | <span data-ttu-id="ee30b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee30b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee30b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee30b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee30b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee30b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee30b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee30b-126">Request body</span></span>
<span data-ttu-id="ee30b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee30b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee30b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee30b-128">Response</span></span>

<span data-ttu-id="ee30b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [суспиЦиаусиприскевент](../resources/suspiciousipriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee30b-129">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee30b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ee30b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee30b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee30b-131">Request</span></span>
<span data-ttu-id="ee30b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee30b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="ee30b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee30b-133">Response</span></span>
<span data-ttu-id="ee30b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee30b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": null,
  "createdDateTime": "2016-02-03T06:08:35.123512Z",
  "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
  "ipAddress": "95.31.18.119",
  "location": "Moskva, Russia, RU",
  "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
  "riskEventStatus": "active",
  "riskLevel": "low",
  "riskType": "SuspiciousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/suspiciousipriskevent-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
