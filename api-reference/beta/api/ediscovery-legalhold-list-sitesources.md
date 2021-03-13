---
title: Список legalHold siteSources
description: Получите список objecs siteSource, связанных с юридическим удержанием.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 313d47528809eea3ba2cc7e27f7e73114195f992
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773062"
---
# <a name="list-legalhold-sitesources"></a><span data-ttu-id="fdd6c-103">Список legalHold siteSources</span><span class="sxs-lookup"><span data-stu-id="fdd6c-103">List legalHold siteSources</span></span>

<span data-ttu-id="fdd6c-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="fdd6c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd6c-105">Получите список [objecs siteSource,](../resources/ediscovery-sitesource.md) связанных с юридическим удержанием.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-105">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdd6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd6c-106">Permissions</span></span>

<span data-ttu-id="fdd6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions- reference).</span><span class="sxs-lookup"><span data-stu-id="fdd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions- reference).</span></span>

|<span data-ttu-id="fdd6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdd6c-109">Permission type</span></span>|<span data-ttu-id="fdd6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdd6c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdd6c-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdd6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdd6c-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd6c-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="fdd6c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdd6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdd6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-114">Not supported.</span></span>|
|<span data-ttu-id="fdd6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdd6c-115">Application</span></span>|<span data-ttu-id="fdd6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdd6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdd6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdd6c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fdd6c-118">Optional query parameters</span></span>

<span data-ttu-id="fdd6c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fdd6c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fdd6c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdd6c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdd6c-121">Request headers</span></span>

|<span data-ttu-id="fdd6c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fdd6c-122">Name</span></span>|<span data-ttu-id="fdd6c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fdd6c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fdd6c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdd6c-124">Authorization</span></span>|<span data-ttu-id="fdd6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdd6c-127">Request body</span></span>

<span data-ttu-id="fdd6c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdd6c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd6c-129">Response</span></span>

<span data-ttu-id="fdd6c-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fdd6c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="fdd6c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fdd6c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdd6c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fdd6c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdd6c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources
```
# <a name="c"></a>[<span data-ttu-id="fdd6c-134">C#</span><span class="sxs-lookup"><span data-stu-id="fdd6c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdd6c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdd6c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdd6c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdd6c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdd6c-137">Java</span><span class="sxs-lookup"><span data-stu-id="fdd6c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fdd6c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdd6c-138">Response</span></span>

<span data-ttu-id="fdd6c-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fdd6c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "43aab990-183e-4593-b772-578bb129e89b",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        },
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "e87b37ac-fad4-471b-9dd8-0e16000a3554",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
