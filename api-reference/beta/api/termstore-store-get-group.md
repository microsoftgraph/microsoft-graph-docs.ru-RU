---
title: Вывод группы
description: Ознакомьтесь с свойствами и отношениями группового объекта.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e13a7d3f79da8227e0599d30182ea30e6799ed96
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961340"
---
# <a name="get-group"></a><span data-ttu-id="d55e2-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="d55e2-103">Get group</span></span>
<span data-ttu-id="d55e2-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="d55e2-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d55e2-105">Ознакомьтесь с свойствами и отношениями [группового](../resources/termstore-group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="d55e2-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d55e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d55e2-106">Permissions</span></span>
<span data-ttu-id="d55e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d55e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d55e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d55e2-109">Permission type</span></span>|<span data-ttu-id="d55e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d55e2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d55e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d55e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d55e2-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d55e2-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d55e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d55e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d55e2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d55e2-114">Not supported.</span></span>    |
|<span data-ttu-id="d55e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d55e2-115">Application</span></span> | <span data-ttu-id="d55e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d55e2-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d55e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d55e2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="d55e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d55e2-118">Request headers</span></span>
|<span data-ttu-id="d55e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d55e2-119">Name</span></span>|<span data-ttu-id="d55e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d55e2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d55e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d55e2-121">Authorization</span></span>|<span data-ttu-id="d55e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d55e2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d55e2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d55e2-124">Request body</span></span>
<span data-ttu-id="d55e2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d55e2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d55e2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d55e2-126">Response</span></span>

<span data-ttu-id="d55e2-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/termstore-group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d55e2-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d55e2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d55e2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d55e2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d55e2-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d55e2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d55e2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```
# <a name="c"></a>[<span data-ttu-id="d55e2-131">C#</span><span class="sxs-lookup"><span data-stu-id="d55e2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d55e2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d55e2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d55e2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d55e2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d55e2-134">Java</span><span class="sxs-lookup"><span data-stu-id="d55e2-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d55e2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d55e2-135">Response</span></span>

<span data-ttu-id="d55e2-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d55e2-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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


