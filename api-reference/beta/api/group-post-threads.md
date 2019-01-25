---
title: Создание цепочки беседы
description: 'Начните групповой чат, создав цепочку. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f320c465cee26ef5a91a821cd70b605f4056a9f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517311"
---
# <a name="create-conversation-thread"></a><span data-ttu-id="d2d8d-103">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="d2d8d-103">Create conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2d8d-104">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-104">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="d2d8d-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread-reply.md) и [записи](post-reply.md).</span><span class="sxs-lookup"><span data-stu-id="d2d8d-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread-reply.md) or [reply post](post-reply.md) to further post to that thread.</span></span>

<span data-ttu-id="d2d8d-107">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation-post-threads.md).</span><span class="sxs-lookup"><span data-stu-id="d2d8d-107">Note: You can also [start a new thread in an existing conversation](conversation-post-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d2d8d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d8d-108">Permissions</span></span>
<span data-ttu-id="d2d8d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d8d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d8d-111">Permission type</span></span>      | <span data-ttu-id="d2d8d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2d8d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2d8d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2d8d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d2d8d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d8d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2d8d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2d8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d8d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-116">Not supported.</span></span>    |
|<span data-ttu-id="d2d8d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2d8d-117">Application</span></span> | <span data-ttu-id="d2d8d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2d8d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2d8d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="d2d8d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2d8d-120">Request headers</span></span>
| <span data-ttu-id="d2d8d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2d8d-121">Header</span></span>       | <span data-ttu-id="d2d8d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2d8d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2d8d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2d8d-123">Authorization</span></span>  | <span data-ttu-id="d2d8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2d8d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2d8d-126">Content-Type</span></span>  | <span data-ttu-id="d2d8d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d8d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2d8d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2d8d-128">Request body</span></span>
<span data-ttu-id="d2d8d-129">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-129">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="d2d8d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2d8d-130">Response</span></span>
<span data-ttu-id="d2d8d-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-131">If successful, this method returns `201 Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d8d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2d8d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d2d8d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2d8d-133">Request</span></span>
<span data-ttu-id="d2d8d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d2d8d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2d8d-135">Response</span></span>
<span data-ttu-id="d2d8d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-136">The following is an example of the response.</span></span>
><span data-ttu-id="d2d8d-137">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d2d8d-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2d8d-138">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-post-threads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
