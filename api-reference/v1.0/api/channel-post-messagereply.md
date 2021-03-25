---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e56d43e84dc7ba2cc47fd30ac47e9cb2fdcc8ea
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202256"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="54b76-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="54b76-103">Reply to a message in a channel</span></span>

<span data-ttu-id="54b76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54b76-105">Создайте новый ответ [на chatMessage в](../resources/chatmessage.md) указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="54b76-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="54b76-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54b76-106">Permissions</span></span>

<span data-ttu-id="54b76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54b76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54b76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54b76-109">Permission type</span></span>                        | <span data-ttu-id="54b76-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54b76-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54b76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54b76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54b76-112">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b76-112">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="54b76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54b76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54b76-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54b76-114">Not supported.</span></span> |
| <span data-ttu-id="54b76-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54b76-115">Application</span></span>                            | <span data-ttu-id="54b76-116">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="54b76-116">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="54b76-117">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="54b76-117">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="54b76-118">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="54b76-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="54b76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54b76-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="54b76-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54b76-120">Request headers</span></span>

| <span data-ttu-id="54b76-121">Имя</span><span class="sxs-lookup"><span data-stu-id="54b76-121">Name</span></span>       | <span data-ttu-id="54b76-122">Тип</span><span class="sxs-lookup"><span data-stu-id="54b76-122">Type</span></span> | <span data-ttu-id="54b76-123">Описание</span><span class="sxs-lookup"><span data-stu-id="54b76-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="54b76-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b76-124">Authorization</span></span>  | <span data-ttu-id="54b76-125">string</span><span class="sxs-lookup"><span data-stu-id="54b76-125">string</span></span>  | <span data-ttu-id="54b76-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54b76-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54b76-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54b76-128">Request body</span></span>

<span data-ttu-id="54b76-129">В тексте запроса поставляем представление JSON объекта [сообщения.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="54b76-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="54b76-130">Обязательным является только свойство body, другие свойства необязательны.</span><span class="sxs-lookup"><span data-stu-id="54b76-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="54b76-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b76-131">Response</span></span>

<span data-ttu-id="54b76-132">В случае успешной работы этот метод возвращает `201 Created` код ответа с [созданным](../resources/chatmessage.md) сообщением.</span><span class="sxs-lookup"><span data-stu-id="54b76-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="54b76-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="54b76-133">Examples</span></span>

### <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="54b76-134">Пример 1. Создание нового ответа на chatMessage</span><span class="sxs-lookup"><span data-stu-id="54b76-134">Example 1: Create a new reply to a chatMessage</span></span>

#### <a name="request"></a><span data-ttu-id="54b76-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b76-135">Request</span></span>
<span data-ttu-id="54b76-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b76-136">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="54b76-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b76-137">Response</span></span>

<span data-ttu-id="54b76-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54b76-138">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
    "id": "1591039710682",
    "replyToId": "1590776551682",
    "etag": "1591039710682",
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
            "id": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="54b76-139">Пример 2. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="54b76-139">Example 2: Import messages</span></span>

> <span data-ttu-id="54b76-140">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="54b76-140">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="54b76-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b76-141">Request</span></span>

<span data-ttu-id="54b76-142">В следующем примере покажите, как импортировать сообщения с использованием ключей и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="54b76-142">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"Joh Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}

```

#### <a name="response"></a><span data-ttu-id="54b76-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b76-143">Response</span></span>

<span data-ttu-id="54b76-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54b76-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
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
