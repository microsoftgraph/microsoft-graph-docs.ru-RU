---
title: Создание беседы
description: 'Создание беседы путем включения цепочки и записи. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c69414b1580aff3e909c02510fbdf6cc81e22d61
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471006"
---
# <a name="create-conversation"></a><span data-ttu-id="3a58d-103">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="3a58d-103">Create conversation</span></span>

<span data-ttu-id="3a58d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a58d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a58d-105">Создание объекта [conversation](../resources/conversation.md) путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="3a58d-105">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="3a58d-106">Размещать в беседе дальнейшие записи можно с помощью [ответов на цепочки](conversationthread-reply.md) и [ответов на записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="3a58d-106">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a58d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a58d-107">Permissions</span></span>
<span data-ttu-id="3a58d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a58d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a58d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a58d-110">Permission type</span></span>      | <span data-ttu-id="3a58d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a58d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a58d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a58d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a58d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a58d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a58d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a58d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a58d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a58d-115">Not supported.</span></span>    |
|<span data-ttu-id="3a58d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a58d-116">Application</span></span> | <span data-ttu-id="3a58d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a58d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a58d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a58d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="3a58d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a58d-119">Request headers</span></span>
| <span data-ttu-id="3a58d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a58d-120">Header</span></span>       | <span data-ttu-id="3a58d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3a58d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a58d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a58d-122">Authorization</span></span>  | <span data-ttu-id="3a58d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a58d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a58d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a58d-125">Content-Type</span></span>  | <span data-ttu-id="3a58d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a58d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a58d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a58d-127">Request body</span></span>
<span data-ttu-id="3a58d-128">Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationthread.md) и [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a58d-128">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="3a58d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a58d-129">Response</span></span>
<span data-ttu-id="3a58d-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a58d-130">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="3a58d-131">Отклик включает идентификаторы для новой беседы и цепочки. Вы можете их использовать в операции [перечисления записей](conversationthread-list-posts.md) для получения новой записи.</span><span class="sxs-lookup"><span data-stu-id="3a58d-131">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="3a58d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3a58d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3a58d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a58d-133">Request</span></span>
<span data-ttu-id="3a58d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a58d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a58d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a58d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations
Content-type: application/json

{
  "topic":"New head count",
  "threads":[
    {
      "posts":[
        {
          "body":{
            "contentType":"html",
            "content":"The confirmation will come by the end of the week."
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
# <a name="c"></a>[<span data-ttu-id="3a58d-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a58d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a58d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a58d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a58d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a58d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a58d-139">Java</span><span class="sxs-lookup"><span data-stu-id="3a58d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a58d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a58d-140">Response</span></span>
<span data-ttu-id="3a58d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a58d-141">The following is an example of the response.</span></span>
><span data-ttu-id="3a58d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a58d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations/$entity",
  "id":"AAQkADPxBgqECsrFDTuM=",
  "threads@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations('AAQkADPxBgqECsrFDTuM%3D')/threads",
  "threads":[
    {
      "id":"AAQkADUNO4xAAMbGA93Sw-EGCoQKysUNO4w=="
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


