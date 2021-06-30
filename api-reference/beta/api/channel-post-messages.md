---
title: Отправка chatMessage в канал
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aac8f715059a2a4b497adbca7d2eb21a4c62dcb3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207583"
---
# <a name="send-chatmessage-in-channel"></a><span data-ttu-id="cfbd8-103">Отправка chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="cfbd8-103">Send chatMessage in channel</span></span>

<span data-ttu-id="cfbd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfbd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfbd8-105">Отправьте новый [chatMessage в](../resources/chatmessage.md) указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="cfbd8-106">**Примечание.** Это нарушение условий использования Microsoft Teams в качестве файла журнала. [](/legal/microsoft-apis/terms-of-use)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="cfbd8-107">Отправка сообщений, которые будут читаться людьми.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfbd8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfbd8-108">Permissions</span></span>

<span data-ttu-id="cfbd8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfbd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfbd8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfbd8-111">Permission type</span></span>                        | <span data-ttu-id="cfbd8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfbd8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfbd8-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfbd8-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cfbd8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfbd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-116">Not supported.</span></span> |
| <span data-ttu-id="cfbd8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfbd8-117">Application</span></span>                            | <span data-ttu-id="cfbd8-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="cfbd8-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="cfbd8-119">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="cfbd8-120">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="cfbd8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfbd8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="cfbd8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfbd8-122">Request headers</span></span>

| <span data-ttu-id="cfbd8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="cfbd8-123">Name</span></span>          | <span data-ttu-id="cfbd8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cfbd8-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cfbd8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfbd8-125">Authorization</span></span> | <span data-ttu-id="cfbd8-126">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-126">Bearer {code}.</span></span> <span data-ttu-id="cfbd8-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-127">Required.</span></span> |
| <span data-ttu-id="cfbd8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfbd8-128">Content-type</span></span> | <span data-ttu-id="cfbd8-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfbd8-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfbd8-131">Request body</span></span>

<span data-ttu-id="cfbd8-132">В теле запроса поставляем JSON-представление [объекта chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="cfbd8-133">Обязательным является только свойство body, другие свойства необязательны.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="cfbd8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfbd8-134">Response</span></span>

<span data-ttu-id="cfbd8-135">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект chatMessage](../resources/chatmessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfbd8-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="cfbd8-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="cfbd8-137">Пример 1. Создание сообщения в указанном канале</span><span class="sxs-lookup"><span data-stu-id="cfbd8-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="cfbd8-138">Дополнительный список примеров см. в [странице Create chatMessage в канале или чате.](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="cfbd8-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="cfbd8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfbd8-139">Request</span></span>
<span data-ttu-id="cfbd8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfbd8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfbd8-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cfbd8-142">C#</span><span class="sxs-lookup"><span data-stu-id="cfbd8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfbd8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfbd8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfbd8-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfbd8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfbd8-145">Java</span><span class="sxs-lookup"><span data-stu-id="cfbd8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfbd8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfbd8-146">Response</span></span>

<span data-ttu-id="cfbd8-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-147">The following is an example of the response.</span></span>

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

### <a name="example-2-import-messages"></a><span data-ttu-id="cfbd8-148">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="cfbd8-148">Example 2: Import messages</span></span>

> <span data-ttu-id="cfbd8-149">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-149">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="cfbd8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfbd8-150">Request</span></span>

<span data-ttu-id="cfbd8-151">В следующем примере покажите, как импортировать сообщения с использованием ключей и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-151">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfbd8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfbd8-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cfbd8-153">C#</span><span class="sxs-lookup"><span data-stu-id="cfbd8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfbd8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfbd8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfbd8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfbd8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfbd8-156">Java</span><span class="sxs-lookup"><span data-stu-id="cfbd8-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfbd8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfbd8-157">Response</span></span>

<span data-ttu-id="cfbd8-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-158">The following is an example of the response.</span></span>

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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="cfbd8-159">Пример 3. Импорт сообщений с помощью inline images</span><span class="sxs-lookup"><span data-stu-id="cfbd8-159">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="cfbd8-160">В настоящее время inline images are the only media type supported by the import message API schpi.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-160">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="cfbd8-161">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-161">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="cfbd8-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfbd8-162">Request</span></span>

<span data-ttu-id="cfbd8-163">В следующем примере показано, как импортировать сообщения, содержащие inline-изображения с помощью клавиш и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-163">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfbd8-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfbd8-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cfbd8-165">C#</span><span class="sxs-lookup"><span data-stu-id="cfbd8-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfbd8-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfbd8-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfbd8-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfbd8-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfbd8-168">Java</span><span class="sxs-lookup"><span data-stu-id="cfbd8-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfbd8-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfbd8-169">Response</span></span>

<span data-ttu-id="cfbd8-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cfbd8-170">The following is an example of the response.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="cfbd8-171">См. также</span><span class="sxs-lookup"><span data-stu-id="cfbd8-171">See also</span></span>

* [<span data-ttu-id="cfbd8-172">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cfbd8-172">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="cfbd8-173">Создание канала</span><span class="sxs-lookup"><span data-stu-id="cfbd8-173">Create channel</span></span>](channel-post.md)

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
