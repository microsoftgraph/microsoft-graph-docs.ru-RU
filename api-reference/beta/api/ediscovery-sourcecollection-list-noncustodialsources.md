---
title: Список noncustodialSources
description: Получите ресурсы noncustodialDataSource из свойства навигации noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 65f59c6694131ce5af98511af75e5424fb06a7ce
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240801"
---
# <a name="list-noncustodialsources"></a><span data-ttu-id="26e8d-103">Список noncustodialSources</span><span class="sxs-lookup"><span data-stu-id="26e8d-103">List noncustodialSources</span></span>

<span data-ttu-id="26e8d-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="26e8d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e8d-105">Получите список [noncustodialDataSource,](../resources/ediscovery-noncustodialdatasource.md) связанный с [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="26e8d-105">Get a list of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) associated with a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="26e8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26e8d-106">Permissions</span></span>

<span data-ttu-id="26e8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e8d-109">Permission type</span></span>|<span data-ttu-id="26e8d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e8d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e8d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e8d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26e8d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e8d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="26e8d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e8d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e8d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e8d-114">Not supported.</span></span>|
|<span data-ttu-id="26e8d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e8d-115">Application</span></span>|<span data-ttu-id="26e8d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e8d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e8d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e8d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26e8d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26e8d-118">Optional query parameters</span></span>

<span data-ttu-id="26e8d-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="26e8d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="26e8d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="26e8d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="26e8d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26e8d-121">Request headers</span></span>

|<span data-ttu-id="26e8d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="26e8d-122">Name</span></span>|<span data-ttu-id="26e8d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="26e8d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26e8d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e8d-124">Authorization</span></span>|<span data-ttu-id="26e8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e8d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e8d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e8d-127">Request body</span></span>

<span data-ttu-id="26e8d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26e8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26e8d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e8d-129">Response</span></span>

<span data-ttu-id="26e8d-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26e8d-130">If successful, this method returns a `200 OK` response code and a collection of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26e8d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="26e8d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26e8d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e8d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="26e8d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="26e8d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```
# <a name="c"></a>[<span data-ttu-id="26e8d-134">C#</span><span class="sxs-lookup"><span data-stu-id="26e8d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-noncustodialdatasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26e8d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26e8d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-noncustodialdatasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26e8d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26e8d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-noncustodialdatasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26e8d-137">Java</span><span class="sxs-lookup"><span data-stu-id="26e8d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-noncustodialdatasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26e8d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e8d-138">Response</span></span>

> <span data-ttu-id="26e8d-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26e8d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.noncustodialDataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.ediscovery.noncustodialDataSource)",
    "value": [
        {
            "status": "0",
            "lastModifiedDateTime": "2021-04-07T16:45:49.625141Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "39383530323537383742433232433246",
            "displayName": "French fry closet",
            "createdDateTime": "2021-04-07T16:45:49.5761676Z",
            "applyHoldToSource": false
        }
    ]
}
```
