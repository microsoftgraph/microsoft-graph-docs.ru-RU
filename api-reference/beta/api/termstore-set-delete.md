---
title: Удаление набора
description: Удаление объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 28ed1e580c13ce675e09f6b892cbd4989e56d664
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980091"
---
# <a name="delete-set"></a><span data-ttu-id="48a4f-103">Удаление набора</span><span class="sxs-lookup"><span data-stu-id="48a4f-103">Delete set</span></span>
<span data-ttu-id="48a4f-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="48a4f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a4f-105">Удаление объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="48a4f-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48a4f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48a4f-106">Permissions</span></span>
<span data-ttu-id="48a4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48a4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48a4f-109">Permission type</span></span>|<span data-ttu-id="48a4f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48a4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48a4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48a4f-111">Delegated (work or school account)</span></span> |<span data-ttu-id="48a4f-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a4f-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="48a4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48a4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a4f-114">Not supported.</span></span>    |
|<span data-ttu-id="48a4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48a4f-115">Application</span></span> | <span data-ttu-id="48a4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a4f-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="48a4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48a4f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="48a4f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48a4f-118">Request headers</span></span>
|<span data-ttu-id="48a4f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="48a4f-119">Name</span></span>|<span data-ttu-id="48a4f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="48a4f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48a4f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48a4f-121">Authorization</span></span>|<span data-ttu-id="48a4f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48a4f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48a4f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48a4f-124">Request body</span></span>
<span data-ttu-id="48a4f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48a4f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48a4f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="48a4f-126">Response</span></span>

<span data-ttu-id="48a4f-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48a4f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="48a4f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="48a4f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48a4f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="48a4f-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48a4f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a4f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="48a4f-131">C#</span><span class="sxs-lookup"><span data-stu-id="48a4f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48a4f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a4f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48a4f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48a4f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48a4f-134">Java</span><span class="sxs-lookup"><span data-stu-id="48a4f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="48a4f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="48a4f-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->


