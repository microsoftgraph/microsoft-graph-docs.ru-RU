---
title: Список relyingPartyDetailedSummary
description: Извлечение списка объектов relyingPartyDetailedSummary.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 17e4c4b3e92173593c768267f6db957942241cdf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052861"
---
# <a name="list-relyingpartydetailedsummary"></a><span data-ttu-id="8aba8-103">Список relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="8aba8-103">List relyingPartyDetailedSummary</span></span>

<span data-ttu-id="8aba8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aba8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aba8-105">Извлечение списка **объектов relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="8aba8-105">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aba8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aba8-106">Permissions</span></span>

<span data-ttu-id="8aba8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8aba8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aba8-109">Permission type</span></span>                        | <span data-ttu-id="8aba8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aba8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8aba8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aba8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8aba8-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="8aba8-112">Report.Read.All</span></span> |
| <span data-ttu-id="8aba8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aba8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aba8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aba8-114">Not supported.</span></span> |
| <span data-ttu-id="8aba8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8aba8-115">Application</span></span>                            | <span data-ttu-id="8aba8-116">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="8aba8-116">Report.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aba8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aba8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a><span data-ttu-id="8aba8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8aba8-118">Function parameters</span></span>

| <span data-ttu-id="8aba8-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="8aba8-119">Parameter</span></span> | <span data-ttu-id="8aba8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8aba8-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8aba8-121">period</span><span class="sxs-lookup"><span data-stu-id="8aba8-121">period</span></span> | <span data-ttu-id="8aba8-122">Поддерживаемые значения: D1, D7, D30.</span><span class="sxs-lookup"><span data-stu-id="8aba8-122">The supported values are: D1, D7, D30.</span></span> <span data-ttu-id="8aba8-123">Эти значения указываются в формате Dn, где n — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8aba8-123">These values follow the format Dn where n represents the number of days over which the report is aggregated.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="8aba8-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8aba8-124">Optional query parameters</span></span>

<span data-ttu-id="8aba8-125">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8aba8-125">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="8aba8-126">Этот параметр можно `$filter` фильтровать, полагаясь наPartyId, migrationStatus и другие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="8aba8-126">You can use the `$filter` parameter to filter by relyingPartyId, migrationStatus and other attributes.</span></span> <span data-ttu-id="8aba8-127">Например, $filter= идентификатор eq relyingPartyId.</span><span class="sxs-lookup"><span data-stu-id="8aba8-127">For example, $filter= relyingPartyId eq 'identifier'.</span></span>
- <span data-ttu-id="8aba8-128">Вы можете использовать `$orderby` `$top` параметры и `$skip` параметры запроса в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="8aba8-128">You can use `$orderby`, `$top`, and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="8aba8-129">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8aba8-129">For general information, see [OData query parameters](/graph/query-parameters).</span></span>


## <a name="request-headers"></a><span data-ttu-id="8aba8-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aba8-130">Request headers</span></span>

| <span data-ttu-id="8aba8-131">Имя</span><span class="sxs-lookup"><span data-stu-id="8aba8-131">Name</span></span>      |<span data-ttu-id="8aba8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8aba8-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8aba8-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aba8-133">Authorization</span></span> | <span data-ttu-id="8aba8-134">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="8aba8-134">Bearer {code}.</span></span> <span data-ttu-id="8aba8-135">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8aba8-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aba8-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aba8-136">Request body</span></span>

<span data-ttu-id="8aba8-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8aba8-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aba8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aba8-138">Response</span></span>

<span data-ttu-id="8aba8-139">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8aba8-139">If successful, this method returns a `200 OK` response code and the requested [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aba8-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="8aba8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aba8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aba8-141">Request</span></span>

<span data-ttu-id="8aba8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8aba8-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8aba8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aba8-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```
# <a name="c"></a>[<span data-ttu-id="8aba8-144">C#</span><span class="sxs-lookup"><span data-stu-id="8aba8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relyingpartydetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8aba8-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aba8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relyingpartydetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aba8-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aba8-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relyingpartydetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aba8-147">Java</span><span class="sxs-lookup"><span data-stu-id="8aba8-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-relyingpartydetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8aba8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aba8-148">Response</span></span>

<span data-ttu-id="8aba8-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8aba8-149">The following is an example of the response.</span></span>

> <span data-ttu-id="8aba8-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8aba8-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1fec2821-6c43-4919-9560-ce36c820faa5",
  "relyingPartyId": "https://contosoorg-dev-ed.my.contoso.com",
  "serviceId": "287ed092-c182-4748-99a9-9ef3b5a0a0f9",
  "relyingPartyName": "contoso",
  "successfulSignInCount": 90,
  "failedSignInCount": 10,
  "totalSignInCount": 100,
  "signInSuccessRate":90.0,
  "uniqueUserCount": 10,
  "migrationStatus": "ready",
  "replyUrls": [
      "https://contosoorg-dev-ed.my.contoso.com"
  ],
  "migrationValidationDetails": [
      {
          "name": "AdditionalWSFedEndpointCheckResult",
          "value": "{\"result\": 0, \"message\": \"No additional WS-Federation endpoints were found.\"}"
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get relyingPartyDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


