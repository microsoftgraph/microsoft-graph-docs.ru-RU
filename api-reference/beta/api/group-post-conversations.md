---
title: Создание беседы
description: 'Создание беседы путем включения цепочки и записи. '
author: dkershaw10
ms.openlocfilehash: 48907b41362f56467fbb090e75faa8f3e18720c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340539"
---
# <a name="create-conversation"></a><span data-ttu-id="c06a2-103">Создание беседы</span><span class="sxs-lookup"><span data-stu-id="c06a2-103">Create conversation</span></span>

> <span data-ttu-id="c06a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c06a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c06a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c06a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c06a2-106">Создание объекта [conversation](../resources/conversation.md) путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="c06a2-106">Create a new [conversation](../resources/conversation.md) by including a thread and a post.</span></span> 

<span data-ttu-id="c06a2-107">Размещать в беседе дальнейшие записи можно с помощью [ответов на цепочки](conversationthread-reply.md) и [ответов на записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="c06a2-107">Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="c06a2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c06a2-108">Permissions</span></span>
<span data-ttu-id="c06a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c06a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c06a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c06a2-111">Permission type</span></span>      | <span data-ttu-id="c06a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c06a2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c06a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c06a2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c06a2-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c06a2-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c06a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c06a2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c06a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c06a2-116">Not supported.</span></span>    |
|<span data-ttu-id="c06a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c06a2-117">Application</span></span> | <span data-ttu-id="c06a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c06a2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c06a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c06a2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```

## <a name="request-headers"></a><span data-ttu-id="c06a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c06a2-120">Request headers</span></span>
| <span data-ttu-id="c06a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c06a2-121">Header</span></span>       | <span data-ttu-id="c06a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c06a2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c06a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c06a2-123">Authorization</span></span>  | <span data-ttu-id="c06a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c06a2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c06a2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c06a2-126">Content-Type</span></span>  | <span data-ttu-id="c06a2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c06a2-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c06a2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c06a2-128">Request body</span></span>
<span data-ttu-id="c06a2-129">Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationthread.md) и [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c06a2-129">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationthread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="c06a2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c06a2-130">Response</span></span>
<span data-ttu-id="c06a2-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c06a2-131">If successful, this method returns `201 Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span> 

<span data-ttu-id="c06a2-132">Отклик включает идентификаторы для новой беседы и цепочки. Вы можете их использовать в операции [перечисления записей](conversationthread-list-posts.md) для получения новой записи.</span><span class="sxs-lookup"><span data-stu-id="c06a2-132">The response includes the IDs for the new conversation and thread, which you can use in the [list posts](conversationthread-list-posts.md) operation to get the new post as well.</span></span>

## <a name="example"></a><span data-ttu-id="c06a2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c06a2-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c06a2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c06a2-134">Request</span></span>
<span data-ttu-id="c06a2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c06a2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups('29981b6a-0e57-42dc-94c9-cd24f5306196')/conversations
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

#### <a name="response"></a><span data-ttu-id="c06a2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c06a2-136">Response</span></span>
<span data-ttu-id="c06a2-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c06a2-137">The following is an example of the response.</span></span>
><span data-ttu-id="c06a2-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="c06a2-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c06a2-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c06a2-139">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->