---
title: Создание объекта chatMessage в канале
description: Создание нового chatMessage в указанном канале.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b14d466c3ccced7f8b5d23dfff7cbdcd6440f830
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272770"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="4113c-103">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="4113c-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="4113c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4113c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4113c-105">Создание нового [chatMessage](../resources/chatmessage.md) в указанном [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4113c-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="4113c-106">**Note**: мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="4113c-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="4113c-107">Пропускная способность, необходимая для обычной миграции, отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4113c-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="4113c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4113c-108">Permissions</span></span>

<span data-ttu-id="4113c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4113c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4113c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4113c-111">Permission type</span></span>                        | <span data-ttu-id="4113c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4113c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4113c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4113c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4113c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4113c-114">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4113c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4113c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4113c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4113c-116">Not supported.</span></span> |
| <span data-ttu-id="4113c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4113c-117">Application</span></span>                            | <span data-ttu-id="4113c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4113c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4113c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4113c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="4113c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4113c-120">Request headers</span></span>

| <span data-ttu-id="4113c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4113c-121">Name</span></span>          | <span data-ttu-id="4113c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4113c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4113c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4113c-123">Authorization</span></span> | <span data-ttu-id="4113c-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4113c-124">Bearer {code}.</span></span> <span data-ttu-id="4113c-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4113c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4113c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4113c-126">Request body</span></span>

<span data-ttu-id="4113c-127">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4113c-127">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="4113c-128">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="4113c-128">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="4113c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4113c-129">Response</span></span>

<span data-ttu-id="4113c-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4113c-130">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4113c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4113c-131">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="4113c-132">Пример 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="4113c-132">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="4113c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4113c-133">Request</span></span>

<span data-ttu-id="4113c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4113c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="4113c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4113c-135">Response</span></span>

<span data-ttu-id="4113c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4113c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="4113c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4113c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
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

### <a name="example-2-mentions"></a><span data-ttu-id="4113c-139">Пример 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="4113c-139">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="4113c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4113c-140">Request</span></span>
<span data-ttu-id="4113c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4113c-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="4113c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4113c-142">Response</span></span>

<span data-ttu-id="4113c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4113c-143">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
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
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-cards"></a><span data-ttu-id="4113c-144">Пример 3: карты</span><span class="sxs-lookup"><span data-stu-id="4113c-144">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="4113c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4113c-145">Request</span></span>
<span data-ttu-id="4113c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4113c-146">The following is an example of the request.</span></span>

><span data-ttu-id="4113c-147">**Примечание:** Идентификатор вложения должен быть уникальным и может быть новым случайно созданным идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="4113c-147">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="4113c-148">Однако идентификатор вложения должен быть одинаковым в элементах _Body_ и _вложениях_ .</span><span class="sxs-lookup"><span data-stu-id="4113c-148">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="4113c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4113c-149">Response</span></span>

<span data-ttu-id="4113c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4113c-150">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
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
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\n\\r\\n\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\n\\r\\n\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-4-file-attachments"></a><span data-ttu-id="4113c-151">Пример 4: вложенные файлы</span><span class="sxs-lookup"><span data-stu-id="4113c-151">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="4113c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4113c-152">Request</span></span>
<span data-ttu-id="4113c-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4113c-153">The following is an example of the request.</span></span>

><span data-ttu-id="4113c-154">**Примечание:** Файл уже должен находиться в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4113c-154">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="4113c-155">Чтобы найти свойства файла, получите **driveItem** для файла.</span><span class="sxs-lookup"><span data-stu-id="4113c-155">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="4113c-156">Например,/дривес/{ИД}/итемс/{ИД}.</span><span class="sxs-lookup"><span data-stu-id="4113c-156">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="4113c-157">Идентификатор вложения — это идентификатор GUID в элементе **ETag** объекта **DriveItem**, вложение **ContentURL** — это **webUrl** папки **driveItem**плюс имя **driveItem**, а имя вложения — имя **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="4113c-157">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "name": "Budget.docx"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="4113c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4113c-158">Response</span></span>

<span data-ttu-id="4113c-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4113c-159">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2/1589481435511?groupId=13a99602-a5d3-4fed-99d2-7dc3ffe3730d&tenantId=e5648b2b-1dea-445a-ab65-4f9326c2bd10&createdTime=1589481435511&parentMessageId=1589481435511",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "598efcd4-e549-402a-9602-0b50201faebe",
            "displayName": "MOD Administrator",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "content": null,
            "name": "Budget.docx",
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="4113c-160">См. также</span><span class="sxs-lookup"><span data-stu-id="4113c-160">See also</span></span>

- [<span data-ttu-id="4113c-161">Ссылки на карточки</span><span class="sxs-lookup"><span data-stu-id="4113c-161">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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
