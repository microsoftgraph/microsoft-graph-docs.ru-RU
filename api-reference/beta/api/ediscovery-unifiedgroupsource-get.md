---
title: Get unifiedGroupSource
description: Ознакомьтесь с свойствами и отношениями объекта unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 74fa278f9de4df399a6b016067050499c5f4ce6a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446825"
---
# <a name="get-unifiedgroupsource"></a><span data-ttu-id="1803f-103">Get unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="1803f-103">Get unifiedGroupSource</span></span>

<span data-ttu-id="1803f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1803f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1803f-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="1803f-105">Read the properties and relationships of a [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1803f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1803f-106">Permissions</span></span>

<span data-ttu-id="1803f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1803f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1803f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1803f-109">Permission type</span></span>|<span data-ttu-id="1803f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1803f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1803f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1803f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1803f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1803f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1803f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1803f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1803f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1803f-114">Not supported.</span></span>|
|<span data-ttu-id="1803f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1803f-115">Application</span></span>|<span data-ttu-id="1803f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1803f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1803f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1803f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1803f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1803f-118">Optional query parameters</span></span>

<span data-ttu-id="1803f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1803f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1803f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1803f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1803f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1803f-121">Request headers</span></span>

|<span data-ttu-id="1803f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1803f-122">Name</span></span>|<span data-ttu-id="1803f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1803f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1803f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1803f-124">Authorization</span></span>|<span data-ttu-id="1803f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1803f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1803f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1803f-127">Request body</span></span>

<span data-ttu-id="1803f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1803f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1803f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1803f-129">Response</span></span>

<span data-ttu-id="1803f-130">В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1803f-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1803f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1803f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1803f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1803f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1803f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1803f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```
# <a name="c"></a>[<span data-ttu-id="1803f-134">C#</span><span class="sxs-lookup"><span data-stu-id="1803f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1803f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1803f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1803f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1803f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1803f-137">Java</span><span class="sxs-lookup"><span data-stu-id="1803f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1803f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1803f-138">Response</span></span>

<span data-ttu-id="1803f-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1803f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "displayName": "Developers group",
    "createdDateTime": "2020-10-27T15:14:11.0048392Z",
    "id": "33434233-3030-3739-3043-393039324633",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "Megan Bowen"
        }
    }
}
```
