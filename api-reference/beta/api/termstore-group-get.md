---
title: Получить группу termStore
description: Ознакомьтесь с свойствами и отношениями группового объекта.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 8f36e8b6b2e03ed9a05294b35736dbbb1b0dd578
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53458971"
---
# <a name="get-termstore-group"></a><span data-ttu-id="c8dd8-103">Получить группу termStore</span><span class="sxs-lookup"><span data-stu-id="c8dd8-103">Get termStore group</span></span>
<span data-ttu-id="c8dd8-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="c8dd8-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8dd8-105">Ознакомьтесь с свойствами и отношениями объекта группы [терминов](../resources/termstore-group.md) store.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8dd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8dd8-106">Permissions</span></span>
<span data-ttu-id="c8dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8dd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8dd8-109">Permission type</span></span>|<span data-ttu-id="c8dd8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8dd8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8dd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8dd8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8dd8-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8dd8-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="c8dd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8dd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8dd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-114">Not supported.</span></span>    |
|<span data-ttu-id="c8dd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8dd8-115">Application</span></span> | <span data-ttu-id="c8dd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="c8dd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8dd8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{group-id}
GET /sites/{site-id}/termStore/groups/{group-id}
```

## <a name="request-headers"></a><span data-ttu-id="c8dd8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8dd8-118">Request headers</span></span>
|<span data-ttu-id="c8dd8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c8dd8-119">Name</span></span>|<span data-ttu-id="c8dd8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c8dd8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c8dd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8dd8-121">Authorization</span></span>|<span data-ttu-id="c8dd8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8dd8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8dd8-124">Request body</span></span>
<span data-ttu-id="c8dd8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8dd8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8dd8-126">Response</span></span>

<span data-ttu-id="c8dd8-127">В случае успеха этот метод возвращает код отклика и `200 OK` [объект Microsoft.graph.termStore.group](../resources/termstore-group.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8dd8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8dd8-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="c8dd8-129">Пример 1. Получить группу termStore</span><span class="sxs-lookup"><span data-stu-id="c8dd8-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="c8dd8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8dd8-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c8dd8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8dd8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```
# <a name="c"></a>[<span data-ttu-id="c8dd8-132">C#</span><span class="sxs-lookup"><span data-stu-id="c8dd8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8dd8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8dd8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8dd8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8dd8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8dd8-135">Java</span><span class="sxs-lookup"><span data-stu-id="c8dd8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c8dd8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8dd8-136">Response</span></span>

><span data-ttu-id="c8dd8-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup"  
}
```
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="c8dd8-138">Пример 2. Получить группу termStore и ее родительский ИД сайта</span><span class="sxs-lookup"><span data-stu-id="c8dd8-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="c8dd8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8dd8-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c8dd8-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8dd8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="c8dd8-141">C#</span><span class="sxs-lookup"><span data-stu-id="c8dd8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8dd8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8dd8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8dd8-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8dd8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8dd8-144">Java</span><span class="sxs-lookup"><span data-stu-id="c8dd8-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c8dd8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8dd8-145">Response</span></span>

><span data-ttu-id="c8dd8-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup",
  "parentSiteId": "microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f"
}
```

### <a name="example-3-get-a-site-collection-termstore-group"></a><span data-ttu-id="c8dd8-147">Пример 3. Получить группу termStore для коллекции сайтов</span><span class="sxs-lookup"><span data-stu-id="c8dd8-147">Example 3: Get a site collection termStore group</span></span>
#### <a name="request"></a><span data-ttu-id="c8dd8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8dd8-148">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C
```

#### <a name="response"></a><span data-ttu-id="c8dd8-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8dd8-149">Response</span></span>

><span data-ttu-id="c8dd8-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8dd8-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup",
}
```

[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termGroup",
  "suppressions": [
  ]
}
-->


