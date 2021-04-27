---
title: Получение объекта anonymousIpRiskEvent
description: Извлечение свойств и связей объекта anonymousipriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: d29167cf1381c3b89fad376aa71b1b9f5d8f507c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048171"
---
# <a name="get-anonymousipriskevent-deprecated"></a><span data-ttu-id="30e67-103">Get anonymousIpRiskEvent (deprecated)</span><span class="sxs-lookup"><span data-stu-id="30e67-103">Get anonymousIpRiskEvent (deprecated)</span></span>

<span data-ttu-id="30e67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30e67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="30e67-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="30e67-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="30e67-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="30e67-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="30e67-107">Извлечение свойств и связей объекта anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="30e67-107">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="30e67-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30e67-108">Permissions</span></span>
<span data-ttu-id="30e67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30e67-111">Permission type</span></span>      | <span data-ttu-id="30e67-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30e67-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30e67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30e67-113">Delegated (work or school account)</span></span> | <span data-ttu-id="30e67-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e67-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="30e67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30e67-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e67-116">Not supported.</span></span>    |
|<span data-ttu-id="30e67-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="30e67-117">Application</span></span> | <span data-ttu-id="30e67-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e67-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30e67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30e67-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="30e67-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30e67-120">Request headers</span></span>
| <span data-ttu-id="30e67-121">Имя</span><span class="sxs-lookup"><span data-stu-id="30e67-121">Name</span></span>      |<span data-ttu-id="30e67-122">Описание</span><span class="sxs-lookup"><span data-stu-id="30e67-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30e67-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30e67-123">Authorization</span></span>  | <span data-ttu-id="30e67-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30e67-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30e67-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30e67-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="30e67-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="30e67-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e67-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30e67-129">Request body</span></span>
<span data-ttu-id="30e67-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30e67-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30e67-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e67-131">Response</span></span>

<span data-ttu-id="30e67-132">В случае успеха этот метод возвращает код ответа и `200 OK` [анонимный объектIpRiskEvent](../resources/anonymousipriskevent.md) в значении тела отклика.</span><span class="sxs-lookup"><span data-stu-id="30e67-132">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="30e67-133">Пример</span><span class="sxs-lookup"><span data-stu-id="30e67-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30e67-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="30e67-134">Request</span></span>
<span data-ttu-id="30e67-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30e67-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="30e67-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e67-136">Response</span></span>
<span data-ttu-id="30e67-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30e67-137">Here is an example of the response.</span></span> <span data-ttu-id="30e67-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30e67-138">Note: The response object shown here might be shortened for readability.</span></span>
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


