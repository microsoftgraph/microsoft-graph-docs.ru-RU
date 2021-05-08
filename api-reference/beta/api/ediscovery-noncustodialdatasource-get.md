---
title: Получить noncustodialDataSource
description: Ознакомьтесь с свойствами и отношениями объекта noncustodialDataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3f943ad2390becfe50185203b278c731e24faad4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240948"
---
# <a name="get-noncustodialdatasource"></a><span data-ttu-id="257a3-103">Получить noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="257a3-103">Get noncustodialDataSource</span></span>

<span data-ttu-id="257a3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="257a3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="257a3-105">Ознакомьтесь с свойствами и отношениями [объекта noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="257a3-105">Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="257a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="257a3-106">Permissions</span></span>

<span data-ttu-id="257a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="257a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="257a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="257a3-109">Permission type</span></span>|<span data-ttu-id="257a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="257a3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="257a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="257a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="257a3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="257a3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="257a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="257a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="257a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="257a3-114">Not supported.</span></span>|
|<span data-ttu-id="257a3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="257a3-115">Application</span></span>|<span data-ttu-id="257a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="257a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="257a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="257a3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="257a3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="257a3-118">Optional query parameters</span></span>

<span data-ttu-id="257a3-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="257a3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="257a3-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="257a3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="257a3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="257a3-121">Request headers</span></span>

|<span data-ttu-id="257a3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="257a3-122">Name</span></span>|<span data-ttu-id="257a3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="257a3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="257a3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="257a3-124">Authorization</span></span>|<span data-ttu-id="257a3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="257a3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="257a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="257a3-127">Request body</span></span>

<span data-ttu-id="257a3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="257a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="257a3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="257a3-129">Response</span></span>

<span data-ttu-id="257a3-130">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="257a3-130">If successful, this method returns a `200 OK` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="257a3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="257a3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="257a3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="257a3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="257a3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="257a3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8b69818bf6af4f8a9dede428401c71e7
```
# <a name="c"></a>[<span data-ttu-id="257a3-134">C#</span><span class="sxs-lookup"><span data-stu-id="257a3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-noncustodialdatasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="257a3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="257a3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-noncustodialdatasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="257a3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="257a3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-noncustodialdatasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="257a3-137">Java</span><span class="sxs-lookup"><span data-stu-id="257a3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-noncustodialdatasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="257a3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="257a3-138">Response</span></span>

<span data-ttu-id="257a3-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="257a3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "Active",
    "lastModifiedDateTime": "2021-02-17T19:41:28.8714643Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "8b69818bf6af4f8a9dede428401c71e7",
    "displayName": null,
    "createdDateTime": "2021-02-17T19:41:22.958104Z",
    "applyHoldToSource": true
}
```
