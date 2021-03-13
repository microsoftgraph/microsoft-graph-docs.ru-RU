---
title: 'sourceCollection: estimateStatistics'
description: Выполняет оценку коллекции исходных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2ae6b7363bdb1be34e38dd7f5502962fc920808d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772711"
---
# <a name="sourcecollection-estimatestatistics"></a><span data-ttu-id="951f2-103">sourceCollection: estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="951f2-103">sourceCollection: estimateStatistics</span></span>

<span data-ttu-id="951f2-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="951f2-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="951f2-105">Запустите оценку количества электронных писем и документов в коллекции исходных данных.</span><span class="sxs-lookup"><span data-stu-id="951f2-105">Run an estimate of the number of emails and documents in the source collection.</span></span> <span data-ttu-id="951f2-106">Дополнительные сведения о исходных коллекциях (также известных как поиски в eDiscovery) см. в примере Сбор данных по делу в [advanced eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="951f2-106">To learn more about source collections (also known as searches in eDiscovery), see [Collect data for a case in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/collecting-data-for-ediscovery).</span></span>

## <a name="permissions"></a><span data-ttu-id="951f2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="951f2-107">Permissions</span></span>

<span data-ttu-id="951f2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="951f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="951f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="951f2-110">Permission type</span></span>|<span data-ttu-id="951f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="951f2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="951f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="951f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="951f2-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="951f2-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="951f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="951f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="951f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="951f2-115">Not supported.</span></span>|
|<span data-ttu-id="951f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="951f2-116">Application</span></span>|<span data-ttu-id="951f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="951f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="951f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="951f2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```

## <a name="request-headers"></a><span data-ttu-id="951f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="951f2-119">Request headers</span></span>

|<span data-ttu-id="951f2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="951f2-120">Name</span></span>|<span data-ttu-id="951f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="951f2-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="951f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="951f2-122">Authorization</span></span>|<span data-ttu-id="951f2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="951f2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="951f2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="951f2-125">Request body</span></span>

<span data-ttu-id="951f2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="951f2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="951f2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="951f2-127">Response</span></span>

<span data-ttu-id="951f2-128">Если оценка успешно запущена, это действие возвращает код `202 Accepted` ответа.</span><span class="sxs-lookup"><span data-stu-id="951f2-128">If the estimate is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="951f2-129">В ответе также будет содержаться `Location` заглавный загот, содержащий расположение оценкиStatisticsOperation, созданной для обработки оценки. [](../resources/ediscovery-estimatestatisticsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="951f2-129">The response will also contain a `Location` header, which contains the location of the [estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) that was created to handle the estimate.</span></span> <span data-ttu-id="951f2-130">Проверьте состояние операции оценки, сделав запрос GET в расположение, после успешного завершения состояние [изменится](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) на `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="951f2-130">Check the status of the estimate operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="951f2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="951f2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="951f2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="951f2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="951f2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="951f2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollection_estimatestatistics"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics
```
# <a name="c"></a>[<span data-ttu-id="951f2-134">C#</span><span class="sxs-lookup"><span data-stu-id="951f2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollection-estimatestatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="951f2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="951f2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollection-estimatestatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="951f2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="951f2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollection-estimatestatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="951f2-137">Java</span><span class="sxs-lookup"><span data-stu-id="951f2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollection-estimatestatistics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="951f2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="951f2-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: private
client-request-id: af32de50-99d9-e3a8-371b-a4f366cc78e7
content-length: 0
content-type: text/plain
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/operations/82edd40e182a464fa02c24a36fa94873
request-id: e890176f-640f-4222-9cd8-be26e71c5e5d
```
