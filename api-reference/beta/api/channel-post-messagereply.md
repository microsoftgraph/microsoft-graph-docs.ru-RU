---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3f284cacc4e41498a4cc011e98ed9f60898dcc20
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866148"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="8e9d5-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="8e9d5-103">Reply to a message in a channel</span></span>

<span data-ttu-id="8e9d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e9d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e9d5-105">Создайте новый ответ [на chatMessage](../resources/chatmessage.md) в указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="8e9d5-106">**Примечание.** Мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="8e9d5-107">Пропускная способность, необходимая для обычной миграции, не существует.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="8e9d5-108">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-108">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="8e9d5-109">Отправлять только сообщения, которые люди будут читать.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-109">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="8e9d5-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e9d5-110">Permissions</span></span>
<span data-ttu-id="8e9d5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e9d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e9d5-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e9d5-113">Permission type</span></span>      | <span data-ttu-id="8e9d5-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e9d5-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8e9d5-116">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9d5-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="8e9d5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e9d5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-118">Not supported.</span></span>    |
|<span data-ttu-id="8e9d5-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e9d5-119">Application</span></span> | <span data-ttu-id="8e9d5-120">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="8e9d5-120">Teamwork.Migrate.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e9d5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e9d5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="8e9d5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e9d5-122">Request headers</span></span>
| <span data-ttu-id="8e9d5-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8e9d5-123">Name</span></span>       | <span data-ttu-id="8e9d5-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8e9d5-124">Type</span></span> | <span data-ttu-id="8e9d5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8e9d5-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e9d5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9d5-126">Authorization</span></span>  | <span data-ttu-id="8e9d5-127">string</span><span class="sxs-lookup"><span data-stu-id="8e9d5-127">string</span></span>  | <span data-ttu-id="8e9d5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e9d5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e9d5-130">Request body</span></span>
<span data-ttu-id="8e9d5-131">В тексте запроса укажу представление объекта [сообщения](../resources/chatmessage.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="8e9d5-132">Только свойство body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="8e9d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e9d5-133">Response</span></span>

<span data-ttu-id="8e9d5-134">В случае успеха этот метод возвращает `201 Created` код ответа с созданным сообщением. [](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="8e9d5-135">Пример 1. Создание ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="8e9d5-135">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="8e9d5-136">Более полный список примеров см. в примере [создания chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="8e9d5-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="8e9d5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e9d5-137">Request</span></span>
<span data-ttu-id="8e9d5-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e9d5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e9d5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="8e9d5-140">C#</span><span class="sxs-lookup"><span data-stu-id="8e9d5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e9d5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e9d5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e9d5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e9d5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e9d5-143">Java</span><span class="sxs-lookup"><span data-stu-id="8e9d5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8e9d5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e9d5-144">Response</span></span>

<span data-ttu-id="8e9d5-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a><span data-ttu-id="8e9d5-146">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="8e9d5-146">Example 2: Import messages</span></span>

> <span data-ttu-id="8e9d5-147">**Примечание.** Для этого сценария `Teamwork.Migrate.All` требуется область разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-147">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="8e9d5-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e9d5-148">Request</span></span>

<span data-ttu-id="8e9d5-149">В следующем примере покажите, как импортировать сообщения времени назад с помощью ключей и ключей `createDateTime` `from` в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-149">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages/{messageId}/replies

{
   "replyToId":null,
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

---
#### <a name="response"></a><span data-ttu-id="8e9d5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e9d5-150">Response</span></span>

<span data-ttu-id="8e9d5-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e9d5-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams/{teamId}/channels/{channelId}/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
