---
title: Перечисление оповещений
description: Получение списка объектов оповещений.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: d50c3244ae2c0e9f158dc38923136ef3e8656f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459215"
---
# <a name="list-alerts"></a><span data-ttu-id="4e7a6-103">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="4e7a6-103">List alerts</span></span>

<span data-ttu-id="4e7a6-104">Получение списка объектов [оповещений](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7a6-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e7a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e7a6-105">Permissions</span></span>

<span data-ttu-id="4e7a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e7a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e7a6-108">Permission type</span></span>      | <span data-ttu-id="4e7a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e7a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e7a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e7a6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e7a6-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e7a6-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="4e7a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e7a6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4e7a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-113">Not supported.</span></span>  |
|<span data-ttu-id="4e7a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e7a6-114">Application</span></span> | <span data-ttu-id="4e7a6-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e7a6-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e7a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e7a6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e7a6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e7a6-117">Optional query parameters</span></span>

<span data-ttu-id="4e7a6-118">Этот метод поддерживает следующие [Параметры запроса OData](/graph/query-parameters) для настройки отклика:</span><span class="sxs-lookup"><span data-stu-id="4e7a6-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="4e7a6-119">`$top`Возвращает сводные результаты из каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="4e7a6-120">Чтобы получить альтернативный набор свойств, используйте параметр запроса `$select` OData, чтобы указать требуемый набор свойств **оповещения** .</span><span class="sxs-lookup"><span data-stu-id="4e7a6-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="4e7a6-121">Например, чтобы вернуть свойства **assignedTo**, **Category**и **Severity** , добавьте в запрос следующее: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="4e7a6-122">**Примечание:** `$top` ограничено 1000 оповещений, а их `$top`  +  `$skip` комбинация не может превышать 6000.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="4e7a6-123">Например, `/security/alerts?$top=10&$skip=5990` возвращает код `200 OK` отклика, но `/security/alerts?$top=10&$skip=5991` возвратит код `400 Bad Request` отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="4e7a6-124">Дополнительные сведения см. в разделе [ответ об ошибках API безопасности Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="4e7a6-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e7a6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e7a6-125">Request headers</span></span>

| <span data-ttu-id="4e7a6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4e7a6-126">Name</span></span>      |<span data-ttu-id="4e7a6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4e7a6-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e7a6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e7a6-128">Authorization</span></span>  | <span data-ttu-id="4e7a6-129">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-129">Bearer {code}.</span></span> <span data-ttu-id="4e7a6-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7a6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e7a6-131">Request body</span></span>

<span data-ttu-id="4e7a6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="4e7a6-133">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="4e7a6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e7a6-134">Response</span></span>

<span data-ttu-id="4e7a6-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **Alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="4e7a6-136">Если поставщик возвращает код состояния, отличный от 2xx или 404, или если время ожидания поставщика истекло, ответ будет кодом `206 Partial Content` состояния с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="4e7a6-137">Дополнительные сведения см. в разделе [ответ об ошибках API безопасности Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="4e7a6-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="4e7a6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e7a6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e7a6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e7a6-139">Request</span></span>

<span data-ttu-id="4e7a6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="4e7a6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e7a6-141">Response</span></span>

<span data-ttu-id="4e7a6-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-142">The following is an example of the response.</span></span>

><span data-ttu-id="4e7a6-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e7a6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
