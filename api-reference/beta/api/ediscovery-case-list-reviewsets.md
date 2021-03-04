---
title: List reviewSets
description: Получите ресурсы reviewSet из объекта case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: eb881a041ac890cb5c2c616cbf57189e26f8e272
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447161"
---
# <a name="list-reviewsets"></a><span data-ttu-id="5c039-103">List reviewSets</span><span class="sxs-lookup"><span data-stu-id="5c039-103">List reviewSets</span></span>

<span data-ttu-id="5c039-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5c039-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c039-105">Получите список [reviewSets из](../resources/ediscovery-reviewset.md) объекта [case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="5c039-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c039-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c039-106">Permissions</span></span>

<span data-ttu-id="5c039-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c039-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c039-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c039-109">Permission type</span></span>|<span data-ttu-id="5c039-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c039-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c039-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c039-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c039-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c039-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5c039-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c039-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c039-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c039-114">Not supported.</span></span>|
|<span data-ttu-id="5c039-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c039-115">Application</span></span>|<span data-ttu-id="5c039-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c039-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c039-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c039-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c039-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c039-118">Optional query parameters</span></span>

<span data-ttu-id="5c039-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5c039-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c039-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c039-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c039-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c039-121">Request headers</span></span>

|<span data-ttu-id="5c039-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5c039-122">Name</span></span>|<span data-ttu-id="5c039-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c039-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c039-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c039-124">Authorization</span></span>|<span data-ttu-id="5c039-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c039-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c039-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c039-127">Request body</span></span>

<span data-ttu-id="5c039-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c039-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c039-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c039-129">Response</span></span>

<span data-ttu-id="5c039-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c039-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c039-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c039-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c039-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c039-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```

### <a name="response"></a><span data-ttu-id="5c039-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c039-133">Response</span></span>

<span data-ttu-id="5c039-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c039-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.reviewSet)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```
