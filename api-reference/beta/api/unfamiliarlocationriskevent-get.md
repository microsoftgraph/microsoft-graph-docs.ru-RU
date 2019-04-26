---
title: Получение объекта unfamiliarLocationRiskEvent
description: Получение свойств и связей объекта унфамилиарлокатионрискевент.
localization_priority: Normal
ms.openlocfilehash: 1a4e65873ba94c2c2c6eb32f59183caeab327de6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329915"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="2b446-103">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2b446-103">Get unfamiliarLocationRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b446-104">Получение свойств и связей объекта унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="2b446-104">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b446-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b446-105">Permissions</span></span>
<span data-ttu-id="2b446-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b446-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b446-108">Permission type</span></span>      | <span data-ttu-id="2b446-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b446-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b446-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b446-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b446-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b446-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="2b446-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b446-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b446-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b446-113">Not supported.</span></span>    |
|<span data-ttu-id="2b446-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b446-114">Application</span></span> | <span data-ttu-id="2b446-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b446-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b446-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b446-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2b446-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b446-117">Request headers</span></span>
| <span data-ttu-id="2b446-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2b446-118">Name</span></span>      |<span data-ttu-id="2b446-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2b446-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b446-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b446-120">Authorization</span></span>  | <span data-ttu-id="2b446-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b446-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b446-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b446-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b446-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2b446-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b446-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b446-126">Request body</span></span>
<span data-ttu-id="2b446-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b446-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b446-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b446-128">Response</span></span>

<span data-ttu-id="2b446-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унфамилиарлокатионрискевент](../resources/unfamiliarlocationriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b446-129">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b446-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2b446-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b446-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b446-131">Request</span></span>
<span data-ttu-id="2b446-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b446-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="2b446-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b446-133">Response</span></span>
<span data-ttu-id="2b446-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b446-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
