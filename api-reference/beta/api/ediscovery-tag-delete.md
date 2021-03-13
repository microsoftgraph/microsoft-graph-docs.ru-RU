---
title: Удаление тега
description: Удаление объекта тега.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8c21df5939cde9b707dd913dbfa383ba1e950d53
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776461"
---
# <a name="delete-tag"></a><span data-ttu-id="4c301-103">Удаление тега</span><span class="sxs-lookup"><span data-stu-id="4c301-103">Delete tag</span></span>

<span data-ttu-id="4c301-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4c301-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c301-105">Удаление объекта [тега.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="4c301-105">Delete a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c301-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c301-106">Permissions</span></span>

<span data-ttu-id="4c301-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c301-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c301-109">Permission type</span></span>|<span data-ttu-id="4c301-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c301-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c301-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c301-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c301-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c301-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4c301-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c301-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c301-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c301-114">Not supported.</span></span>|
|<span data-ttu-id="4c301-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c301-115">Application</span></span>|<span data-ttu-id="4c301-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c301-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c301-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c301-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/tags/{tagId}?forcedelete=true
```

## <a name="query-parameters"></a><span data-ttu-id="4c301-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4c301-118">Query parameters</span></span>

<span data-ttu-id="4c301-119">В URL-адресе запроса укайте следующий необходимый параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="4c301-119">In the request URL, provide the following required query parameter.</span></span>

| <span data-ttu-id="4c301-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c301-120">Parameter</span></span>     | <span data-ttu-id="4c301-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c301-121">Type</span></span>    | <span data-ttu-id="4c301-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c301-122">Description</span></span>                                                                              |
|:--------------|:--------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="4c301-123">forcedelete</span><span class="sxs-lookup"><span data-stu-id="4c301-123">forcedelete</span></span>   | <span data-ttu-id="4c301-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c301-124">Boolean</span></span> | <span data-ttu-id="4c301-125">Если задайте true, тег и дети будут удалены, если ложные, а тег имеет детей, удаление не удастся.</span><span class="sxs-lookup"><span data-stu-id="4c301-125">If set to true, the tag and children will be deleted, if false, and the tag has children, the delete will fail.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4c301-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c301-126">Request headers</span></span>

|<span data-ttu-id="4c301-127">Имя</span><span class="sxs-lookup"><span data-stu-id="4c301-127">Name</span></span>|<span data-ttu-id="4c301-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4c301-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4c301-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c301-129">Authorization</span></span>|<span data-ttu-id="4c301-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c301-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c301-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c301-132">Request body</span></span>

<span data-ttu-id="4c301-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c301-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c301-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c301-134">Response</span></span>

<span data-ttu-id="4c301-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c301-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4c301-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c301-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c301-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c301-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4c301-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c301-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tag"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/9985bd266f2f459cbebc81522734b452?forcedelete=true
```
# <a name="c"></a>[<span data-ttu-id="4c301-139">C#</span><span class="sxs-lookup"><span data-stu-id="4c301-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c301-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c301-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c301-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c301-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c301-142">Java</span><span class="sxs-lookup"><span data-stu-id="4c301-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c301-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c301-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
