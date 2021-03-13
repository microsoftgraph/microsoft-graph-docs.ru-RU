---
title: List reviewSets
description: Получите ресурсы reviewSet из объекта case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1ef80d6801cad9405d4089c548ef8ad93e0bd794
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776650"
---
# <a name="list-reviewsets"></a><span data-ttu-id="bd014-103">List reviewSets</span><span class="sxs-lookup"><span data-stu-id="bd014-103">List reviewSets</span></span>

<span data-ttu-id="bd014-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bd014-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd014-105">Получите список [reviewSets из](../resources/ediscovery-reviewset.md) объекта [case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="bd014-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd014-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd014-106">Permissions</span></span>

<span data-ttu-id="bd014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd014-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd014-109">Permission type</span></span>|<span data-ttu-id="bd014-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd014-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd014-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd014-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd014-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd014-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bd014-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd014-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd014-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd014-114">Not supported.</span></span>|
|<span data-ttu-id="bd014-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd014-115">Application</span></span>|<span data-ttu-id="bd014-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd014-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd014-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd014-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd014-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd014-118">Optional query parameters</span></span>

<span data-ttu-id="bd014-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bd014-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bd014-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bd014-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd014-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd014-121">Request headers</span></span>

|<span data-ttu-id="bd014-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bd014-122">Name</span></span>|<span data-ttu-id="bd014-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bd014-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bd014-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd014-124">Authorization</span></span>|<span data-ttu-id="bd014-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd014-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd014-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd014-127">Request body</span></span>

<span data-ttu-id="bd014-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd014-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd014-129">Response</span></span>

<span data-ttu-id="bd014-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bd014-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd014-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd014-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd014-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd014-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bd014-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd014-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```
# <a name="c"></a>[<span data-ttu-id="bd014-134">C#</span><span class="sxs-lookup"><span data-stu-id="bd014-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd014-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd014-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd014-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd014-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd014-137">Java</span><span class="sxs-lookup"><span data-stu-id="bd014-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd014-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd014-138">Response</span></span>

<span data-ttu-id="bd014-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd014-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
