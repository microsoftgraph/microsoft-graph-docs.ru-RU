---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f0c5ea3e8a36071bc78d4a65add47e14fa7fe9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837977"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="e1b11-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="e1b11-103">Create conversation thread</span></span>
<span data-ttu-id="e1b11-104">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="e1b11-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="e1b11-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="e1b11-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="e1b11-107">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="e1b11-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1b11-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b11-108">Permissions</span></span>
<span data-ttu-id="e1b11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1b11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b11-111">Permission type</span></span>      | <span data-ttu-id="e1b11-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1b11-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1b11-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1b11-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b11-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b11-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1b11-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1b11-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b11-116">Not supported.</span></span>    |
|<span data-ttu-id="e1b11-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1b11-117">Application</span></span> | <span data-ttu-id="e1b11-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b11-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1b11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1b11-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="e1b11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1b11-120">Request headers</span></span>
| <span data-ttu-id="e1b11-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1b11-121">Header</span></span>       | <span data-ttu-id="e1b11-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1b11-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1b11-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1b11-123">Authorization</span></span>  | <span data-ttu-id="e1b11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1b11-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1b11-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1b11-126">Content-Type</span></span>  | <span data-ttu-id="e1b11-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b11-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1b11-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1b11-128">Request body</span></span>
<span data-ttu-id="e1b11-129">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b11-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="e1b11-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1b11-130">Response</span></span>
<span data-ttu-id="e1b11-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1b11-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b11-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e1b11-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e1b11-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1b11-133">Request</span></span>
<span data-ttu-id="e1b11-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1b11-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
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
#### <a name="response"></a><span data-ttu-id="e1b11-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1b11-135">Response</span></span>
<span data-ttu-id="e1b11-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1b11-136">The following is an example of the response.</span></span>
><span data-ttu-id="e1b11-137">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e1b11-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1b11-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1b11-138">All the properties will be returned from an actual call.</span></span>
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
  "lastDeliveredDateTime": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
