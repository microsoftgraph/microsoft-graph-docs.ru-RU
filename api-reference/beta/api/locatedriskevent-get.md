---
title: Получение locatedRiskEvent
description: Извлечение свойств и связи объекта locatedriskevent.
ms.openlocfilehash: 9803df66f305d3750747c964c2d50485278edc05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079073"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="0ebf3-103">Получение locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0ebf3-103">Get locatedRiskEvent</span></span>

> <span data-ttu-id="0ebf3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ebf3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ebf3-106">Извлечение свойств и связи объекта locatedriskevent.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-106">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ebf3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ebf3-107">Permissions</span></span>
<span data-ttu-id="0ebf3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ebf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ebf3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ebf3-110">Permission type</span></span>      | <span data-ttu-id="0ebf3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ebf3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ebf3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ebf3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ebf3-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ebf3-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="0ebf3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ebf3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ebf3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-115">Not supported.</span></span>    |
|<span data-ttu-id="0ebf3-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0ebf3-116">Application</span></span> | <span data-ttu-id="0ebf3-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ebf3-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ebf3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ebf3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ebf3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ebf3-119">Request headers</span></span>
| <span data-ttu-id="0ebf3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ebf3-120">Name</span></span>      |<span data-ttu-id="0ebf3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0ebf3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ebf3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ebf3-122">Authorization</span></span>  | <span data-ttu-id="0ebf3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ebf3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ebf3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ebf3-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ebf3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ebf3-128">Request body</span></span>
<span data-ttu-id="0ebf3-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ebf3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ebf3-130">Response</span></span>

<span data-ttu-id="0ebf3-131">Успешно завершена, этот метод возвращает `200 OK` объект [locatedRiskEvent](../resources/locatedriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-131">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ebf3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0ebf3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ebf3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ebf3-133">Request</span></span>
<span data-ttu-id="0ebf3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ebf3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="0ebf3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ebf3-135">Response</span></span>
<span data-ttu-id="0ebf3-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0ebf3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get locatedRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
