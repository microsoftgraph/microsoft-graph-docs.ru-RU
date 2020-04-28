---
title: Получение Локатедрискевент
description: Получение свойств и связей объекта локатедрискевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8b43453dcfbc752bc2f11b1576e7aafa4adbec0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457085"
---
# <a name="get-locatedriskevent"></a><span data-ttu-id="7d195-103">Получение Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="7d195-103">Get locatedRiskEvent</span></span>

<span data-ttu-id="7d195-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d195-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d195-105">Получение свойств и связей объекта локатедрискевент.</span><span class="sxs-lookup"><span data-stu-id="7d195-105">Retrieve the properties and relationships of a locatedriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d195-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d195-106">Permissions</span></span>
<span data-ttu-id="7d195-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d195-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d195-109">Permission type</span></span>      | <span data-ttu-id="7d195-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d195-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d195-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d195-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d195-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d195-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="7d195-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d195-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d195-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d195-114">Not supported.</span></span>    |
|<span data-ttu-id="7d195-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d195-115">Application</span></span> | <span data-ttu-id="7d195-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d195-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d195-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d195-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /locatedRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7d195-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d195-118">Request headers</span></span>
| <span data-ttu-id="7d195-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d195-119">Name</span></span>      |<span data-ttu-id="7d195-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d195-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d195-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d195-121">Authorization</span></span>  | <span data-ttu-id="7d195-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d195-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d195-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d195-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d195-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7d195-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d195-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d195-127">Request body</span></span>
<span data-ttu-id="7d195-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d195-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d195-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d195-129">Response</span></span>

<span data-ttu-id="7d195-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [локатедрискевент](../resources/locatedriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d195-130">If successful, this method returns a `200 OK` response code and [locatedRiskEvent](../resources/locatedriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d195-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d195-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d195-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d195-132">Request</span></span>
<span data-ttu-id="7d195-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d195-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_locatedriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/locatedRiskEvents/27b91217-a6ca-edff-da2b-c46feaf0228f-a6653179-3c7b-4e99-bb4c-dddeb18adfc1-42445d4d-fe22-9840-cf9d-72f6ce8cd056
```
##### <a name="response"></a><span data-ttu-id="7d195-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d195-134">Response</span></span>
<span data-ttu-id="7d195-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d195-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
