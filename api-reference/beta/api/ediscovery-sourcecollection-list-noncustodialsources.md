---
title: Список noncustodialSources
description: Получите ресурсы noncustodialDataSource из свойства навигации noncustodialSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7c553c00397f128a105eddd4d253d639706392c5
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080818"
---
# <a name="list-noncustodialsources"></a><span data-ttu-id="a419b-103">Список noncustodialSources</span><span class="sxs-lookup"><span data-stu-id="a419b-103">List noncustodialSources</span></span>

<span data-ttu-id="a419b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a419b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a419b-105">Получите список [noncustodialDataSource,](../resources/ediscovery-noncustodialdatasource.md) связанный с [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a419b-105">Get a list of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) associated with a [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="a419b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a419b-106">Permissions</span></span>

<span data-ttu-id="a419b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a419b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a419b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a419b-109">Permission type</span></span>|<span data-ttu-id="a419b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a419b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a419b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a419b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a419b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a419b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a419b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a419b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a419b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a419b-114">Not supported.</span></span>|
|<span data-ttu-id="a419b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a419b-115">Application</span></span>|<span data-ttu-id="a419b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a419b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a419b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a419b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a419b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a419b-118">Optional query parameters</span></span>

<span data-ttu-id="a419b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a419b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a419b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a419b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a419b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a419b-121">Request headers</span></span>

|<span data-ttu-id="a419b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a419b-122">Name</span></span>|<span data-ttu-id="a419b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a419b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a419b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a419b-124">Authorization</span></span>|<span data-ttu-id="a419b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a419b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a419b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a419b-127">Request body</span></span>

<span data-ttu-id="a419b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a419b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a419b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a419b-129">Response</span></span>

<span data-ttu-id="a419b-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a419b-130">If successful, this method returns a `200 OK` response code and a collection of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a419b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a419b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a419b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a419b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/noncustodialSources
```

### <a name="response"></a><span data-ttu-id="a419b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a419b-133">Response</span></span>

> <span data-ttu-id="a419b-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a419b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
