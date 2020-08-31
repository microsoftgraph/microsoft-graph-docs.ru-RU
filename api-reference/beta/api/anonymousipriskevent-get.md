---
title: Получение объекта anonymousIpRiskEvent
description: Получение свойств и связей объекта анонимаусиприскевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: c4c514e1b838c8146841b3eb1c42988d9e709f9f
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311488"
---
# <a name="get-anonymousipriskevent-deprecated"></a><span data-ttu-id="8bd11-103">Получение Анонимаусиприскевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="8bd11-103">Get anonymousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="8bd11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bd11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="8bd11-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="8bd11-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="8bd11-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="8bd11-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="8bd11-107">Получение свойств и связей объекта анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="8bd11-107">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8bd11-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bd11-108">Permissions</span></span>
<span data-ttu-id="8bd11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bd11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bd11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bd11-111">Permission type</span></span>      | <span data-ttu-id="8bd11-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bd11-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bd11-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bd11-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8bd11-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bd11-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="8bd11-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bd11-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bd11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bd11-116">Not supported.</span></span>    |
|<span data-ttu-id="8bd11-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bd11-117">Application</span></span> | <span data-ttu-id="8bd11-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bd11-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bd11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bd11-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bd11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bd11-120">Request headers</span></span>
| <span data-ttu-id="8bd11-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8bd11-121">Name</span></span>      |<span data-ttu-id="8bd11-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8bd11-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bd11-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bd11-123">Authorization</span></span>  | <span data-ttu-id="8bd11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bd11-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bd11-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8bd11-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="8bd11-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8bd11-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bd11-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bd11-129">Request body</span></span>
<span data-ttu-id="8bd11-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bd11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bd11-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bd11-131">Response</span></span>

<span data-ttu-id="8bd11-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [анонимаусиприскевент](../resources/anonymousipriskevent.md) в значении тела отклика.</span><span class="sxs-lookup"><span data-stu-id="8bd11-132">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="8bd11-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8bd11-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bd11-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bd11-134">Request</span></span>
<span data-ttu-id="8bd11-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bd11-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="8bd11-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bd11-136">Response</span></span>
<span data-ttu-id="8bd11-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bd11-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
