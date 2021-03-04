---
title: Получение объекта leakedCredentialsRiskEvent
description: Извлечение свойств и связей объекта leakedcredentialsriskevent.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: identity-and-sign-in
ms.openlocfilehash: c76eab673cc93f31dfa4f95cb2847c91a427d2f2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443785"
---
# <a name="get-leakedcredentialsriskevent-deprecated"></a><span data-ttu-id="a36fa-103">Get leakedCredentialsRiskEvent (deprecated)</span><span class="sxs-lookup"><span data-stu-id="a36fa-103">Get leakedCredentialsRiskEvent (deprecated)</span></span>

<span data-ttu-id="a36fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a36fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="a36fa-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="a36fa-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="a36fa-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="a36fa-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="a36fa-107">Извлечение свойств и связей объекта leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="a36fa-107">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a36fa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a36fa-108">Permissions</span></span>
<span data-ttu-id="a36fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a36fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a36fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a36fa-111">Permission type</span></span>      | <span data-ttu-id="a36fa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a36fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a36fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a36fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a36fa-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a36fa-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="a36fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a36fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a36fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a36fa-116">Not supported.</span></span>    |
|<span data-ttu-id="a36fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a36fa-117">Application</span></span> | <span data-ttu-id="a36fa-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="a36fa-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a36fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a36fa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a36fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a36fa-120">Request headers</span></span>
| <span data-ttu-id="a36fa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a36fa-121">Name</span></span>      |<span data-ttu-id="a36fa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a36fa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a36fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a36fa-123">Authorization</span></span>  | <span data-ttu-id="a36fa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a36fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a36fa-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a36fa-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="a36fa-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a36fa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a36fa-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a36fa-129">Request body</span></span>
<span data-ttu-id="a36fa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a36fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a36fa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a36fa-131">Response</span></span>

<span data-ttu-id="a36fa-132">В случае успешной работы этот метод возвращает код отклика и передает `200 OK` [объектCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) в текст ответа.</span><span class="sxs-lookup"><span data-stu-id="a36fa-132">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a36fa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a36fa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a36fa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a36fa-134">Request</span></span>
<span data-ttu-id="a36fa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a36fa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="a36fa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a36fa-136">Response</span></span>
<span data-ttu-id="a36fa-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a36fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "closedDateTime": null,
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "active",
  "riskLevel": "high",
  "riskType": "LeakedCredentialsRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


