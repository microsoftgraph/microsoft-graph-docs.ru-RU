---
title: Создание беседы
description: 'Создание беседы путем включения цепочки и записи. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a81ae51a7fbccebd60354cf9eb659697b8e7f474
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613953"
---
# <a name="create-conversation"></a><span data-ttu-id="523c7-103">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="523c7-103">Create conversation</span></span>
<span data-ttu-id="523c7-104">Создание объекта [conversation](../resources/conversation.md) путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="523c7-104">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="523c7-105">Размещать в беседе дальнейшие записи можно с помощью [ответов на цепочки](conversationthread-reply.md) и [ответов на записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="523c7-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="523c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="523c7-106">Permissions</span></span>
<span data-ttu-id="523c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="523c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="523c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="523c7-109">Permission type</span></span>      | <span data-ttu-id="523c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="523c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="523c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="523c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="523c7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="523c7-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="523c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="523c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="523c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="523c7-114">Not supported.</span></span>    |
|<span data-ttu-id="523c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="523c7-115">Application</span></span> | <span data-ttu-id="523c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="523c7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="523c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="523c7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="523c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="523c7-118">Request headers</span></span>
| <span data-ttu-id="523c7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="523c7-119">Header</span></span>       | <span data-ttu-id="523c7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="523c7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="523c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="523c7-121">Authorization</span></span>  | <span data-ttu-id="523c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="523c7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="523c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="523c7-124">Content-Type</span></span>  | <span data-ttu-id="523c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="523c7-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="523c7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="523c7-126">Request body</span></span>
<span data-ttu-id="523c7-127">Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationthread.md) и [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="523c7-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="523c7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="523c7-128">Response</span></span>
<span data-ttu-id="523c7-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="523c7-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="523c7-130">Отклик включает идентификаторы для новой беседы и цепочки. Вы можете их использовать в операции [перечисления записей](conversationthread-list-posts.md) для получения новой записи.</span><span class="sxs-lookup"><span data-stu-id="523c7-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="523c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="523c7-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="523c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="523c7-132">Request</span></span>
<span data-ttu-id="523c7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="523c7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["29981b6a-0e57-42dc-94c9-cd24f5306196"],
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
    "topic":"New locations for this quarter",
    "threads":[
        {
            "posts":[
                {
                    "body":{
                        "contentType":"html",
                        "content":"What do we know so far?"
                    },
                    "newParticipants":[
                        {
                            "emailAddress":{
                                "name":"Adele Vance",
                                "address":"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="523c7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="523c7-134">Response</span></span>
<span data-ttu-id="523c7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="523c7-135">The following is an example of the response.</span></span>
><span data-ttu-id="523c7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="523c7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
    "id":"AAQkADDVKtMlRp4Txc6k=",
    "threads@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADDVKtMlRp4Txc6k%3D')/threads",
    "threads":[
        {
            "id":"AAQkADQDarUNUq0yVGnhPFzqQ=="
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="523c7-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="523c7-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="523c7-139">Языках</span><span class="sxs-lookup"><span data-stu-id="523c7-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_conversation_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="523c7-140">Язык</span><span class="sxs-lookup"><span data-stu-id="523c7-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_conversation_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-conversations.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-conversations.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
