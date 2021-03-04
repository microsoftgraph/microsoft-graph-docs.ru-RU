---
title: Список подозрительныхIpRiskEvents
description: Извлечение списка подозрительных объектов.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 1fb00ef2852e908ebdb4e5d9b2cfd84d561985de
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445010"
---
# <a name="list-suspiciousipriskevents-deprecated"></a><span data-ttu-id="02e9f-103">Список подозрительныхIpRiskEvents (обесценен)</span><span class="sxs-lookup"><span data-stu-id="02e9f-103">List suspiciousIpRiskEvents (deprecated)</span></span>

<span data-ttu-id="02e9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="02e9f-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="02e9f-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="02e9f-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="02e9f-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="02e9f-107">Извлечение списка подозрительных объектов.</span><span class="sxs-lookup"><span data-stu-id="02e9f-107">Retrieve a list of suspiciousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="02e9f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02e9f-108">Permissions</span></span>
<span data-ttu-id="02e9f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e9f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02e9f-111">Permission type</span></span>      | <span data-ttu-id="02e9f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02e9f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02e9f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02e9f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02e9f-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e9f-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="02e9f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02e9f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02e9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e9f-116">Not supported.</span></span>    |
|<span data-ttu-id="02e9f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="02e9f-117">Application</span></span> | <span data-ttu-id="02e9f-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e9f-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02e9f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02e9f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="02e9f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02e9f-120">Request headers</span></span>
| <span data-ttu-id="02e9f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="02e9f-121">Name</span></span>      |<span data-ttu-id="02e9f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="02e9f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02e9f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02e9f-123">Authorization</span></span>  | <span data-ttu-id="02e9f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02e9f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02e9f-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="02e9f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="02e9f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="02e9f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e9f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02e9f-129">Request body</span></span>
<span data-ttu-id="02e9f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02e9f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02e9f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e9f-131">Response</span></span>

<span data-ttu-id="02e9f-132">В случае успешной работы этот метод возвращает код ответа и коллекцию подозрительных `200 OK` [объектовIpRiskEvent](../resources/suspiciousipriskevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02e9f-132">If successful, this method returns a `200 OK` response code and collection of [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02e9f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="02e9f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02e9f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e9f-134">Request</span></span>
<span data-ttu-id="02e9f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e9f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="02e9f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e9f-136">Response</span></span>
<span data-ttu-id="02e9f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02e9f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


