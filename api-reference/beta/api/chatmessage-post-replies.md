---
title: Отправка ответов на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d591247e17e5b734f144ec0891bdc1a3163ca7b6
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583078"
---
# <a name="send-replies-to-a-message-in-a-channel"></a><span data-ttu-id="1c246-103">Отправка ответов на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="1c246-103">Send replies to a message in a channel</span></span>

<span data-ttu-id="1c246-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c246-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c246-105">Отправьте новый ответ в [chatMessage в](../resources/chatmessage.md) указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="1c246-105">Send a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="1c246-106">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="1c246-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="1c246-107">Отправка сообщений, которые будут читаться людьми.</span><span class="sxs-lookup"><span data-stu-id="1c246-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="1c246-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c246-108">Permissions</span></span>
<span data-ttu-id="1c246-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c246-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c246-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c246-111">Permission type</span></span>                        | <span data-ttu-id="1c246-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c246-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c246-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c246-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c246-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c246-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1c246-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c246-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c246-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c246-116">Not supported.</span></span> |
| <span data-ttu-id="1c246-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c246-117">Application</span></span>                            | <span data-ttu-id="1c246-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="1c246-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="1c246-119">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="1c246-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="1c246-120">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="1c246-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c246-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c246-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="1c246-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c246-122">Request headers</span></span>
| <span data-ttu-id="1c246-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1c246-123">Name</span></span>       | <span data-ttu-id="1c246-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1c246-124">Type</span></span> | <span data-ttu-id="1c246-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1c246-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c246-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c246-126">Authorization</span></span>  | <span data-ttu-id="1c246-127">string</span><span class="sxs-lookup"><span data-stu-id="1c246-127">string</span></span>  | <span data-ttu-id="1c246-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c246-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c246-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c246-130">Request body</span></span>
<span data-ttu-id="1c246-131">В тексте запроса поставляем представление JSON объекта [сообщения.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1c246-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="1c246-132">Обязательным является только свойство body, другие свойства необязательны.</span><span class="sxs-lookup"><span data-stu-id="1c246-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="1c246-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c246-133">Response</span></span>

<span data-ttu-id="1c246-134">В случае успешной работы этот метод возвращает `201 Created` код ответа с [созданным](../resources/chatmessage.md) сообщением.</span><span class="sxs-lookup"><span data-stu-id="1c246-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="1c246-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c246-135">Examples</span></span>

### <a name="example-1-send-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="1c246-136">Пример 1. Отправка нового ответа в chatMessage</span><span class="sxs-lookup"><span data-stu-id="1c246-136">Example 1: Send a new reply to a chatMessage</span></span>

<span data-ttu-id="1c246-137">Дополнительный список примеров см. в [странице Create chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="1c246-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

#### <a name="request"></a><span data-ttu-id="1c246-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c246-138">Request</span></span>
<span data-ttu-id="1c246-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c246-139">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessagereply_1"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616990032035/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="1c246-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c246-140">Response</span></span>

<span data-ttu-id="1c246-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c246-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616990032035')/replies/$entity",
    "id": "1616990171266",
    "replyToId": "1616990032035",
    "etag": "1616990171266",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:56:11.266Z",
    "lastModifiedDateTime": "2021-03-29T03:56:11.266Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990171266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990171266&parentMessageId=1616990032035",
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
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a><span data-ttu-id="1c246-142">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="1c246-142">Example 2: Import messages</span></span>

> <span data-ttu-id="1c246-143">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="1c246-143">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="1c246-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c246-144">Request</span></span>

<span data-ttu-id="1c246-145">В следующем примере покажите, как импортировать сообщения с использованием ключей и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="1c246-145">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessagereply_2"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"John Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

#### <a name="response"></a><span data-ttu-id="1c246-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c246-146">Response</span></span>

<span data-ttu-id="1c246-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c246-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
   "id":"1591039710682",
   "replyToId":"1590776551682",
   "etag":"1591039710682",
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
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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
