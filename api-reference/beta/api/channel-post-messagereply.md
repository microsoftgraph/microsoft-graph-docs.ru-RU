---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: db0164be77260c60c2d89c726b048b4af8dc741d
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101904"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="f5140-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="f5140-103">Reply to a message in a channel</span></span>

<span data-ttu-id="f5140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5140-105">Создайте новый ответ [на chatMessage](../resources/chatmessage.md) в указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="f5140-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="f5140-106">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="f5140-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="f5140-107">Отправлять только сообщения, которые будут читаться.</span><span class="sxs-lookup"><span data-stu-id="f5140-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="f5140-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5140-108">Permissions</span></span>
<span data-ttu-id="f5140-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5140-111">Permission type</span></span>                        | <span data-ttu-id="f5140-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5140-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5140-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5140-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5140-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5140-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f5140-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5140-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5140-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5140-116">Not supported.</span></span> |
| <span data-ttu-id="f5140-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5140-117">Application</span></span>                            | <span data-ttu-id="f5140-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="f5140-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="f5140-119">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="f5140-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="f5140-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5140-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="f5140-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5140-121">Request headers</span></span>
| <span data-ttu-id="f5140-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f5140-122">Name</span></span>       | <span data-ttu-id="f5140-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f5140-123">Type</span></span> | <span data-ttu-id="f5140-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f5140-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5140-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5140-125">Authorization</span></span>  | <span data-ttu-id="f5140-126">string</span><span class="sxs-lookup"><span data-stu-id="f5140-126">string</span></span>  | <span data-ttu-id="f5140-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5140-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5140-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5140-129">Request body</span></span>
<span data-ttu-id="f5140-130">В тексте запроса укажу представление объекта [сообщения](../resources/chatmessage.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f5140-130">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="f5140-131">Только свойство body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="f5140-131">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="f5140-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5140-132">Response</span></span>

<span data-ttu-id="f5140-133">В случае успеха этот метод возвращает `201 Created` код ответа с созданным сообщением. [](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f5140-133">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="f5140-134">Пример 1. Создание ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="f5140-134">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="f5140-135">Более полный список примеров см. в примере [создания chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="f5140-135">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="f5140-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5140-136">Request</span></span>
<span data-ttu-id="f5140-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5140-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5140-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5140-138">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="f5140-139">C#</span><span class="sxs-lookup"><span data-stu-id="f5140-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5140-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5140-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5140-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5140-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5140-142">Java</span><span class="sxs-lookup"><span data-stu-id="f5140-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f5140-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5140-143">Response</span></span>

<span data-ttu-id="f5140-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5140-144">The following is an example of the response.</span></span>
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

### <a name="example-2-import-messages"></a><span data-ttu-id="f5140-145">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="f5140-145">Example 2: Import messages</span></span>

> <span data-ttu-id="f5140-146">**Примечание.** Для этого `Teamwork.Migrate.All` сценария требуется область разрешений.</span><span class="sxs-lookup"><span data-stu-id="f5140-146">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="f5140-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5140-147">Request</span></span>

<span data-ttu-id="f5140-148">В следующем примере покажите, как импортировать сообщения во времени с помощью ключей и `createDateTime` ключей `from` в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="f5140-148">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

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
#### <a name="response"></a><span data-ttu-id="f5140-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5140-149">Response</span></span>

<span data-ttu-id="f5140-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5140-150">The following is an example of the response.</span></span>

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
