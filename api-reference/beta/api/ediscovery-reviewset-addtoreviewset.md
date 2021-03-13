---
title: 'reviewSet: addToReviewSet'
description: Начните процесс добавления коллекции из служб Microsoft 365 в набор отзывов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a1002d8b322876f753f424a1bffeb7ef8a278b35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772915"
---
# <a name="reviewset-addtoreviewset"></a><span data-ttu-id="e797d-103">reviewSet: addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="e797d-103">reviewSet: addToReviewSet</span></span>

<span data-ttu-id="e797d-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e797d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e797d-105">Начните процесс добавления коллекции из служб Microsoft 365 в набор отзывов.</span><span class="sxs-lookup"><span data-stu-id="e797d-105">Start the process of adding a collection from Microsoft 365 services to a review set.</span></span> <span data-ttu-id="e797d-106">После создания операции можно получить состояние операции путем получения параметра `Location` из заглавных параметров ответа.</span><span class="sxs-lookup"><span data-stu-id="e797d-106">After the operation is created, you can get the status of the operation by retrieving the `Location` parameter from the response headers.</span></span> <span data-ttu-id="e797d-107">Расположение предоставляет URL-адрес, который возвращает [случайExportOperation](../resources/ediscovery-caseexportoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e797d-107">The location provides a URL that will return a [caseExportOperation](../resources/ediscovery-caseexportoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e797d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e797d-108">Permissions</span></span>

<span data-ttu-id="e797d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e797d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e797d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e797d-111">Permission type</span></span>|<span data-ttu-id="e797d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e797d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e797d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e797d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e797d-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e797d-114">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e797d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e797d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e797d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e797d-116">Not supported.</span></span>|
|<span data-ttu-id="e797d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e797d-117">Application</span></span>|<span data-ttu-id="e797d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e797d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e797d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e797d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
```

## <a name="request-headers"></a><span data-ttu-id="e797d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e797d-120">Request headers</span></span>

|<span data-ttu-id="e797d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e797d-121">Name</span></span>|<span data-ttu-id="e797d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e797d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e797d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e797d-123">Authorization</span></span>|<span data-ttu-id="e797d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e797d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e797d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e797d-126">Content-Type</span></span>|<span data-ttu-id="e797d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e797d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e797d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e797d-129">Request body</span></span>

<span data-ttu-id="e797d-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e797d-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e797d-131">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e797d-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e797d-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="e797d-132">Parameter</span></span>|<span data-ttu-id="e797d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e797d-133">Type</span></span>|<span data-ttu-id="e797d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e797d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e797d-135">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e797d-135">sourceCollection</span></span>|[<span data-ttu-id="e797d-136">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="e797d-136">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourcecollection.md)|<span data-ttu-id="e797d-137">ID **источникаCollection**.</span><span class="sxs-lookup"><span data-stu-id="e797d-137">The ID of the **sourceCollection**.</span></span>|
|<span data-ttu-id="e797d-138">additionalData</span><span class="sxs-lookup"><span data-stu-id="e797d-138">additionalData</span></span>|[<span data-ttu-id="e797d-139">microsoft.graph.ediscovery.dataCollectionScope</span><span class="sxs-lookup"><span data-stu-id="e797d-139">microsoft.graph.ediscovery.dataCollectionScope</span></span>](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|<span data-ttu-id="e797d-140">**DataCollectionScope,** который будет включен в коллекцию.</span><span class="sxs-lookup"><span data-stu-id="e797d-140">The **dataCollectionScope** that will be included with the collection.</span></span>|

## <a name="response"></a><span data-ttu-id="e797d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e797d-141">Response</span></span>

<span data-ttu-id="e797d-142">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e797d-142">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e797d-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="e797d-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e797d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e797d-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e797d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e797d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_addtoreviewset"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet
Content-Type: application/json
Content-length: 531

{
    "sourceCollection": {
        "id": "1a9b4145d8f84e39bc45a7f68c5c5119"
    },
    "additionalData": "linkedFiles"
}
```
# <a name="c"></a>[<span data-ttu-id="e797d-146">C#</span><span class="sxs-lookup"><span data-stu-id="e797d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-addtoreviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e797d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e797d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-addtoreviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e797d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e797d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-addtoreviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e797d-149">Java</span><span class="sxs-lookup"><span data-stu-id="e797d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-addtoreviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e797d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e797d-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
