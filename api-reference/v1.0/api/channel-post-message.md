---
title: Создание объекта chatMessage в канале
description: Создайте новый chatMessage в указанном канале.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a40f4f34b8eda962a9ce7b80fefa6b4c5b372d26
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202785"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="c1694-103">Создание объекта chatMessage в канале</span><span class="sxs-lookup"><span data-stu-id="c1694-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="c1694-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1694-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1694-105">Создайте [новый chatMessage](../resources/chatmessage.md) в указанном [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="c1694-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="c1694-106">**Примечание.** Мы не рекомендуем использовать этот API для переноса данных.</span><span class="sxs-lookup"><span data-stu-id="c1694-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="c1694-107">Он не имеет пропускной способности, необходимой для обычной миграции.</span><span class="sxs-lookup"><span data-stu-id="c1694-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1694-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1694-108">Permissions</span></span>

<span data-ttu-id="c1694-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1694-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1694-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1694-111">Permission type</span></span>                        | <span data-ttu-id="c1694-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1694-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1694-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1694-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1694-114">ChannelMessage.Send, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1694-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c1694-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1694-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1694-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1694-116">Not supported.</span></span> |
| <span data-ttu-id="c1694-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1694-117">Application</span></span>                            | <span data-ttu-id="c1694-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="c1694-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="c1694-119">**Примечание.** Разрешения приложений *поддерживаются только* для [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="c1694-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="c1694-120">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества импортированных данных.</span><span class="sxs-lookup"><span data-stu-id="c1694-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="c1694-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="c1694-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1694-122">Request headers</span></span>

| <span data-ttu-id="c1694-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c1694-123">Name</span></span>          | <span data-ttu-id="c1694-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c1694-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1694-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1694-125">Authorization</span></span> | <span data-ttu-id="c1694-126">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c1694-126">Bearer {code}.</span></span> <span data-ttu-id="c1694-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c1694-127">Required.</span></span> |
| <span data-ttu-id="c1694-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1694-128">Content-type</span></span> | <span data-ttu-id="c1694-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1694-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1694-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1694-131">Request body</span></span>

<span data-ttu-id="c1694-132">В теле запроса поставляем JSON-представление [объекта chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c1694-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="c1694-133">Обязательным является только свойство body, другие свойства необязательны.</span><span class="sxs-lookup"><span data-stu-id="c1694-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="c1694-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-134">Response</span></span>

<span data-ttu-id="c1694-135">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект chatMessage](../resources/chatmessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c1694-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1694-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1694-136">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="c1694-137">Пример 1. Hello World</span><span class="sxs-lookup"><span data-stu-id="c1694-137">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-138">Request</span></span>

<span data-ttu-id="c1694-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-139">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```


#### <a name="response"></a><span data-ttu-id="c1694-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-140">Response</span></span>

<span data-ttu-id="c1694-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1694-141">The following is an example of the response.</span></span>

> <span data-ttu-id="c1694-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1694-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-2-mentions"></a><span data-ttu-id="c1694-144">Пример 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="c1694-144">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-145">Request</span></span>
<span data-ttu-id="c1694-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1694-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1694-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="c1694-148">C#</span><span class="sxs-lookup"><span data-stu-id="c1694-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1694-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1694-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1694-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1694-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1694-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-151">Response</span></span>

<span data-ttu-id="c1694-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1694-152">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-3-cards"></a><span data-ttu-id="c1694-153">Пример 3. Карты</span><span class="sxs-lookup"><span data-stu-id="c1694-153">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-154">Request</span></span>
<span data-ttu-id="c1694-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-155">The following is an example of the request.</span></span>

><span data-ttu-id="c1694-156">**Примечание:** ID вложения должен быть уникальным и может быть новым случайно созданным GUID.</span><span class="sxs-lookup"><span data-stu-id="c1694-156">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="c1694-157">Однако, ID вложения должен быть одинаковым в элементах _тела_ и _вложений._</span><span class="sxs-lookup"><span data-stu-id="c1694-157">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1694-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1694-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="c1694-159">C#</span><span class="sxs-lookup"><span data-stu-id="c1694-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1694-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1694-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1694-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1694-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1694-162">Java</span><span class="sxs-lookup"><span data-stu-id="c1694-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1694-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-163">Response</span></span>

<span data-ttu-id="c1694-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1694-164">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-4-file-attachments"></a><span data-ttu-id="c1694-165">Пример 4. Вложения файлов</span><span class="sxs-lookup"><span data-stu-id="c1694-165">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-166">Request</span></span>
<span data-ttu-id="c1694-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-167">The following is an example of the request.</span></span>

><span data-ttu-id="c1694-168">**Примечание:** Файл уже должен быть в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c1694-168">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="c1694-169">Чтобы найти свойства файла, получите **driveItem** для файла.</span><span class="sxs-lookup"><span data-stu-id="c1694-169">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="c1694-170">Например, /drives/{id}/items/{id}.</span><span class="sxs-lookup"><span data-stu-id="c1694-170">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="c1694-171">Ваш ИД вложения — это GUID в **eTag** **driveItem,** содержимое вложения — это **webUrl** папки driveItem плюс имя **driveItem,** а имя вложения — имя  **driveItem.** </span><span class="sxs-lookup"><span data-stu-id="c1694-171">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1694-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1694-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="c1694-173">C#</span><span class="sxs-lookup"><span data-stu-id="c1694-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1694-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1694-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1694-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1694-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1694-176">Java</span><span class="sxs-lookup"><span data-stu-id="c1694-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1694-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-177">Response</span></span>

<span data-ttu-id="c1694-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1694-178">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime":"2020-07-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-5-import-messages"></a><span data-ttu-id="c1694-179">Пример 5. Импорт сообщений</span><span class="sxs-lookup"><span data-stu-id="c1694-179">Example 5: Import messages</span></span>

> <span data-ttu-id="c1694-180">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="c1694-180">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-181">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c1694-182">В следующем примере покажите, как импортировать сообщения с использованием ключей и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-182">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "deleted":false,
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
   },
}
```

#### <a name="response"></a><span data-ttu-id="c1694-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-183">Response</span></span>

<span data-ttu-id="c1694-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1694-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-6-import-messages-with-inline-images"></a><span data-ttu-id="c1694-185">Пример 6. Импорт сообщений с помощью inline-изображений</span><span class="sxs-lookup"><span data-stu-id="c1694-185">Example 6: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="c1694-186">В настоящее время inline images are the only media type supported by the import message API schpi.</span><span class="sxs-lookup"><span data-stu-id="c1694-186">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="c1694-187">**Примечание.** Область `Teamwork.Migrate.All` разрешений требуется для этого сценария.</span><span class="sxs-lookup"><span data-stu-id="c1694-187">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c1694-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1694-188">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c1694-189">В следующем примере показано, как импортировать сообщения, содержащие inline-изображения с помощью клавиш и ключей в `createDateTime` `from` тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c1694-189">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
{
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

#### <a name="response"></a><span data-ttu-id="c1694-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1694-190">Response</span></span>

<span data-ttu-id="c1694-191">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1694-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="c1694-192">См. также</span><span class="sxs-lookup"><span data-stu-id="c1694-192">See also</span></span>

* [<span data-ttu-id="c1694-193">Ссылки на карточки</span><span class="sxs-lookup"><span data-stu-id="c1694-193">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)
* [<span data-ttu-id="c1694-194">Импорт сообщений из сторонних платформ в Teams с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c1694-194">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="c1694-195">Создание канала</span><span class="sxs-lookup"><span data-stu-id="c1694-195">Create channel</span></span>](channel-post.md)

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

