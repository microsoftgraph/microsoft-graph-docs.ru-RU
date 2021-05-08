---
title: 'noncustodialDataSource: release'
description: Освобождает источник данных, не в отношении хранения, из дела.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b8839fe08dc74fe03c2ff2f0dc09d8c14865a297
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240906"
---
# <a name="noncustodialdatasource-release"></a><span data-ttu-id="3cb0e-103">noncustodialDataSource: release</span><span class="sxs-lookup"><span data-stu-id="3cb0e-103">noncustodialDataSource: release</span></span>

<span data-ttu-id="3cb0e-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3cb0e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb0e-105">Освобождает источник данных, не в отношении хранения, из дела.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-105">Releases the non-custodial data source from the case.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb0e-106">Permissions</span></span>

<span data-ttu-id="3cb0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb0e-109">Permission type</span></span>|<span data-ttu-id="3cb0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb0e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb0e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3cb0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cb0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-114">Not supported.</span></span>|
|<span data-ttu-id="3cb0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cb0e-115">Application</span></span>|<span data-ttu-id="3cb0e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/Release
```

## <a name="request-headers"></a><span data-ttu-id="3cb0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cb0e-118">Request headers</span></span>

|<span data-ttu-id="3cb0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3cb0e-119">Name</span></span>|<span data-ttu-id="3cb0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb0e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cb0e-121">Authorization</span></span>|<span data-ttu-id="3cb0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb0e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cb0e-124">Request body</span></span>

<span data-ttu-id="3cb0e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb0e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb0e-126">Response</span></span>

<span data-ttu-id="3cb0e-127">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-127">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3cb0e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3cb0e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cb0e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cb0e-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cb0e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb0e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "noncustodialdatasource_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release
```
# <a name="c"></a>[<span data-ttu-id="3cb0e-131">C#</span><span class="sxs-lookup"><span data-stu-id="3cb0e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/noncustodialdatasource-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cb0e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb0e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/noncustodialdatasource-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cb0e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cb0e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/noncustodialdatasource-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cb0e-134">Java</span><span class="sxs-lookup"><span data-stu-id="3cb0e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/noncustodialdatasource-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cb0e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb0e-135">Response</span></span>

<span data-ttu-id="3cb0e-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3cb0e-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
