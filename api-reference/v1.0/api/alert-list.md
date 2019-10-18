---
title: Перечисление оповещений
description: Получение списка объектов alert.
author: preetikr
localization_priority: Priority
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 41f5badd0e4a9ef7ae0580a5c231dae7500b020c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726608"
---
# <a name="list-alerts"></a><span data-ttu-id="d298d-103">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="d298d-103">List alerts</span></span>

<span data-ttu-id="d298d-104">Получение списка объектов [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="d298d-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d298d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d298d-105">Permissions</span></span>

<span data-ttu-id="d298d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d298d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d298d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d298d-108">Permission type</span></span>      | <span data-ttu-id="d298d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d298d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d298d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d298d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d298d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d298d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="d298d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d298d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d298d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d298d-113">Not supported.</span></span>  |
|<span data-ttu-id="d298d-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="d298d-114">Application</span></span> | <span data-ttu-id="d298d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d298d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d298d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d298d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}' and {property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d298d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d298d-117">Optional query parameters</span></span>

<span data-ttu-id="d298d-118">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d298d-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="d298d-119">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="d298d-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="d298d-120">Чтобы возвратить альтернативный набор свойств, используйте параметр запроса OData `$select`, чтобы указать нужный набор свойств **alert**.</span><span class="sxs-lookup"><span data-stu-id="d298d-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="d298d-121">Например, чтобы вернуть свойства **assignedTo**, **category** и **severity**, добавьте в свой запрос следующее: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="d298d-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="d298d-122">**Примечание.** Параметр `$top` ограничен значением 1000 оповещений, а сочетание `$top` + `$skip` не может превышать 6000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="d298d-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="d298d-123">Например, `/security/alerts?$top=10&$skip=5990` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=5991` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="d298d-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="d298d-124">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d298d-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d298d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d298d-125">Request headers</span></span>

| <span data-ttu-id="d298d-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d298d-126">Name</span></span>      |<span data-ttu-id="d298d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d298d-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d298d-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d298d-128">Authorization</span></span>  | <span data-ttu-id="d298d-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="d298d-129">Bearer {code}.</span></span> <span data-ttu-id="d298d-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d298d-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d298d-131">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="d298d-131">Request body</span></span>

<span data-ttu-id="d298d-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d298d-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="d298d-133">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="d298d-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="d298d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d298d-134">Response</span></span>

<span data-ttu-id="d298d-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов **alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d298d-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="d298d-136">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="d298d-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="d298d-137">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d298d-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="d298d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d298d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d298d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d298d-139">Request</span></span>

<span data-ttu-id="d298d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d298d-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d298d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d298d-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d298d-142">C#</span><span class="sxs-lookup"><span data-stu-id="d298d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d298d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d298d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d298d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d298d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d298d-145">Java</span><span class="sxs-lookup"><span data-stu-id="d298d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d298d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d298d-146">Response</span></span>

<span data-ttu-id="d298d-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d298d-147">The following is an example of the response.</span></span>

><span data-ttu-id="d298d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d298d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
