---
title: Вывод группы
description: Ознакомьтесь с свойствами и отношениями группового объекта.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2c95937181d90a2f1b8759464b7ef8506397c4a1
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507174"
---
# <a name="get-group"></a><span data-ttu-id="3fd05-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="3fd05-103">Get group</span></span>
<span data-ttu-id="3fd05-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="3fd05-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fd05-105">Ознакомьтесь с свойствами и отношениями объекта группы [терминов](../resources/termstore-group.md) store.</span><span class="sxs-lookup"><span data-stu-id="3fd05-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fd05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd05-106">Permissions</span></span>
<span data-ttu-id="3fd05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fd05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fd05-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fd05-109">Permission type</span></span>|<span data-ttu-id="3fd05-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fd05-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fd05-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fd05-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fd05-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd05-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="3fd05-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fd05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fd05-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd05-114">Not supported.</span></span>    |
|<span data-ttu-id="3fd05-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fd05-115">Application</span></span> | <span data-ttu-id="3fd05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fd05-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="3fd05-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fd05-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="3fd05-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fd05-118">Request headers</span></span>
|<span data-ttu-id="3fd05-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3fd05-119">Name</span></span>|<span data-ttu-id="3fd05-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3fd05-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3fd05-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fd05-121">Authorization</span></span>|<span data-ttu-id="3fd05-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fd05-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fd05-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fd05-124">Request body</span></span>
<span data-ttu-id="3fd05-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fd05-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fd05-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd05-126">Response</span></span>

<span data-ttu-id="3fd05-127">В случае успеха этот метод возвращает код отклика и `200 OK` [объект Microsoft.graph.termStore.group](../resources/termstore-group.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3fd05-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3fd05-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3fd05-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="3fd05-129">Пример 1. Получить группу termStore</span><span class="sxs-lookup"><span data-stu-id="3fd05-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="3fd05-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fd05-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3fd05-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fd05-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="3fd05-132">C#</span><span class="sxs-lookup"><span data-stu-id="3fd05-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fd05-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fd05-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fd05-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fd05-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fd05-135">Java</span><span class="sxs-lookup"><span data-stu-id="3fd05-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3fd05-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd05-136">Response</span></span>

<span data-ttu-id="3fd05-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fd05-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="3fd05-138">Пример 2. Получить группу termStore и ее родительский ИД сайта</span><span class="sxs-lookup"><span data-stu-id="3fd05-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="3fd05-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fd05-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3fd05-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fd05-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}?$select=*,parentSiteId
```
# <a name="c"></a>[<span data-ttu-id="3fd05-141">C#</span><span class="sxs-lookup"><span data-stu-id="3fd05-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fd05-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fd05-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fd05-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fd05-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fd05-144">Java</span><span class="sxs-lookup"><span data-stu-id="3fd05-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3fd05-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fd05-145">Response</span></span>

<span data-ttu-id="3fd05-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fd05-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "parentSiteId": "microsoft.sharepoint.com,05259ba9-25a8-4c93-a9a9-f995ef1fc51f,a785ad58-1d57-4f8a-aa71-77170459bd0d"
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


