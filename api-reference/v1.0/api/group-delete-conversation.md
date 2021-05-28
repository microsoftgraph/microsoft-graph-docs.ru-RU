---
title: Удаление беседы
description: Удаление объекта conversation.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 962216fbb34f63de654de877b2833befab95b739
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682609"
---
# <a name="delete-conversation"></a><span data-ttu-id="d04d3-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="d04d3-103">Delete conversation</span></span>

<span data-ttu-id="d04d3-104">Пространство имен: microsoft.graph Delete a [conversation](../resources/conversation.md) object.</span><span class="sxs-lookup"><span data-stu-id="d04d3-104">Namespace: microsoft.graph Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d04d3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d04d3-105">Permissions</span></span>
<span data-ttu-id="d04d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d04d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d04d3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d04d3-108">Permission type</span></span>      | <span data-ttu-id="d04d3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d04d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d04d3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d04d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d04d3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d04d3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d04d3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d04d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d04d3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d04d3-113">Not supported.</span></span>    |
|<span data-ttu-id="d04d3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d04d3-114">Application</span></span> | <span data-ttu-id="d04d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d04d3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d04d3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d04d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d04d3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d04d3-117">Request headers</span></span>
| <span data-ttu-id="d04d3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d04d3-118">Name</span></span>       | <span data-ttu-id="d04d3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d04d3-119">Type</span></span> | <span data-ttu-id="d04d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d04d3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d04d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d04d3-121">Authorization</span></span>  | <span data-ttu-id="d04d3-122">string</span><span class="sxs-lookup"><span data-stu-id="d04d3-122">string</span></span>  | <span data-ttu-id="d04d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d04d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d04d3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d04d3-125">Request body</span></span>
<span data-ttu-id="d04d3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d04d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d04d3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d04d3-127">Response</span></span>
<span data-ttu-id="d04d3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d04d3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d04d3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d04d3-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d04d3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d04d3-131">Request</span></span>
<span data-ttu-id="d04d3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d04d3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d04d3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d04d3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="d04d3-134">C#</span><span class="sxs-lookup"><span data-stu-id="d04d3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d04d3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d04d3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d04d3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d04d3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d04d3-137">Java</span><span class="sxs-lookup"><span data-stu-id="d04d3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d04d3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d04d3-138">Response</span></span>
<span data-ttu-id="d04d3-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d04d3-139">The following is an example of the response.</span></span> 
><span data-ttu-id="d04d3-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d04d3-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

