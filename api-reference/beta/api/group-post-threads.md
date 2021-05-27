---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 06dfeaa50fc10907d71684602df40aaf2cbda428
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681293"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="1f92c-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="1f92c-103">Create conversation thread</span></span>

<span data-ttu-id="1f92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f92c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f92c-105">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="1f92c-105">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="1f92c-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="1f92c-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="1f92c-108">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="1f92c-108">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1f92c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f92c-109">Permissions</span></span>
<span data-ttu-id="1f92c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f92c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f92c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f92c-112">Permission type</span></span>      | <span data-ttu-id="1f92c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f92c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f92c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f92c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1f92c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f92c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f92c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f92c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f92c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f92c-117">Not supported.</span></span>    |
|<span data-ttu-id="1f92c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f92c-118">Application</span></span> | <span data-ttu-id="1f92c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f92c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f92c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f92c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="1f92c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f92c-121">Request headers</span></span>
| <span data-ttu-id="1f92c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f92c-122">Header</span></span>       | <span data-ttu-id="1f92c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1f92c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f92c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f92c-124">Authorization</span></span>  | <span data-ttu-id="1f92c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f92c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f92c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f92c-127">Content-Type</span></span>  | <span data-ttu-id="1f92c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f92c-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f92c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f92c-129">Request body</span></span>
<span data-ttu-id="1f92c-130">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f92c-130">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="1f92c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f92c-131">Response</span></span>
<span data-ttu-id="1f92c-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f92c-132">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f92c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f92c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1f92c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f92c-134">Request</span></span>
<span data-ttu-id="1f92c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f92c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f92c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f92c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
# <a name="c"></a>[<span data-ttu-id="1f92c-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f92c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationthread-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f92c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f92c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationthread-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f92c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f92c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationthread-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f92c-140">Java</span><span class="sxs-lookup"><span data-stu-id="1f92c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationthread-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f92c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f92c-141">Response</span></span>
<span data-ttu-id="1f92c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f92c-142">The following is an example of the response.</span></span>
><span data-ttu-id="1f92c-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1f92c-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


