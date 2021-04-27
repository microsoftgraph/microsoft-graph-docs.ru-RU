---
title: Get reviewSet
description: Извлечение свойств и связей объекта reviewSet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 220a52d7ceb7a3b5fce766a9ec98dbe9c7bf308b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044699"
---
# <a name="get-reviewset"></a><span data-ttu-id="72d52-103">Get reviewSet</span><span class="sxs-lookup"><span data-stu-id="72d52-103">Get reviewSet</span></span>

<span data-ttu-id="72d52-104">Пространство имен: microsoft.graph.ediscovery.ediscovery</span><span class="sxs-lookup"><span data-stu-id="72d52-104">Namespace: microsoft.graph.ediscovery.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d52-105">Извлечение свойств и связей объекта [reviewSet.](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="72d52-105">Retrieve the properties and relationships of a [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72d52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72d52-106">Permissions</span></span>

<span data-ttu-id="72d52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72d52-109">Permission type</span></span>|<span data-ttu-id="72d52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72d52-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72d52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72d52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72d52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d52-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="72d52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72d52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72d52-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d52-114">Not supported.</span></span>|
|<span data-ttu-id="72d52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72d52-115">Application</span></span>|<span data-ttu-id="72d52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72d52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72d52-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72d52-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72d52-118">Optional query parameters</span></span>

<span data-ttu-id="72d52-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="72d52-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="72d52-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="72d52-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="72d52-121">По умолчанию возвращаются все поля набора обзоров; Однако вы можете указать определенные поля для возврата с помощью параметра `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="72d52-121">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="72d52-122">Например, чтобы вернуть только **displayName** и ID, добавьте в запрос следующее: `$select=displayName,Id` .</span><span class="sxs-lookup"><span data-stu-id="72d52-122">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="72d52-123">Поскольку запрос может возвращать многие случаи, их можно фильтровать с помощью **displayName.**</span><span class="sxs-lookup"><span data-stu-id="72d52-123">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="72d52-124">Чтобы фильтровать **по displayName,** добавьте в запрос следующее: где имя набора `$filter=displayName eq 'rs1'` отзывов rs1.</span><span class="sxs-lookup"><span data-stu-id="72d52-124">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="72d52-125">Дополнительные сведения о фильтрации и указании полей см. в рублях [Using Filter Expressions in OData URIS. ](/dynamics-nav/using-filter-expressions-in-odata-uris)</span><span class="sxs-lookup"><span data-stu-id="72d52-125">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72d52-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72d52-126">Request headers</span></span>

| <span data-ttu-id="72d52-127">Имя</span><span class="sxs-lookup"><span data-stu-id="72d52-127">Name</span></span>      |<span data-ttu-id="72d52-128">Описание</span><span class="sxs-lookup"><span data-stu-id="72d52-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72d52-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72d52-129">Authorization</span></span> | <span data-ttu-id="72d52-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72d52-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72d52-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72d52-132">Request body</span></span>

<span data-ttu-id="72d52-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72d52-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72d52-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d52-134">Response</span></span>

<span data-ttu-id="72d52-135">В случае успеха этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72d52-135">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72d52-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="72d52-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72d52-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="72d52-137">Request</span></span>

<span data-ttu-id="72d52-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72d52-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72d52-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="72d52-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="72d52-140">C#</span><span class="sxs-lookup"><span data-stu-id="72d52-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72d52-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d52-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72d52-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72d52-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72d52-143">Java</span><span class="sxs-lookup"><span data-stu-id="72d52-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72d52-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d52-144">Response</span></span>

<span data-ttu-id="72d52-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="72d52-145">The following is an example of the response.</span></span>

> <span data-ttu-id="72d52-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72d52-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
