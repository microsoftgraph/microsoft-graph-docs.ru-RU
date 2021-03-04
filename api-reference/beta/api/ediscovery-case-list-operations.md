---
title: Операции списка
description: Получите список caseOperations из объекта case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6f6cd402a88f0ce10e963cab0e3c0d94549f0dbd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447167"
---
# <a name="list-operations"></a><span data-ttu-id="d3a1f-103">Операции списка</span><span class="sxs-lookup"><span data-stu-id="d3a1f-103">List operations</span></span>

<span data-ttu-id="d3a1f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d3a1f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a1f-105">Получите список [caseOperations из](../resources/ediscovery-caseoperation.md) [объекта case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="d3a1f-105">Get the list of [caseOperations](../resources/ediscovery-caseoperation.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3a1f-106">Permissions</span></span>

<span data-ttu-id="d3a1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3a1f-109">Permission type</span></span>|<span data-ttu-id="d3a1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3a1f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3a1f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a1f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a1f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d3a1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3a1f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-114">Not supported.</span></span>|
|<span data-ttu-id="d3a1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3a1f-115">Application</span></span>|<span data-ttu-id="d3a1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3a1f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3a1f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3a1f-118">Optional query parameters</span></span>

<span data-ttu-id="d3a1f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d3a1f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d3a1f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a1f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3a1f-121">Request headers</span></span>

|<span data-ttu-id="d3a1f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d3a1f-122">Name</span></span>|<span data-ttu-id="d3a1f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d3a1f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3a1f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3a1f-124">Authorization</span></span>|<span data-ttu-id="d3a1f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a1f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3a1f-127">Request body</span></span>
<span data-ttu-id="d3a1f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a1f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3a1f-129">Response</span></span>

<span data-ttu-id="d3a1f-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3a1f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d3a1f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3a1f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3a1f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_caseoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations
```

### <a name="response"></a><span data-ttu-id="d3a1f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3a1f-133">Response</span></span>

<span data-ttu-id="d3a1f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3a1f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.caseOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
      "id": "41362b70-2b70-4136-702b-3641702b3641",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
