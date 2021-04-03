---
title: Отправка сообщения в чате
description: Отправка нового сообщения в чате.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34a3fd2d8b78f845c730b07e4eb566745babd67d
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582935"
---
# <a name="send-message-in-a-chat"></a><span data-ttu-id="3d85b-103">Отправка сообщения в чате</span><span class="sxs-lookup"><span data-stu-id="3d85b-103">Send message in a chat</span></span>

<span data-ttu-id="3d85b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d85b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d85b-105">Отправьте новый [чатMessage](../resources/chatmessage.md) в указанном [чате.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="3d85b-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="3d85b-106">Этот API не может создать новый чат; Для получения [](chat-list-messages.md) ID существующего чата перед созданием сообщения чата необходимо использовать метод чаты списка.</span><span class="sxs-lookup"><span data-stu-id="3d85b-106">This API cannot create a new chat; you must use the [list chats](chat-list-messages.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="3d85b-107">**Примечание.** Мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="3d85b-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="3d85b-108">Он не имеет пропускной способности, необходимой для обычной миграции.</span><span class="sxs-lookup"><span data-stu-id="3d85b-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="3d85b-109">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="3d85b-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="3d85b-110">Отправка сообщений, которые будут читаться людьми.</span><span class="sxs-lookup"><span data-stu-id="3d85b-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d85b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d85b-111">Permissions</span></span>

<span data-ttu-id="3d85b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d85b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d85b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d85b-114">Permission type</span></span>                        | <span data-ttu-id="3d85b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d85b-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d85b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d85b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d85b-117">ChatMessage.Send, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d85b-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="3d85b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d85b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d85b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d85b-119">Not supported.</span></span> |
| <span data-ttu-id="3d85b-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d85b-120">Application</span></span>                            | <span data-ttu-id="3d85b-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d85b-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d85b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d85b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="3d85b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d85b-123">Request headers</span></span>

| <span data-ttu-id="3d85b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3d85b-124">Name</span></span>          | <span data-ttu-id="3d85b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3d85b-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3d85b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d85b-126">Authorization</span></span> | <span data-ttu-id="3d85b-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="3d85b-127">Bearer {code}.</span></span> <span data-ttu-id="3d85b-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3d85b-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d85b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d85b-129">Request body</span></span>

<span data-ttu-id="3d85b-130">В теле запроса поставляем JSON-представление [объекта chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="3d85b-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3d85b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d85b-131">Response</span></span>

<span data-ttu-id="3d85b-132">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект chatMessage](../resources/chatmessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3d85b-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d85b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d85b-133">Examples</span></span>

<span data-ttu-id="3d85b-134">Дополнительный список примеров см. в [странице Create chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="3d85b-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="3d85b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d85b-135">Request</span></span>

<span data-ttu-id="3d85b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d85b-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessages_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```

### <a name="response"></a><span data-ttu-id="3d85b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d85b-137">Response</span></span>

<span data-ttu-id="3d85b-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3d85b-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages/$entity",
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
