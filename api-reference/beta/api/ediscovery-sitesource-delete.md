---
title: Удаление siteSource
description: Удаление объекта siteSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5948064b4fffa2af858b3e6bfb92eb02f991c784
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446927"
---
# <a name="delete-sitesource"></a><span data-ttu-id="d0228-103">Удаление siteSource</span><span class="sxs-lookup"><span data-stu-id="d0228-103">Delete siteSource</span></span>

<span data-ttu-id="d0228-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d0228-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0228-105">Удаление [объекта siteSource.](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="d0228-105">Delete a [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0228-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0228-106">Permissions</span></span>

<span data-ttu-id="d0228-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0228-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0228-109">Permission type</span></span>|<span data-ttu-id="d0228-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0228-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0228-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0228-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0228-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0228-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d0228-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0228-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0228-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0228-114">Not supported.</span></span>|
|<span data-ttu-id="d0228-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0228-115">Application</span></span>|<span data-ttu-id="d0228-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0228-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0228-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0228-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="d0228-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0228-118">Request headers</span></span>

|<span data-ttu-id="d0228-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d0228-119">Name</span></span>|<span data-ttu-id="d0228-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d0228-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0228-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0228-121">Authorization</span></span>|<span data-ttu-id="d0228-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0228-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0228-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0228-124">Request body</span></span>

<span data-ttu-id="d0228-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0228-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0228-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0228-126">Response</span></span>

<span data-ttu-id="d0228-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0228-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d0228-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0228-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0228-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0228-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0228-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0228-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sitesource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```
# <a name="c"></a>[<span data-ttu-id="d0228-131">C#</span><span class="sxs-lookup"><span data-stu-id="d0228-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0228-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0228-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0228-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0228-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0228-134">Java</span><span class="sxs-lookup"><span data-stu-id="d0228-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0228-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0228-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
