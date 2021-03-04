---
title: Список unfamiliarLocationRiskEvents
description: Извлечение списка объектов unfamiliarlocationriskevent.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: 41300d4983e494e6d53f6de53d4052a0322d6d2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444863"
---
# <a name="list-unfamiliarlocationriskevents-deprecated"></a><span data-ttu-id="dfd63-103">Список незнакомыхLocationRiskEvents (отстает)</span><span class="sxs-lookup"><span data-stu-id="dfd63-103">List unfamiliarLocationRiskEvents (deprecated)</span></span>

<span data-ttu-id="dfd63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfd63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="dfd63-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="dfd63-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="dfd63-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="dfd63-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="dfd63-107">Извлечение списка объектов unfamiliarlocationriskevent.</span><span class="sxs-lookup"><span data-stu-id="dfd63-107">Retrieve a list of unfamiliarlocationriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfd63-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfd63-108">Permissions</span></span>
<span data-ttu-id="dfd63-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfd63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd63-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfd63-111">Permission type</span></span>      | <span data-ttu-id="dfd63-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfd63-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfd63-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfd63-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dfd63-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfd63-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="dfd63-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfd63-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfd63-116">Not supported.</span></span>    |
|<span data-ttu-id="dfd63-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dfd63-117">Application</span></span> | <span data-ttu-id="dfd63-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfd63-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfd63-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfd63-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="dfd63-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfd63-120">Request headers</span></span>
| <span data-ttu-id="dfd63-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dfd63-121">Name</span></span>      |<span data-ttu-id="dfd63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dfd63-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfd63-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfd63-123">Authorization</span></span>  | <span data-ttu-id="dfd63-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfd63-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfd63-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dfd63-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="dfd63-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd63-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfd63-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfd63-129">Request body</span></span>
<span data-ttu-id="dfd63-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfd63-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfd63-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd63-131">Response</span></span>

<span data-ttu-id="dfd63-132">В случае успешной работы этот метод возвращает код отклика и коллекцию незнакомых `200 OK` [объектовLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dfd63-132">If successful, this method returns a `200 OK` response code and collection of [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfd63-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dfd63-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfd63-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfd63-134">Request</span></span>
<span data-ttu-id="dfd63-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfd63-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents
```
##### <a name="response"></a><span data-ttu-id="dfd63-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd63-136">Response</span></span>
<span data-ttu-id="dfd63-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfd63-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List unfamiliarLocationRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


