---
title: Get sourceCollection
description: Ознакомьтесь с свойствами и отношениями объекта sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b10f29de6bbf61151f55aae2a37ac10ddf3ece86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446894"
---
# <a name="get-sourcecollection"></a><span data-ttu-id="2425f-103">Get sourceCollection</span><span class="sxs-lookup"><span data-stu-id="2425f-103">Get sourceCollection</span></span>

<span data-ttu-id="2425f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2425f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2425f-105">Ознакомьтесь с свойствами и отношениями [объекта sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="2425f-105">Read the properties and relationships of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2425f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2425f-106">Permissions</span></span>

<span data-ttu-id="2425f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2425f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2425f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2425f-109">Permission type</span></span>|<span data-ttu-id="2425f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2425f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2425f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2425f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2425f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2425f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="2425f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2425f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2425f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2425f-114">Not supported.</span></span>|
|<span data-ttu-id="2425f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2425f-115">Application</span></span>|<span data-ttu-id="2425f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2425f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2425f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2425f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2425f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2425f-118">Optional query parameters</span></span>

<span data-ttu-id="2425f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2425f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2425f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2425f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="2425f-121">Используйте для расширения операций набора `$expand` обзоров, источников хранителя и последней операции статистики оценки.</span><span class="sxs-lookup"><span data-stu-id="2425f-121">Use `$expand` to expand review set operations, custodian sources, and the last estimate statistics operation.</span></span>

```http
https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

## <a name="request-headers"></a><span data-ttu-id="2425f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2425f-122">Request headers</span></span>

|<span data-ttu-id="2425f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2425f-123">Name</span></span>|<span data-ttu-id="2425f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2425f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2425f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2425f-125">Authorization</span></span>|<span data-ttu-id="2425f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2425f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2425f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2425f-128">Request body</span></span>

<span data-ttu-id="2425f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2425f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2425f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2425f-130">Response</span></span>

<span data-ttu-id="2425f-131">В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2425f-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2425f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2425f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2425f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2425f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

### <a name="response"></a><span data-ttu-id="2425f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2425f-134">Response</span></span>

<span data-ttu-id="2425f-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2425f-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.onmicrosoft.com"
        }
    },
    "addToReviewSetOperation": {
        "createdDateTime": "2021-01-13T05:38:49.9186654Z",
        "completedDateTime": "2021-01-13T07:54:45.0007868Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "addToReviewSet",
        "id": "aef586b34d89405d802497658a14194f",
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": null,
                "userPrincipalName": "admin@contoso.com"
            }
        }
    },
    "lastEstimateStatisticsOperation": {
        "createdDateTime": "2021-01-12T21:53:50.7272654Z",
        "completedDateTime": "2021-01-12T21:54:49.5595543Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "f3db0382af0842eaa98c7dd59e7dace6",
        "indexedItemCount": 39598,
        "indexedItemsSize": 3760920737,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 1,
        "siteCount": 1,
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": "EDisco Admin",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    }
}
```
