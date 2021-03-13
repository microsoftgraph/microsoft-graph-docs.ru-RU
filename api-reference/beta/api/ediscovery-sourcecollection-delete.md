---
title: Удаление sourceCollection
description: Удаление объекта sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 13380114c2d2e7a1f0ff4d1f612a411d8efad6f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772746"
---
# <a name="delete-sourcecollection"></a><span data-ttu-id="d2b43-103">Удаление sourceCollection</span><span class="sxs-lookup"><span data-stu-id="d2b43-103">Delete sourceCollection</span></span>

<span data-ttu-id="d2b43-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d2b43-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b43-105">Удаление [объекта sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="d2b43-105">Delete a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2b43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2b43-106">Permissions</span></span>

<span data-ttu-id="d2b43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2b43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2b43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2b43-109">Permission type</span></span>|<span data-ttu-id="d2b43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2b43-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2b43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2b43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2b43-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2b43-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d2b43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2b43-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2b43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2b43-114">Not supported.</span></span>|
|<span data-ttu-id="d2b43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2b43-115">Application</span></span>|<span data-ttu-id="d2b43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2b43-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2b43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2b43-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="d2b43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2b43-118">Request headers</span></span>

|<span data-ttu-id="d2b43-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2b43-119">Name</span></span>|<span data-ttu-id="d2b43-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2b43-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2b43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2b43-121">Authorization</span></span>|<span data-ttu-id="d2b43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2b43-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2b43-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2b43-124">Request body</span></span>

<span data-ttu-id="d2b43-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2b43-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2b43-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2b43-126">Response</span></span>

<span data-ttu-id="d2b43-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2b43-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d2b43-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2b43-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2b43-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2b43-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d2b43-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2b43-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sourcecollection"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```
# <a name="c"></a>[<span data-ttu-id="d2b43-131">C#</span><span class="sxs-lookup"><span data-stu-id="d2b43-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2b43-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2b43-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2b43-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2b43-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2b43-134">Java</span><span class="sxs-lookup"><span data-stu-id="d2b43-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2b43-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2b43-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
