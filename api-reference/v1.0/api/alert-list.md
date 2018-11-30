---
title: перечисление оповещений;
description: Получение списка объектов оповещения.
ms.openlocfilehash: c25784f62d37722fc997e57b9f15c9857133b964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027171"
---
# <a name="list-alerts"></a><span data-ttu-id="a7a9f-103">перечисление оповещений;</span><span class="sxs-lookup"><span data-stu-id="a7a9f-103">List alerts</span></span>

<span data-ttu-id="a7a9f-104">Получение списка объектов [оповещение](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="a7a9f-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7a9f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7a9f-105">Permissions</span></span>

<span data-ttu-id="a7a9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7a9f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7a9f-108">Permission type</span></span>      | <span data-ttu-id="a7a9f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7a9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7a9f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7a9f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a7a9f-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a9f-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="a7a9f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7a9f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a7a9f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-113">Not supported.</span></span>  |
|<span data-ttu-id="a7a9f-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a7a9f-114">Application</span></span> | <span data-ttu-id="a7a9f-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a9f-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7a9f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7a9f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7a9f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7a9f-117">Optional query parameters</span></span>

<span data-ttu-id="a7a9f-118">Этот метод поддерживает следующие [Параметры запроса OData](/graph/query-parameters) для настройки ответа:</span><span class="sxs-lookup"><span data-stu-id="a7a9f-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="a7a9f-119">`$top`Возвращает совокупные верхней результаты из каждого API поставщика безопасности.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="a7a9f-120">Чтобы вернуть набор альтернативных свойства, используйте OData `$select` параметр для определения набора свойств **оповещения** , которые будут запроса.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="a7a9f-121">Например, для возврата **assignedTo**, **категории**и свойства **уровень серьезности** , добавьте следующий запрос: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7a9f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7a9f-122">Request headers</span></span>

| <span data-ttu-id="a7a9f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a7a9f-123">Name</span></span>      |<span data-ttu-id="a7a9f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a7a9f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7a9f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7a9f-125">Authorization</span></span>  | <span data-ttu-id="a7a9f-p103">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7a9f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7a9f-128">Request body</span></span>

<span data-ttu-id="a7a9f-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-129">Do not supply a request body for this method.</span></span> <span data-ttu-id="a7a9f-130">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-130">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="a7a9f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7a9f-131">Response</span></span>

<span data-ttu-id="a7a9f-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов **оповещения** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-132">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="a7a9f-133">Если код состояния, отличный от 2xx или 404 возвращается у поставщика или если поставщик времени ожидания, ответ будет `206 Partial Content` код состояния с ответом поставщиков в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-133">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="a7a9f-134">Для получения дополнительных сведений см [Microsoft Graph безопасности API сообщений об ошибках](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="a7a9f-134">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="a7a9f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a7a9f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7a9f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7a9f-136">Request</span></span>

<span data-ttu-id="a7a9f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="a7a9f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7a9f-138">Response</span></span>

<span data-ttu-id="a7a9f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-139">The following is an example of the response.</span></span>

><span data-ttu-id="a7a9f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7a9f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
