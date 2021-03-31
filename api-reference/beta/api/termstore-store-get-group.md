---
title: Вывод группы
description: Ознакомьтесь с свойствами и отношениями группового объекта.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86a96855c330e581e98da902b5e38f16cc857ec9
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473299"
---
# <a name="get-group"></a><span data-ttu-id="4bb07-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="4bb07-103">Get group</span></span>
<span data-ttu-id="4bb07-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="4bb07-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb07-105">Ознакомьтесь с свойствами и отношениями объекта группы [терминов](../resources/termstore-group.md) store.</span><span class="sxs-lookup"><span data-stu-id="4bb07-105">Read the properties and relationships of a term store [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bb07-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb07-106">Permissions</span></span>
<span data-ttu-id="4bb07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bb07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb07-109">Permission type</span></span>|<span data-ttu-id="4bb07-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb07-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bb07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4bb07-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb07-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="4bb07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bb07-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb07-114">Not supported.</span></span>    |
|<span data-ttu-id="4bb07-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb07-115">Application</span></span> | <span data-ttu-id="4bb07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb07-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="4bb07-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb07-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="4bb07-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb07-118">Request headers</span></span>
|<span data-ttu-id="4bb07-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4bb07-119">Name</span></span>|<span data-ttu-id="4bb07-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb07-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4bb07-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bb07-121">Authorization</span></span>|<span data-ttu-id="4bb07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bb07-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb07-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb07-124">Request body</span></span>
<span data-ttu-id="4bb07-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bb07-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bb07-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb07-126">Response</span></span>

<span data-ttu-id="4bb07-127">В случае успеха этот метод возвращает код отклика и `200 OK` [объект Microsoft.graph.termStore.group](../resources/termstore-group.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4bb07-127">If successful, this method returns a `200 OK` response code and a [microsoft.graph.termStore.group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bb07-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4bb07-128">Examples</span></span>

### <a name="example-1-get-a-termstore-group"></a><span data-ttu-id="4bb07-129">Пример 1. Получить группу termStore</span><span class="sxs-lookup"><span data-stu-id="4bb07-129">Example 1: Get a termStore group</span></span>

#### <a name="request"></a><span data-ttu-id="4bb07-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb07-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4bb07-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bb07-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="4bb07-132">C#</span><span class="sxs-lookup"><span data-stu-id="4bb07-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bb07-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bb07-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bb07-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bb07-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bb07-135">Java</span><span class="sxs-lookup"><span data-stu-id="4bb07-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4bb07-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb07-136">Response</span></span>

<span data-ttu-id="4bb07-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4bb07-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-a-termstore-group-and-its-parent-site-id"></a><span data-ttu-id="4bb07-138">Пример 2. Получить группу termStore и ее родительский ИД сайта</span><span class="sxs-lookup"><span data-stu-id="4bb07-138">Example 2: Get a termStore group and its parent site ID</span></span>

#### <a name="request"></a><span data-ttu-id="4bb07-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb07-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}?$select=*,parentSiteId
```

#### <a name="response"></a><span data-ttu-id="4bb07-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb07-140">Response</span></span>

<span data-ttu-id="4bb07-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4bb07-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


