---
title: Список дополнительныхSources
description: Получите список дополнительных объектов dataSource, связанных с исходным собранием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5f9c08fe286be1dd983fa81a4b9ee9b61563b503
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446888"
---
# <a name="list-additionalsources"></a><span data-ttu-id="b00b6-103">Список дополнительныхSources</span><span class="sxs-lookup"><span data-stu-id="b00b6-103">List additionalSources</span></span>

<span data-ttu-id="b00b6-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b00b6-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b00b6-105">Получите список дополнительных объектов [dataSource,](../resources/ediscovery-datasource.md) связанных с исходным собранием.</span><span class="sxs-lookup"><span data-stu-id="b00b6-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="b00b6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b00b6-106">Permissions</span></span>

<span data-ttu-id="b00b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b00b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b00b6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b00b6-109">Permission type</span></span>|<span data-ttu-id="b00b6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b00b6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b00b6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b00b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b00b6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00b6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b00b6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b00b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b00b6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b00b6-114">Not supported.</span></span>|
|<span data-ttu-id="b00b6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b00b6-115">Application</span></span>|<span data-ttu-id="b00b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b00b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b00b6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b00b6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b00b6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b00b6-118">Optional query parameters</span></span>

<span data-ttu-id="b00b6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b00b6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b00b6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b00b6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b00b6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b00b6-121">Request headers</span></span>

|<span data-ttu-id="b00b6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b00b6-122">Name</span></span>|<span data-ttu-id="b00b6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b00b6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b00b6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b00b6-124">Authorization</span></span>|<span data-ttu-id="b00b6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b00b6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b00b6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b00b6-127">Request body</span></span>

<span data-ttu-id="b00b6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b00b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b00b6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00b6-129">Response</span></span>

<span data-ttu-id="b00b6-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b00b6-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b00b6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b00b6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b00b6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b00b6-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

### <a name="response"></a><span data-ttu-id="b00b6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b00b6-133">Response</span></span>

<span data-ttu-id="b00b6-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b00b6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
