---
title: 'reviewSetQuery: applyTags'
description: Применяйте теги к документам, которые соответствуют указанному запросу.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2c3f41d1fbe9851babc582c1f21c9f9673d53541
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446954"
---
# <a name="reviewsetquery-applytags"></a><span data-ttu-id="5ab61-103">reviewSetQuery: applyTags</span><span class="sxs-lookup"><span data-stu-id="5ab61-103">reviewSetQuery: applyTags</span></span>

<span data-ttu-id="5ab61-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5ab61-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="5ab61-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ab61-105">Permissions</span></span>

<span data-ttu-id="5ab61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ab61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ab61-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ab61-108">Permission type</span></span>|<span data-ttu-id="5ab61-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ab61-109">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ab61-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ab61-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5ab61-111">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ab61-111">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5ab61-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ab61-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ab61-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ab61-113">Not supported.</span></span>|
|<span data-ttu-id="5ab61-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ab61-114">Application</span></span>|<span data-ttu-id="5ab61-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ab61-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ab61-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ab61-116">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewSetId}/queries/{reviewSetQueryId}/applyTags
```

## <a name="request-headers"></a><span data-ttu-id="5ab61-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ab61-117">Request headers</span></span>

|<span data-ttu-id="5ab61-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5ab61-118">Name</span></span>|<span data-ttu-id="5ab61-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5ab61-119">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ab61-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ab61-120">Authorization</span></span>|<span data-ttu-id="5ab61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ab61-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ab61-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ab61-123">Content-Type</span></span>|<span data-ttu-id="5ab61-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ab61-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ab61-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ab61-126">Request body</span></span>

<span data-ttu-id="5ab61-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ab61-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5ab61-128">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5ab61-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5ab61-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="5ab61-129">Parameter</span></span>|<span data-ttu-id="5ab61-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5ab61-130">Type</span></span>|<span data-ttu-id="5ab61-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ab61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ab61-132">tagsToAdd</span><span class="sxs-lookup"><span data-stu-id="5ab61-132">tagsToAdd</span></span>|<span data-ttu-id="5ab61-133">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="5ab61-133">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="5ab61-134">ID-теги для добавления в документы, соответствующие запросу.</span><span class="sxs-lookup"><span data-stu-id="5ab61-134">IDs of tags to add to the documents that match the query.</span></span>|
|<span data-ttu-id="5ab61-135">tagsToRemove</span><span class="sxs-lookup"><span data-stu-id="5ab61-135">tagsToRemove</span></span>|<span data-ttu-id="5ab61-136">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="5ab61-136">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="5ab61-137">ID-теги для удаления из документов, которые соответствуют запросу.</span><span class="sxs-lookup"><span data-stu-id="5ab61-137">IDs of tags to remove from the documents that match the query.</span></span>|

## <a name="response"></a><span data-ttu-id="5ab61-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ab61-138">Response</span></span>

<span data-ttu-id="5ab61-139">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="5ab61-139">If successful, this action returns a `202 Accepted` response code.</span></span>

<span data-ttu-id="5ab61-140">Если операция по тегированию успешно запущена, это действие возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="5ab61-140">If the tagging operation is started successfully, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="5ab61-141">В ответе также будет содержаться `Location` заглавный загот, содержащий расположение [тегаOperation,](../resources/ediscovery-tagOperation.md) созданного для обработки тегов.</span><span class="sxs-lookup"><span data-stu-id="5ab61-141">The response will also contain a `Location` header, which contains the location of the [tagOperation](../resources/ediscovery-tagOperation.md) that was created to handle the tagging.</span></span> <span data-ttu-id="5ab61-142">Проверьте состояние операции по тегированию, сделав запрос GET в расположение, после успешного завершения состояние [изменится](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) на `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="5ab61-142">Check the status of the tagging operation by making a GET request to the location, when successfully completed, the [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) will change to `succeeded`.</span></span>

## <a name="examples"></a><span data-ttu-id="5ab61-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ab61-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ab61-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ab61-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reviewsetquery_applytags"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/reviewsets/6c95c2a6-31fa-45a8-93ef-dd4531974783/queries/b4798d14-748d-468e-a1ec-96a2b1d49677/applyTags
Content-Type: application/json
Content-length: 778

{
    "tagsToAdd": [
        {
            "id": "b4798d14-748d-468e-a1ec-96a2b1d49677"
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="5ab61-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ab61-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 56c9dd8b-d8f7-59ae-6733-38191862c9c9,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/operations('d77f7933e88842bab3221e280be9dc0b'),
request-id: c2397a81-e9c2-4851-b669-d87e0751e45a
```
