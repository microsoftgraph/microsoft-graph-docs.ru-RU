---
title: Получение объекта suspiciousIpRiskEvent
description: Получение свойств и связей объекта суспиЦиаусиприскевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 456b038b9aaa71280ee00df336d3e12b6cd4c133
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312007"
---
# <a name="get-suspiciousipriskevent-deprecated"></a><span data-ttu-id="aec35-103">Получение СуспиЦиаусиприскевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="aec35-103">Get suspiciousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="aec35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="aec35-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="aec35-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="aec35-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="aec35-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="aec35-107">Получение свойств и связей объекта суспиЦиаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="aec35-107">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aec35-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aec35-108">Permissions</span></span>
<span data-ttu-id="aec35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aec35-111">Permission type</span></span>      | <span data-ttu-id="aec35-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aec35-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aec35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aec35-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aec35-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec35-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="aec35-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aec35-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aec35-116">Not supported.</span></span>    |
|<span data-ttu-id="aec35-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aec35-117">Application</span></span> | <span data-ttu-id="aec35-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="aec35-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aec35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aec35-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="aec35-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aec35-120">Request headers</span></span>
| <span data-ttu-id="aec35-121">Имя</span><span class="sxs-lookup"><span data-stu-id="aec35-121">Name</span></span>      |<span data-ttu-id="aec35-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aec35-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aec35-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aec35-123">Authorization</span></span>  | <span data-ttu-id="aec35-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aec35-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aec35-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aec35-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="aec35-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="aec35-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec35-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aec35-129">Request body</span></span>
<span data-ttu-id="aec35-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aec35-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aec35-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aec35-131">Response</span></span>

<span data-ttu-id="aec35-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [суспиЦиаусиприскевент](../resources/suspiciousipriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aec35-132">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aec35-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aec35-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aec35-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aec35-134">Request</span></span>
<span data-ttu-id="aec35-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aec35-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="aec35-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="aec35-136">Response</span></span>
<span data-ttu-id="aec35-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aec35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
