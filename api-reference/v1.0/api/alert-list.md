---
title: Перечисление оповещений
description: Получение списка объектов alert.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d18f49c5e1a0dcc8d079816ff7ad17c6e21df2ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551381"
---
# <a name="list-alerts"></a><span data-ttu-id="8665f-103">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="8665f-103">List alerts</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8665f-104">Получение списка объектов [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="8665f-104">Retrieve a list of [plannertask](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8665f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8665f-105">Permissions</span></span>

<span data-ttu-id="8665f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8665f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8665f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8665f-108">Permission type</span></span>      | <span data-ttu-id="8665f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8665f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8665f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8665f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8665f-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8665f-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="8665f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8665f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8665f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8665f-113">Not supported.</span></span>  |
|<span data-ttu-id="8665f-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8665f-114">Application</span></span> | <span data-ttu-id="8665f-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8665f-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8665f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8665f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8665f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8665f-117">Optional query parameters</span></span>

<span data-ttu-id="8665f-118">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8665f-118">This method supports the following OData Query Parameters to help customize the response.</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="8665f-119">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="8665f-119">`$top` will return the aggregated top results from each security API provider.</span></span>

<span data-ttu-id="8665f-120">Чтобы возвратить альтернативный набор свойств, используйте параметр запроса OData `$select`, чтобы указать нужный набор свойств **alert**.</span><span class="sxs-lookup"><span data-stu-id="8665f-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="8665f-121">Например, чтобы вернуть свойства **assignedTo**, **category** и **severity**, добавьте в свой запрос следующее: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="8665f-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="8665f-122">**Примечание.** Параметр `$top` ограничен значением 1000 оповещений, а сочетание `$top` + `$skip` не может превышать 6000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="8665f-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="8665f-123">Например, `/security/alerts?$top=10&$skip=5990` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=5991` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="8665f-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="8665f-124">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="8665f-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8665f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8665f-125">Request headers</span></span>

| <span data-ttu-id="8665f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8665f-126">Name</span></span>      |<span data-ttu-id="8665f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8665f-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8665f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8665f-128">Authorization</span></span>  | <span data-ttu-id="8665f-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="8665f-129">Bearer {code}</span></span> <span data-ttu-id="8665f-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8665f-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8665f-131">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="8665f-131">Request body</span></span>

<span data-ttu-id="8665f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8665f-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="8665f-133">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="8665f-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="8665f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8665f-134">Response</span></span>

<span data-ttu-id="8665f-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов **alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8665f-135">If successful, this method returns a `200 OK` response code and collection of **directoryObject** objects in the response body.</span></span> <span data-ttu-id="8665f-136">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="8665f-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="8665f-137">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="8665f-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="8665f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8665f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="8665f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8665f-139">Request</span></span>

<span data-ttu-id="8665f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8665f-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="8665f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8665f-141">Response</span></span>

<span data-ttu-id="8665f-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8665f-142">The following is an example of the response.</span></span>

><span data-ttu-id="8665f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8665f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
