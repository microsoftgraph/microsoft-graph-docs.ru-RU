---
title: Создание цепочки
description: Создание цепочки в указанной беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4df6ba09df66966a741d6cff25580c0177848085
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960534"
---
# <a name="create-thread"></a><span data-ttu-id="ba2a6-103">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="ba2a6-103">Create thread</span></span>

> <span data-ttu-id="ba2a6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba2a6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba2a6-106">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-106">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="ba2a6-p102">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread-reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post-reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p102">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="ba2a6-110">Примечание. Вы также можете [начать новую беседу, создав цепочку](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="ba2a6-110">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba2a6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba2a6-111">Permissions</span></span>
<span data-ttu-id="ba2a6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba2a6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba2a6-114">Permission type</span></span>      | <span data-ttu-id="ba2a6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba2a6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ba2a6-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2a6-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba2a6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba2a6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba2a6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-119">Not supported.</span></span>    |
|<span data-ttu-id="ba2a6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba2a6-120">Application</span></span> | <span data-ttu-id="ba2a6-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2a6-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba2a6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba2a6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="ba2a6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba2a6-123">Request headers</span></span>
| <span data-ttu-id="ba2a6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ba2a6-124">Name</span></span>       | <span data-ttu-id="ba2a6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ba2a6-125">Type</span></span> | <span data-ttu-id="ba2a6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ba2a6-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba2a6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba2a6-127">Authorization</span></span>  | <span data-ttu-id="ba2a6-128">строка</span><span class="sxs-lookup"><span data-stu-id="ba2a6-128">string</span></span>  | <span data-ttu-id="ba2a6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba2a6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba2a6-131">Request body</span></span>
<span data-ttu-id="ba2a6-132">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-132">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ba2a6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba2a6-133">Response</span></span>

<span data-ttu-id="ba2a6-134">В случае успеха этот метод возвратит код отклика `201 Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-134">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba2a6-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ba2a6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba2a6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba2a6-136">Request</span></span>
<span data-ttu-id="ba2a6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="ba2a6-138">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-138">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ba2a6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba2a6-139">Response</span></span>

<span data-ttu-id="ba2a6-p105">В случае успеха этот метод возвратит код отклика `201 Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba2a6-p105">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
