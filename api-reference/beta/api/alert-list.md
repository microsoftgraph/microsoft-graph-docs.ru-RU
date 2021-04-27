---
title: Перечисление оповещений
description: Получение списка объектов alert.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 79d430f7ed898795a8fec07280b5bb30d9400af8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048192"
---
# <a name="list-alerts"></a><span data-ttu-id="4457c-103">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="4457c-103">List alerts</span></span>

<span data-ttu-id="4457c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4457c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4457c-105">Получение списка объектов [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="4457c-105">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4457c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4457c-106">Permissions</span></span>

<span data-ttu-id="4457c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4457c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4457c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4457c-109">Permission type</span></span>      | <span data-ttu-id="4457c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4457c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4457c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4457c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4457c-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4457c-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="4457c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4457c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4457c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4457c-114">Not supported.</span></span>  |
|<span data-ttu-id="4457c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4457c-115">Application</span></span> | <span data-ttu-id="4457c-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4457c-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4457c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4457c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4457c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4457c-118">Optional query parameters</span></span>

<span data-ttu-id="4457c-119">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4457c-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="4457c-120">`$top` – Возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="4457c-120">`$top` - Returns the aggregated top results from each security API provider.</span></span>
- `$filter`

<span data-ttu-id="4457c-121">В таблице ниже перечислены ключевые слова `$filter` по именам поставщиков.</span><span class="sxs-lookup"><span data-stu-id="4457c-121">The following table lists the `$filter` keywords by each vendor name.</span></span>

| <span data-ttu-id="4457c-122">Наименование поставщика</span><span class="sxs-lookup"><span data-stu-id="4457c-122">Vendor name</span></span>      |<span data-ttu-id="4457c-123">ключевое слово $filter</span><span class="sxs-lookup"><span data-stu-id="4457c-123">$filter keyword</span></span>|
|:----------|:----------|
| <span data-ttu-id="4457c-124">Расширенная защита от угроз Azure</span><span class="sxs-lookup"><span data-stu-id="4457c-124">Azure Advanced Threat Protection</span></span> | <span data-ttu-id="4457c-125">Расширенная защита от угроз Azure</span><span class="sxs-lookup"><span data-stu-id="4457c-125">Azure Advanced Threat Protection</span></span> | 
| <span data-ttu-id="4457c-126">Центр безопасности Azure</span><span class="sxs-lookup"><span data-stu-id="4457c-126">Azure Security Center</span></span> | <span data-ttu-id="4457c-127">ASC</span><span class="sxs-lookup"><span data-stu-id="4457c-127">ASC</span></span> |
| <span data-ttu-id="4457c-128">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="4457c-128">Microsoft Cloud App Security</span></span> | <span data-ttu-id="4457c-129">MCAS</span><span class="sxs-lookup"><span data-stu-id="4457c-129">MCAS</span></span> |
| <span data-ttu-id="4457c-130">Защита идентификации Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4457c-130">Azure Active Directory Identity Protection</span></span> | <span data-ttu-id="4457c-131">IPC</span><span class="sxs-lookup"><span data-stu-id="4457c-131">IPC</span></span> |
| <span data-ttu-id="4457c-132">Azure Sentinel</span><span class="sxs-lookup"><span data-stu-id="4457c-132">Azure Sentinel</span></span> | <span data-ttu-id="4457c-133">Azure Sentinel</span><span class="sxs-lookup"><span data-stu-id="4457c-133">Azure Sentinel</span></span> |
| <span data-ttu-id="4457c-134">Advanced Threat Protection в Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="4457c-134">Microsoft Defender Advanced Threat Protection</span></span> | <span data-ttu-id="4457c-135">ATP в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="4457c-135">Microsoft Defender ATP</span></span> |
| <span data-ttu-id="4457c-136">Office 365</span><span class="sxs-lookup"><span data-stu-id="4457c-136">Office 365</span></span> |  <span data-ttu-id="4457c-137">В настоящее время не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4457c-137">Not currently supported.</span></span> |

<span data-ttu-id="4457c-138">Чтобы возвратить альтернативный набор свойств, используйте параметр запроса OData `$select`, чтобы указать нужный набор свойств **alert**.</span><span class="sxs-lookup"><span data-stu-id="4457c-138">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="4457c-139">Например, чтобы вернуть свойства **assignedTo**, **category** и **severity**, добавьте в свой запрос следующее: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="4457c-139">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="4457c-140">**Примечание.** Параметр запроса OData `$top` имеет ограничение в 1000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="4457c-140">**Note:** The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="4457c-141">В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="4457c-141">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="4457c-142">Для разбивки на страницы можно использовать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="4457c-142">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="4457c-143">Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений.</span><span class="sxs-lookup"><span data-stu-id="4457c-143">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="4457c-144">Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="4457c-144">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="4457c-145">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="4457c-145">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4457c-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4457c-146">Request headers</span></span>

| <span data-ttu-id="4457c-147">Имя</span><span class="sxs-lookup"><span data-stu-id="4457c-147">Name</span></span>      |<span data-ttu-id="4457c-148">Описание</span><span class="sxs-lookup"><span data-stu-id="4457c-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4457c-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4457c-149">Authorization</span></span>  | <span data-ttu-id="4457c-150">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4457c-150">Bearer {code}.</span></span> <span data-ttu-id="4457c-151">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4457c-151">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4457c-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4457c-152">Request body</span></span>

<span data-ttu-id="4457c-153">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4457c-153">Do not supply a request body for this method.</span></span> <span data-ttu-id="4457c-154">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4457c-154">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="4457c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4457c-155">Response</span></span>

<span data-ttu-id="4457c-156">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов **alert** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4457c-156">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="4457c-157">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4457c-157">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="4457c-158">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="4457c-158">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="4457c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4457c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="4457c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4457c-160">Request</span></span>

<span data-ttu-id="4457c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4457c-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4457c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4457c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts
```
# <a name="c"></a>[<span data-ttu-id="4457c-163">C#</span><span class="sxs-lookup"><span data-stu-id="4457c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4457c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4457c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4457c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4457c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4457c-166">Java</span><span class="sxs-lookup"><span data-stu-id="4457c-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4457c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4457c-167">Response</span></span>

<span data-ttu-id="4457c-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4457c-168">The following is an example of the response.</span></span>

><span data-ttu-id="4457c-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4457c-169">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "suppressions": [
  ]
}
-->


