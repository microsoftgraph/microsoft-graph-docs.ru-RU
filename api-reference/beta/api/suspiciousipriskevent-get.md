---
title: Получение объекта suspiciousIpRiskEvent
description: Извлечение свойств и связей объекта suspiciousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: a0d879e95de6fdfe70b74ad4b9632ab1c650b0bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054870"
---
# <a name="get-suspiciousipriskevent-deprecated"></a><span data-ttu-id="d5d09-103">Get suspiciousIpRiskEvent (deprecated)</span><span class="sxs-lookup"><span data-stu-id="d5d09-103">Get suspiciousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="d5d09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="d5d09-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="d5d09-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="d5d09-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="d5d09-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="d5d09-107">Извлечение свойств и связей объекта suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="d5d09-107">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5d09-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5d09-108">Permissions</span></span>
<span data-ttu-id="d5d09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5d09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5d09-111">Permission type</span></span>      | <span data-ttu-id="d5d09-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5d09-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5d09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5d09-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d5d09-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5d09-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="d5d09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5d09-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5d09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5d09-116">Not supported.</span></span>    |
|<span data-ttu-id="d5d09-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5d09-117">Application</span></span> | <span data-ttu-id="d5d09-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5d09-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5d09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5d09-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d5d09-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5d09-120">Request headers</span></span>
| <span data-ttu-id="d5d09-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d5d09-121">Name</span></span>      |<span data-ttu-id="d5d09-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d09-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5d09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5d09-123">Authorization</span></span>  | <span data-ttu-id="d5d09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5d09-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5d09-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d5d09-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d5d09-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d5d09-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d09-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5d09-129">Request body</span></span>
<span data-ttu-id="d5d09-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5d09-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5d09-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5d09-131">Response</span></span>

<span data-ttu-id="d5d09-132">В случае успешной работы этот метод возвращает код ответа и подозрительный `200 OK` [объектIpRiskEvent](../resources/suspiciousipriskevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d5d09-132">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5d09-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d5d09-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5d09-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5d09-134">Request</span></span>
<span data-ttu-id="d5d09-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5d09-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="d5d09-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5d09-136">Response</span></span>
<span data-ttu-id="d5d09-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5d09-137">Here is an example of the response.</span></span> <span data-ttu-id="d5d09-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5d09-138">Note: The response object shown here might be shortened for readability.</span></span>
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


