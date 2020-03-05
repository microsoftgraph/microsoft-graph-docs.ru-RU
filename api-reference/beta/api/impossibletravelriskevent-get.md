---
title: Получение объекта impossibleTravelRiskEvent
description: Получение свойств и связей объекта импоссиблетравелрискевент.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 5483054ce20ca5c9385e24920bff3c57f2706fb5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446420"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="bc3dc-103">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="bc3dc-103">Get impossibleTravelRiskEvent</span></span>

<span data-ttu-id="bc3dc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc3dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="bc3dc-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="bc3dc-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="bc3dc-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="bc3dc-107">Получение свойств и связей объекта импоссиблетравелрискевент.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-107">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc3dc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3dc-108">Permissions</span></span>
<span data-ttu-id="bc3dc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc3dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc3dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3dc-111">Permission type</span></span>      | <span data-ttu-id="bc3dc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc3dc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc3dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc3dc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc3dc-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc3dc-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="bc3dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc3dc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc3dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-116">Not supported.</span></span>    |
|<span data-ttu-id="bc3dc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc3dc-117">Application</span></span> | <span data-ttu-id="bc3dc-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc3dc-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc3dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc3dc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc3dc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc3dc-120">Request headers</span></span>
| <span data-ttu-id="bc3dc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bc3dc-121">Name</span></span>      |<span data-ttu-id="bc3dc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bc3dc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc3dc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc3dc-123">Authorization</span></span>  | <span data-ttu-id="bc3dc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc3dc-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc3dc-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc3dc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc3dc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc3dc-129">Request body</span></span>
<span data-ttu-id="bc3dc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc3dc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc3dc-131">Response</span></span>

<span data-ttu-id="bc3dc-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импоссиблетравелрискевент](../resources/impossibletravelriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-132">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc3dc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bc3dc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc3dc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc3dc-134">Request</span></span>
<span data-ttu-id="bc3dc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="bc3dc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc3dc-136">Response</span></span>
<span data-ttu-id="bc3dc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc3dc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
