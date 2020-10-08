---
title: Создание беседы
description: 'Создание беседы путем включения цепочки и записи. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d4d2b411d339e73b7a3f99dee4dbb602e4724ad7
ms.sourcegitcommit: 258974d689cb8f04ff542ec8bc5fe5793da5cc05
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2020
ms.locfileid: "48385816"
---
# <a name="create-conversation"></a><span data-ttu-id="ed125-103">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="ed125-103">Create conversation</span></span>

<span data-ttu-id="ed125-104">Пространство имен: Microsoft. Graph создание новой [беседы](../resources/conversation.md) путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="ed125-104">Namespace: microsoft.graph Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="ed125-105">Размещать в беседе дальнейшие записи можно с помощью [ответов на цепочки](conversationthread-reply.md) и [ответов на записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="ed125-105">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed125-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed125-106">Permissions</span></span>
<span data-ttu-id="ed125-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed125-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed125-109">Permission type</span></span>      | <span data-ttu-id="ed125-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed125-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed125-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed125-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed125-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed125-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed125-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed125-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed125-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed125-114">Not supported.</span></span>    |
|<span data-ttu-id="ed125-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed125-115">Application</span></span> | <span data-ttu-id="ed125-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed125-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed125-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed125-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="ed125-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed125-118">Request headers</span></span>
| <span data-ttu-id="ed125-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed125-119">Header</span></span>       | <span data-ttu-id="ed125-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ed125-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed125-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed125-121">Authorization</span></span>  | <span data-ttu-id="ed125-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed125-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed125-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed125-124">Content-Type</span></span>  | <span data-ttu-id="ed125-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed125-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed125-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed125-126">Request body</span></span>
<span data-ttu-id="ed125-127">Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationthread.md) и [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed125-127">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="ed125-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed125-128">Response</span></span>
<span data-ttu-id="ed125-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed125-129">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

<span data-ttu-id="ed125-130">Отклик включает идентификаторы для новой беседы и цепочки. Вы можете их использовать в операции [перечисления записей](conversationthread-list-posts.md) для получения новой записи.</span><span class="sxs-lookup"><span data-stu-id="ed125-130">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="ed125-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ed125-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ed125-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed125-132">Request</span></span>
<span data-ttu-id="ed125-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed125-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
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

#### <a name="response"></a><span data-ttu-id="ed125-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed125-134">Response</span></span>
<span data-ttu-id="ed125-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed125-135">The following is an example of the response.</span></span>
><span data-ttu-id="ed125-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed125-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

