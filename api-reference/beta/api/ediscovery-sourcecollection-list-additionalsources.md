---
title: Список дополнительныхSources
description: Получите список дополнительных объектов dataSource, связанных с исходным собранием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e254383ebe5fd9eb4930e7089e095a3669e77959
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080313"
---
# <a name="list-additionalsources"></a><span data-ttu-id="bc948-103">Список дополнительныхSources</span><span class="sxs-lookup"><span data-stu-id="bc948-103">List additionalSources</span></span>

<span data-ttu-id="bc948-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bc948-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc948-105">Получите список дополнительных объектов [dataSource,](../resources/ediscovery-datasource.md) связанных с исходным собранием.</span><span class="sxs-lookup"><span data-stu-id="bc948-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc948-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc948-106">Permissions</span></span>

<span data-ttu-id="bc948-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc948-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc948-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc948-109">Permission type</span></span>|<span data-ttu-id="bc948-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc948-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc948-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc948-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc948-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc948-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bc948-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc948-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc948-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc948-114">Not supported.</span></span>|
|<span data-ttu-id="bc948-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc948-115">Application</span></span>|<span data-ttu-id="bc948-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc948-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc948-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc948-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc948-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc948-118">Optional query parameters</span></span>

<span data-ttu-id="bc948-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bc948-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bc948-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bc948-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc948-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc948-121">Request headers</span></span>

|<span data-ttu-id="bc948-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bc948-122">Name</span></span>|<span data-ttu-id="bc948-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bc948-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bc948-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc948-124">Authorization</span></span>|<span data-ttu-id="bc948-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc948-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc948-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc948-127">Request body</span></span>

<span data-ttu-id="bc948-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc948-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc948-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc948-129">Response</span></span>

<span data-ttu-id="bc948-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bc948-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc948-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="bc948-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc948-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc948-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bc948-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc948-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_datasource_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```
# <a name="c"></a>[<span data-ttu-id="bc948-134">C#</span><span class="sxs-lookup"><span data-stu-id="bc948-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-datasource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc948-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc948-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-datasource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc948-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc948-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-datasource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc948-137">Java</span><span class="sxs-lookup"><span data-stu-id="bc948-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-datasource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bc948-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc948-138">Response</span></span>

> <span data-ttu-id="bc948-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bc948-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
