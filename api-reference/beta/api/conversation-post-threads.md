---
title: Создание цепочки
description: Создание цепочки в указанной беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f4b939758906da1814ee4ffc2a722427bf4e7f6e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326694"
---
# <a name="create-thread"></a><span data-ttu-id="6f8f8-103">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="6f8f8-103">Create thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f8f8-104">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-104">Create a new thread in the specified conversation.</span></span>

<span data-ttu-id="6f8f8-p101">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread-reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post-reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-p101">A thread and post are created as specified. Use [reply thread](conversationthread-reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post-reply.md) to that post in that thread.</span></span>

<span data-ttu-id="6f8f8-108">Примечание. Вы также можете [начать новую беседу, создав цепочку](group-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="6f8f8-108">Note: You can also [start a new conversation by first creating a thread](group-post-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f8f8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f8f8-109">Permissions</span></span>
<span data-ttu-id="6f8f8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f8f8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f8f8-112">Permission type</span></span>      | <span data-ttu-id="6f8f8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f8f8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f8f8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f8f8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6f8f8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f8f8-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f8f8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f8f8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f8f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-117">Not supported.</span></span>    |
|<span data-ttu-id="6f8f8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f8f8-118">Application</span></span> | <span data-ttu-id="6f8f8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f8f8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f8f8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="6f8f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f8f8-121">Request headers</span></span>
| <span data-ttu-id="6f8f8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6f8f8-122">Name</span></span>       | <span data-ttu-id="6f8f8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6f8f8-123">Type</span></span> | <span data-ttu-id="6f8f8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6f8f8-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f8f8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f8f8-125">Authorization</span></span>  | <span data-ttu-id="6f8f8-126">string</span><span class="sxs-lookup"><span data-stu-id="6f8f8-126">string</span></span>  | <span data-ttu-id="6f8f8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f8f8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f8f8-129">Request body</span></span>
<span data-ttu-id="6f8f8-130">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-130">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6f8f8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f8f8-131">Response</span></span>

<span data-ttu-id="6f8f8-132">В случае успеха этот метод возвратит код отклика `201 Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-132">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6f8f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f8f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f8f8-134">Request</span></span>
<span data-ttu-id="6f8f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="6f8f8-136">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-136">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6f8f8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f8f8-137">Response</span></span>

<span data-ttu-id="6f8f8-p104">В случае успеха этот метод возвратит код отклика `201 Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f8f8-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
