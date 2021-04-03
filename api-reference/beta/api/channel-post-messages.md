---
title: Отправка chatMessage в канал
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e12ac09d3a4925ffca04bffada4a6763a539624e
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583089"
---
# <a name="send-chatmessage-in-channel"></a><span data-ttu-id="d2e93-103">Отправка chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="d2e93-103">Send chatMessage in channel</span></span>

<span data-ttu-id="d2e93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2e93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e93-105">Отправьте новый [chatMessage в](../resources/chatmessage.md) указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="d2e93-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="d2e93-106">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="d2e93-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="d2e93-107">Отправка сообщений, которые будут читаться людьми.</span><span class="sxs-lookup"><span data-stu-id="d2e93-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e93-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e93-108">Permissions</span></span>

<span data-ttu-id="d2e93-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2e93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e93-111">Permission type</span></span>                        | <span data-ttu-id="d2e93-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2e93-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2e93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2e93-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2e93-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e93-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d2e93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2e93-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e93-116">Not supported.</span></span> |
| <span data-ttu-id="d2e93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2e93-117">Application</span></span>                            | <span data-ttu-id="d2e93-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="d2e93-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="d2e93-119">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="d2e93-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="d2e93-120">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="d2e93-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="d2e93-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2e93-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="d2e93-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2e93-122">Request headers</span></span>

| <span data-ttu-id="d2e93-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d2e93-123">Name</span></span>          | <span data-ttu-id="d2e93-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e93-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d2e93-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2e93-125">Authorization</span></span> | <span data-ttu-id="d2e93-126">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="d2e93-126">Bearer {code}.</span></span> <span data-ttu-id="d2e93-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d2e93-127">Required.</span></span> |
| <span data-ttu-id="d2e93-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2e93-128">Content-type</span></span> | <span data-ttu-id="d2e93-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e93-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2e93-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2e93-131">Request body</span></span>

<span data-ttu-id="d2e93-132">В теле запроса поставляем JSON-представление [объекта chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="d2e93-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="d2e93-133">Обязательным является только свойство body, другие свойства необязательны.</span><span class="sxs-lookup"><span data-stu-id="d2e93-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="d2e93-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e93-134">Response</span></span>

<span data-ttu-id="d2e93-135">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект chatMessage](../resources/chatmessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e93-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2e93-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2e93-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="d2e93-137">Пример 1. Создание сообщения в указанном канале</span><span class="sxs-lookup"><span data-stu-id="d2e93-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="d2e93-138">Дополнительный список примеров см. в [странице Create chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="d2e93-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="d2e93-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e93-139">Request</span></span>
<span data-ttu-id="d2e93-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e93-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_1"
}-->
```http
POST https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

### <a name="response"></a><span data-ttu-id="d2e93-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e93-141">Response</span></span>

<span data-ttu-id="d2e93-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e93-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616990032035",
    "replyToId": null,
    "etag": "1616990032035",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:53:52.035Z",
    "lastModifiedDateTime": "2021-03-29T03:53:52.035Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990032035?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990032035&parentMessageId=1616990032035",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="d2e93-143">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="d2e93-143">Example 2: Import messages</span></span>

> <span data-ttu-id="d2e93-144">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="d2e93-144">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="d2e93-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e93-145">Request</span></span>

<span data-ttu-id="d2e93-146">В следующем примере покажите, как импортировать сообщения с использованием ключей и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e93-146">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_2"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

### <a name="response"></a><span data-ttu-id="d2e93-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e93-147">Response</span></span>

<span data-ttu-id="d2e93-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e93-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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
         "displayName":"John Doe",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="d2e93-149">Пример 3. Импорт сообщений с помощью inline images</span><span class="sxs-lookup"><span data-stu-id="d2e93-149">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="d2e93-150">В настоящее время inline images are the only media type supported by the import message API schpi.</span><span class="sxs-lookup"><span data-stu-id="d2e93-150">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="d2e93-151">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="d2e93-151">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="d2e93-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e93-152">Request</span></span>

<span data-ttu-id="d2e93-153">В следующем примере показано, как импортировать сообщения, содержащие inline-изображения с помощью клавиш и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e93-153">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_channelmessage_3"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "hostedContents":[
      {
         "@microsoft.graph.temporaryId":"1",
         "contentBytes":"iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
         "contentType":"image/png"
      }
   ]
}
```

#### <a name="response"></a><span data-ttu-id="d2e93-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e93-154">Response</span></span>

<span data-ttu-id="d2e93-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e93-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"https://graph.microsoft.com/teams/teamId/channels/channelId/messages/id-value/hostedContents/hostedContentId/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}

```

## <a name="see-also"></a><span data-ttu-id="d2e93-156">См. также</span><span class="sxs-lookup"><span data-stu-id="d2e93-156">See also</span></span>

* [<span data-ttu-id="d2e93-157">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d2e93-157">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="d2e93-158">Создание канала</span><span class="sxs-lookup"><span data-stu-id="d2e93-158">Create channel</span></span>](channel-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
