---
title: List custodianSources
description: Получите список объектов dataSource, связанных с исходным собранием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e1a0a653476ff0226d33c19f33eda9d1d7bc2c04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952113"
---
# <a name="list-custodiansources"></a><span data-ttu-id="bea17-103">List custodianSources</span><span class="sxs-lookup"><span data-stu-id="bea17-103">List custodianSources</span></span>

<span data-ttu-id="bea17-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bea17-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea17-105">Получите список объектов [dataSource,](../resources/ediscovery-datasource.md) связанных с исходным собранием.</span><span class="sxs-lookup"><span data-stu-id="bea17-105">Get the list of [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="bea17-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bea17-106">Permissions</span></span>

<span data-ttu-id="bea17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea17-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bea17-109">Permission type</span></span>|<span data-ttu-id="bea17-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bea17-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bea17-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bea17-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bea17-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea17-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bea17-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bea17-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bea17-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea17-114">Not supported.</span></span>|
|<span data-ttu-id="bea17-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bea17-115">Application</span></span>|<span data-ttu-id="bea17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea17-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bea17-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bea17-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bea17-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bea17-118">Optional query parameters</span></span>

<span data-ttu-id="bea17-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bea17-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bea17-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bea17-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bea17-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bea17-121">Request headers</span></span>

|<span data-ttu-id="bea17-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bea17-122">Name</span></span>|<span data-ttu-id="bea17-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bea17-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bea17-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bea17-124">Authorization</span></span>|<span data-ttu-id="bea17-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bea17-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bea17-127">Request body</span></span>

<span data-ttu-id="bea17-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bea17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bea17-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea17-129">Response</span></span>

<span data-ttu-id="bea17-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bea17-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bea17-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="bea17-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bea17-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bea17-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bea17-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bea17-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_datasource_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources
```
# <a name="c"></a>[<span data-ttu-id="bea17-134">C#</span><span class="sxs-lookup"><span data-stu-id="bea17-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-datasource-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bea17-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bea17-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-datasource-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bea17-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bea17-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-datasource-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bea17-137">Java</span><span class="sxs-lookup"><span data-stu-id="bea17-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-datasource-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bea17-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea17-138">Response</span></span>

<span data-ttu-id="bea17-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bea17-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.dataSource",
      "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
      "displayName": "String",
      "createdDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ]
}
```
