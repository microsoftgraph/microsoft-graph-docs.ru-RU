---
title: Получение объекта unfamiliarLocationRiskEvent
description: Получение свойств и связей объекта унфамилиарлокатионрискевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 454dc4fe6ae232cf926dd0c6dc4116e9650362b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095613"
---
# <a name="get-unfamiliarlocationriskevent-deprecated"></a><span data-ttu-id="0b464-103">Получение Унфамилиарлокатионрискевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="0b464-103">Get unfamiliarLocationRiskEvent (deprecated)</span></span>

<span data-ttu-id="0b464-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b464-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="0b464-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="0b464-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="0b464-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="0b464-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="0b464-107">Получение свойств и связей объекта унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="0b464-107">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b464-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b464-108">Permissions</span></span>
<span data-ttu-id="0b464-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b464-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b464-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b464-111">Permission type</span></span>      | <span data-ttu-id="0b464-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b464-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b464-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b464-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0b464-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b464-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="0b464-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b464-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b464-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b464-116">Not supported.</span></span>    |
|<span data-ttu-id="0b464-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b464-117">Application</span></span> | <span data-ttu-id="0b464-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b464-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b464-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b464-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0b464-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b464-120">Request headers</span></span>
| <span data-ttu-id="0b464-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0b464-121">Name</span></span>      |<span data-ttu-id="0b464-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0b464-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b464-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b464-123">Authorization</span></span>  | <span data-ttu-id="0b464-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b464-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b464-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b464-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b464-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0b464-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b464-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b464-129">Request body</span></span>
<span data-ttu-id="0b464-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b464-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b464-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b464-131">Response</span></span>

<span data-ttu-id="0b464-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унфамилиарлокатионрискевент](../resources/unfamiliarlocationriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b464-132">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b464-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0b464-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b464-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b464-134">Request</span></span>
<span data-ttu-id="0b464-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b464-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="0b464-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b464-136">Response</span></span>
<span data-ttu-id="0b464-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b464-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


