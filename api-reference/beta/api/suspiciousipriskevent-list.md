---
title: Список СуспиЦиаусиприскевентс
description: Получение списка объектов суспиЦиаусиприскевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 38fd4dc80dccf1b83ddd284bbe620fb8eee0a601
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013876"
---
# <a name="list-suspiciousipriskevents-deprecated"></a><span data-ttu-id="e9291-103">Список СуспиЦиаусиприскевентс (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="e9291-103">List suspiciousIpRiskEvents (deprecated)</span></span>

<span data-ttu-id="e9291-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9291-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="e9291-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="e9291-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="e9291-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="e9291-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="e9291-107">Получение списка объектов суспиЦиаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="e9291-107">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9291-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9291-108">Permissions</span></span>
<span data-ttu-id="e9291-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9291-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9291-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9291-111">Permission type</span></span>      | <span data-ttu-id="e9291-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9291-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9291-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9291-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e9291-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9291-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e9291-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9291-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9291-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9291-116">Not supported.</span></span>    |
|<span data-ttu-id="e9291-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9291-117">Application</span></span> | <span data-ttu-id="e9291-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9291-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9291-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9291-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="e9291-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9291-120">Request headers</span></span>
| <span data-ttu-id="e9291-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e9291-121">Name</span></span>      |<span data-ttu-id="e9291-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e9291-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9291-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9291-123">Authorization</span></span>  | <span data-ttu-id="e9291-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9291-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9291-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9291-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9291-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e9291-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9291-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9291-129">Request body</span></span>
<span data-ttu-id="e9291-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9291-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9291-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9291-131">Response</span></span>

<span data-ttu-id="e9291-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [суспиЦиаусиприскевент](../resources/suspiciousipriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9291-132">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9291-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e9291-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9291-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9291-134">Request</span></span>
<span data-ttu-id="e9291-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9291-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="e9291-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9291-136">Response</span></span>
<span data-ttu-id="e9291-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9291-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List suspiciousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


