---
title: Удаление unifiedGroupSource
description: Удаление объекта unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7e58bd2da85d980944b7df840cac95ed0a5dd6b1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446822"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="c74fc-103">Удаление unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="c74fc-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="c74fc-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c74fc-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c74fc-105">Удаление [объекта unifiedGroupSource.](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="c74fc-105">Delete a [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c74fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c74fc-106">Permissions</span></span>

<span data-ttu-id="c74fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c74fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c74fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c74fc-109">Permission type</span></span>|<span data-ttu-id="c74fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c74fc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c74fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c74fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c74fc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c74fc-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c74fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c74fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c74fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c74fc-114">Not supported.</span></span>|
|<span data-ttu-id="c74fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c74fc-115">Application</span></span>|<span data-ttu-id="c74fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c74fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c74fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c74fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="c74fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c74fc-118">Request headers</span></span>

|<span data-ttu-id="c74fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c74fc-119">Name</span></span>|<span data-ttu-id="c74fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c74fc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c74fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c74fc-121">Authorization</span></span>|<span data-ttu-id="c74fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c74fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c74fc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c74fc-124">Request body</span></span>

<span data-ttu-id="c74fc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c74fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c74fc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c74fc-126">Response</span></span>

<span data-ttu-id="c74fc-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c74fc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c74fc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c74fc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c74fc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c74fc-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c74fc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c74fc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```
# <a name="c"></a>[<span data-ttu-id="c74fc-131">C#</span><span class="sxs-lookup"><span data-stu-id="c74fc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c74fc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c74fc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c74fc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c74fc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c74fc-134">Java</span><span class="sxs-lookup"><span data-stu-id="c74fc-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c74fc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c74fc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
