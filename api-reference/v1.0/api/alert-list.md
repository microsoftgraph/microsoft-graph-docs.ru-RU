---
title: Перечисление оповещений
description: Получение списка объектов alert.
author: preetikr
localization_priority: Priority
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: be594c14612e8957e052ba536a1cf3c74fe7cdf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518961"
---
# <a name="list-alerts"></a><span data-ttu-id="7bc0d-103">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="7bc0d-103">List alerts</span></span>

<span data-ttu-id="7bc0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bc0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bc0d-105">Получение списка объектов [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="7bc0d-105">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bc0d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc0d-106">Permissions</span></span>

<span data-ttu-id="7bc0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc0d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc0d-109">Permission type</span></span>      | <span data-ttu-id="7bc0d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bc0d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc0d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bc0d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="7bc0d-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc0d-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="7bc0d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bc0d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7bc0d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-114">Not supported.</span></span>  |
|<span data-ttu-id="7bc0d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7bc0d-115">Application</span></span> | <span data-ttu-id="7bc0d-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc0d-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bc0d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bc0d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}' and {property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bc0d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bc0d-118">Optional query parameters</span></span>

<span data-ttu-id="7bc0d-119">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="7bc0d-120">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="7bc0d-121">Чтобы возвратить альтернативный набор свойств, используйте параметр запроса OData `$select`, чтобы указать нужный набор свойств **alert**.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-121">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="7bc0d-122">Например, чтобы вернуть свойства **assignedTo**, **category** и **severity**, добавьте в свой запрос следующее: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-122">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="7bc0d-123">**Примечание.** Параметр запроса OData `$top` имеет ограничение в 1000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-123">**Note:** The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="7bc0d-124">В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-124">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="7bc0d-125">Для разбивки на страницы можно использовать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-125">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="7bc0d-126">Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-126">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="7bc0d-127">Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-127">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="7bc0d-128">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="7bc0d-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bc0d-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bc0d-129">Request headers</span></span>

| <span data-ttu-id="7bc0d-130">Имя</span><span class="sxs-lookup"><span data-stu-id="7bc0d-130">Name</span></span>      |<span data-ttu-id="7bc0d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc0d-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bc0d-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bc0d-132">Authorization</span></span>  | <span data-ttu-id="7bc0d-133">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-133">Bearer {code}.</span></span> <span data-ttu-id="7bc0d-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bc0d-135">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="7bc0d-135">Request body</span></span>

<span data-ttu-id="7bc0d-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-136">Do not supply a request body for this method.</span></span> <span data-ttu-id="7bc0d-137">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-137">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="7bc0d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc0d-138">Response</span></span>

<span data-ttu-id="7bc0d-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов **alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-139">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="7bc0d-140">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-140">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="7bc0d-141">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="7bc0d-141">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="7bc0d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="7bc0d-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bc0d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bc0d-143">Request</span></span>

<span data-ttu-id="7bc0d-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bc0d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc0d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="c"></a>[<span data-ttu-id="7bc0d-146">C#</span><span class="sxs-lookup"><span data-stu-id="7bc0d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bc0d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bc0d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bc0d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bc0d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bc0d-149">Java</span><span class="sxs-lookup"><span data-stu-id="7bc0d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bc0d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc0d-150">Response</span></span>

<span data-ttu-id="7bc0d-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-151">The following is an example of the response.</span></span>

><span data-ttu-id="7bc0d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bc0d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
