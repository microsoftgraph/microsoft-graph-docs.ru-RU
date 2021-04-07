---
title: Отправка сообщения в чате
description: Отправка нового сообщения в чате.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79df3a5e6d6aae74cc0f9d19cdd2abb2003c8f46
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610681"
---
# <a name="send-message-in-a-chat"></a><span data-ttu-id="d7c9c-103">Отправка сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="d7c9c-103">Send message in a chat</span></span>

<span data-ttu-id="d7c9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7c9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7c9c-105">Отправьте новый [чатMessage](../resources/chatmessage.md) в указанном [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="d7c9c-106">Этот API не может создать новый чат; Для получения [](chat-list.md) ID существующего чата перед созданием сообщения чата необходимо использовать метод чаты списка.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="d7c9c-107">**Примечание.** Мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="d7c9c-108">Он не имеет пропускной способности, необходимой для обычной миграции.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="d7c9c-109">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="d7c9c-110">Отправка сообщений, которые будут читаться людьми.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7c9c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c9c-111">Permissions</span></span>

<span data-ttu-id="d7c9c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c9c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7c9c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c9c-114">Permission type</span></span>                        | <span data-ttu-id="d7c9c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d7c9c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7c9c-117">ChatMessage.Send, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7c9c-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="d7c9c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c9c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-119">Not supported.</span></span> |
| <span data-ttu-id="d7c9c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7c9c-120">Application</span></span>                            | <span data-ttu-id="d7c9c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c9c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7c9c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="d7c9c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7c9c-123">Request headers</span></span>

| <span data-ttu-id="d7c9c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d7c9c-124">Name</span></span>          | <span data-ttu-id="d7c9c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d7c9c-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d7c9c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7c9c-126">Authorization</span></span> | <span data-ttu-id="d7c9c-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-127">Bearer {code}.</span></span> <span data-ttu-id="d7c9c-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7c9c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7c9c-129">Request body</span></span>

<span data-ttu-id="d7c9c-130">В теле запроса поставляем JSON-представление [объекта chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7c9c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c9c-131">Response</span></span>

<span data-ttu-id="d7c9c-132">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект chatMessage](../resources/chatmessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7c9c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="d7c9c-133">Examples</span></span>

<span data-ttu-id="d7c9c-134">Дополнительный список примеров см. в [странице Create chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="d7c9c-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="d7c9c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7c9c-135">Request</span></span>

<span data-ttu-id="d7c9c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7c9c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7c9c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_chatmessages_1"
}-->
```http
POST https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d7c9c-138">C#</span><span class="sxs-lookup"><span data-stu-id="d7c9c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-chatmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7c9c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7c9c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-chatmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7c9c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7c9c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-chatmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7c9c-141">Java</span><span class="sxs-lookup"><span data-stu-id="d7c9c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-chatmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7c9c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c9c-142">Response</span></span>

<span data-ttu-id="d7c9c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c9c-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages/$entity",
    "id": "1616991463150",
    "replyToId": null,
    "etag": "1616991463150",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:17:43.15Z",
    "lastModifiedDateTime": "2021-03-29T04:17:43.15Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
    "importance": "normal",
    "locale": "en-us",
    "webUrl": null,
    "channelIdentity": null,
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "text",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
