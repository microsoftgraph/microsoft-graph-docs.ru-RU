---
title: Список Релингпартидетаиледсуммари
description: Получение списка объектов Релингпартидетаиледсуммари.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6009003b47b1e0bf0406cb3f9cbe8853d8a9b72b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971960"
---
# <a name="list-relyingpartydetailedsummary"></a><span data-ttu-id="4c191-103">Список Релингпартидетаиледсуммари</span><span class="sxs-lookup"><span data-stu-id="4c191-103">List relyingPartyDetailedSummary</span></span>

<span data-ttu-id="4c191-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c191-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c191-105">Получение списка объектов **релингпартидетаиледсуммари** .</span><span class="sxs-lookup"><span data-stu-id="4c191-105">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c191-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c191-106">Permissions</span></span>

<span data-ttu-id="4c191-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c191-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c191-109">Permission type</span></span>                        | <span data-ttu-id="4c191-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c191-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c191-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c191-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c191-112">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c191-112">Report.Read.All</span></span> |
| <span data-ttu-id="4c191-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c191-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c191-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c191-114">Not supported.</span></span> |
| <span data-ttu-id="4c191-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c191-115">Application</span></span>                            | <span data-ttu-id="4c191-116">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c191-116">Report.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c191-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c191-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a><span data-ttu-id="4c191-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4c191-118">Function parameters</span></span>

| <span data-ttu-id="4c191-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c191-119">Parameter</span></span> | <span data-ttu-id="4c191-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4c191-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="4c191-121">period</span><span class="sxs-lookup"><span data-stu-id="4c191-121">period</span></span> | <span data-ttu-id="4c191-122">Поддерживаются следующие значения: D1, D7, D30.</span><span class="sxs-lookup"><span data-stu-id="4c191-122">The supported values are: D1, D7, D30.</span></span> <span data-ttu-id="4c191-123">Эти значения указываются в формате Dn, где n — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4c191-123">These values follow the format Dn where n represents the number of days over which the report is aggregated.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="4c191-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c191-124">Optional query parameters</span></span>

<span data-ttu-id="4c191-125">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c191-125">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="4c191-126">Параметр можно использовать `$filter` для фильтрации по релингпартид, мигратионстатус и другим атрибутам.</span><span class="sxs-lookup"><span data-stu-id="4c191-126">You can use the `$filter` parameter to filter by relyingPartyId, migrationStatus and other attributes.</span></span> <span data-ttu-id="4c191-127">Например, $filter = Релингпартид EQ "identifier".</span><span class="sxs-lookup"><span data-stu-id="4c191-127">For example, $filter= relyingPartyId eq 'identifier'.</span></span>
- <span data-ttu-id="4c191-128">Вы можете использовать `$orderby` `$top` Параметры, и `$skip` запросы в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="4c191-128">You can use `$orderby`, `$top`, and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="4c191-129">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c191-129">For general information, see [OData query parameters](/graph/query-parameters).</span></span>


## <a name="request-headers"></a><span data-ttu-id="4c191-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c191-130">Request headers</span></span>

| <span data-ttu-id="4c191-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4c191-131">Name</span></span>      |<span data-ttu-id="4c191-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c191-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c191-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c191-133">Authorization</span></span> | <span data-ttu-id="4c191-134">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4c191-134">Bearer {code}.</span></span> <span data-ttu-id="4c191-135">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c191-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c191-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c191-136">Request body</span></span>

<span data-ttu-id="4c191-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c191-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c191-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c191-138">Response</span></span>

<span data-ttu-id="4c191-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [релингпартидетаиледсуммари](../resources/relyingpartydetailedsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c191-139">If successful, this method returns a `200 OK` response code and the requested [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c191-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c191-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c191-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c191-141">Request</span></span>

<span data-ttu-id="4c191-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c191-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c191-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c191-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```
# <a name="c"></a>[<span data-ttu-id="4c191-144">C#</span><span class="sxs-lookup"><span data-stu-id="4c191-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relyingpartydetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c191-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c191-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relyingpartydetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c191-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c191-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relyingpartydetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c191-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c191-147">Response</span></span>

<span data-ttu-id="4c191-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c191-148">The following is an example of the response.</span></span>

> <span data-ttu-id="4c191-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c191-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


