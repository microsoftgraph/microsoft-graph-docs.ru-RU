---
title: перечисление оповещений;
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: e6ddf41616d27b41414386f83a9ce067411d92b9
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184513"
---
# <a name="list-alerts"></a><span data-ttu-id="d48db-104">перечисление оповещений;</span><span class="sxs-lookup"><span data-stu-id="d48db-104">List alerts</span></span>

 > <span data-ttu-id="d48db-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d48db-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d48db-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48db-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d48db-107">Получение списка объектов [оповещение](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="d48db-107">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d48db-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d48db-108">Permissions</span></span>

<span data-ttu-id="d48db-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d48db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d48db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d48db-111">Permission type</span></span>      | <span data-ttu-id="d48db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d48db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d48db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d48db-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="d48db-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d48db-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="d48db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d48db-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d48db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48db-116">Not supported.</span></span>  |
|<span data-ttu-id="d48db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d48db-117">Application</span></span> | <span data-ttu-id="d48db-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d48db-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d48db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d48db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d48db-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d48db-120">Optional query parameters</span></span>

<span data-ttu-id="d48db-121">Этот метод поддерживает следующие [Параметры запроса OData](/graph/query-parameters) для настройки ответа:</span><span class="sxs-lookup"><span data-stu-id="d48db-121">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="d48db-122">`$top`Возвращает совокупные верхней результаты из каждого API поставщика безопасности.</span><span class="sxs-lookup"><span data-stu-id="d48db-122">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="d48db-123">Чтобы вернуть набор альтернативных свойства, используйте OData `$select` параметр для определения набора свойств **оповещения** , которые будут запроса.</span><span class="sxs-lookup"><span data-stu-id="d48db-123">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="d48db-124">Например, для возврата **assignedTo**, **категории**и свойства **уровень серьезности** , добавьте следующий запрос: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="d48db-124">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="d48db-125">**Примечание:** `$top` имеет более 1000 оповещения и сочетание `$top`  +  `$skip` не может превышать 6000 оповещения.</span><span class="sxs-lookup"><span data-stu-id="d48db-125">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="d48db-126">Например `/security/alerts?$top=10&$skip=5990` возвращает `200 OK` код ответа, но `/security/alerts?$top=10&$skip=5991` возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="d48db-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="d48db-127">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d48db-127">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d48db-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d48db-128">Request headers</span></span>

| <span data-ttu-id="d48db-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d48db-129">Name</span></span>      |<span data-ttu-id="d48db-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d48db-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d48db-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d48db-131">Authorization</span></span>  | <span data-ttu-id="d48db-p106">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d48db-p106">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d48db-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d48db-134">Request body</span></span>

<span data-ttu-id="d48db-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d48db-135">Do not supply a request body for this method.</span></span> <span data-ttu-id="d48db-136">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="d48db-136">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="d48db-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d48db-137">Response</span></span>

<span data-ttu-id="d48db-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов **оповещения** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d48db-138">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="d48db-139">Если код состояния, отличный от 2xx или 404 возвращается у поставщика или если поставщик времени ожидания, ответ будет `206 Partial Content` код состояния с ответа поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="d48db-139">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="d48db-140">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d48db-140">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="d48db-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d48db-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d48db-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d48db-142">Request</span></span>

<span data-ttu-id="d48db-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d48db-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="d48db-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d48db-144">Response</span></span>

<span data-ttu-id="d48db-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d48db-145">The following is an example of the response.</span></span>

><span data-ttu-id="d48db-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d48db-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
