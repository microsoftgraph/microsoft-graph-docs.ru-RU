---
title: Получить хранителя
description: Ознакомьтесь с свойствами и отношениями объекта-хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 18fc6d6bb852b8615c3b30e34bd88789c026390d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946324"
---
# <a name="get-custodian"></a><span data-ttu-id="b60f6-103">Получить хранителя</span><span class="sxs-lookup"><span data-stu-id="b60f6-103">Get custodian</span></span>

<span data-ttu-id="b60f6-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b60f6-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b60f6-105">Ознакомьтесь с свойствами и отношениями [объекта-хранителя.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="b60f6-105">Read the properties and relationships of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b60f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b60f6-106">Permissions</span></span>

<span data-ttu-id="b60f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b60f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b60f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b60f6-109">Permission type</span></span>|<span data-ttu-id="b60f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b60f6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b60f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b60f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b60f6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b60f6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b60f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b60f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b60f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b60f6-114">Not supported.</span></span>|
|<span data-ttu-id="b60f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b60f6-115">Application</span></span>|<span data-ttu-id="b60f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b60f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b60f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b60f6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caesId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b60f6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b60f6-118">Optional query parameters</span></span>

<span data-ttu-id="b60f6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b60f6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b60f6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b60f6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b60f6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b60f6-121">Request headers</span></span>

|<span data-ttu-id="b60f6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b60f6-122">Name</span></span>|<span data-ttu-id="b60f6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b60f6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b60f6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b60f6-124">Authorization</span></span>|<span data-ttu-id="b60f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b60f6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b60f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b60f6-127">Request body</span></span>

<span data-ttu-id="b60f6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b60f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b60f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b60f6-129">Response</span></span>

<span data-ttu-id="b60f6-130">В случае успеха этот метод возвращает код отклика и `200 OK` [объект microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b60f6-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b60f6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b60f6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b60f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b60f6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b60f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b60f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```
# <a name="c"></a>[<span data-ttu-id="b60f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="b60f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b60f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b60f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b60f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b60f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b60f6-137">Java</span><span class="sxs-lookup"><span data-stu-id="b60f6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b60f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b60f6-138">Response</span></span>

<span data-ttu-id="b60f6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b60f6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": true,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T20:59:55.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
