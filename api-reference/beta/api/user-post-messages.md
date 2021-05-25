---
title: Создание объекта Message
description: Создайте черновик нового сообщения в формате JSON или MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: acb10508eec31e39d5f631aee91dc3b85f964d3d
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645572"
---
# <a name="create-message"></a><span data-ttu-id="2cada-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="2cada-103">Create Message</span></span>

<span data-ttu-id="2cada-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cada-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cada-105">Создайте черновик нового сообщения в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="2cada-105">Create a draft of a new message in either JSON or MIME format.</span></span>

<span data-ttu-id="2cada-106">При использовании формата JSON можно:</span><span class="sxs-lookup"><span data-stu-id="2cada-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="2cada-107">Включив [вложение.](../resources/attachment.md)</span><span class="sxs-lookup"><span data-stu-id="2cada-107">Include an [attachment](../resources/attachment.md).</span></span>
- <span data-ttu-id="2cada-108">Используйте [упоминание,](../resources/mention.md) чтобы вызвать другого пользователя в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="2cada-108">Use a [mention](../resources/mention.md) to call out another user in the new message.</span></span>
- <span data-ttu-id="2cada-109">[Обнови](../api/message-update.md) проект позже, чтобы добавить содержимое в **тело** или изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="2cada-109">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="2cada-110">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="2cada-110">When using MIME format:</span></span>
- <span data-ttu-id="2cada-111">Предоформим соответствующие заголовки интернет-сообщений и [содержимое MIME](https://tools.ietf.org/html/rfc2045), все закодированные в [](https://tools.ietf.org/html/rfc2076) **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2cada-111">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="2cada-112">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="2cada-112">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="2cada-113">По умолчанию эта операция сохраняет черновик в папке Черновики.</span><span class="sxs-lookup"><span data-stu-id="2cada-113">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="2cada-114">[Отправка](/graph/api-reference/beta/api/message-send.md) черновика сообщения в последующей операции.</span><span class="sxs-lookup"><span data-stu-id="2cada-114">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="2cada-115">Кроме того, [отправьте новое сообщение](../api/user-sendmail.md) в одном действии или [](../api/message-createreply.md) создайте [](../api/message-createreplyall.md) черновик для отправки, [](../api/message-createforward.md)чтобы ответить или ответить всем на существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="2cada-115">Alternatively, [send a new message](../api/user-sendmail.md) in a single action, or create a draft [to forward](../api/message-createforward.md), [to reply](../api/message-createreply.md) or [to reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cada-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cada-116">Permissions</span></span>
<span data-ttu-id="2cada-117">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2cada-117">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="2cada-118">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cada-118">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cada-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cada-119">Permission type</span></span>      | <span data-ttu-id="2cada-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cada-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cada-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cada-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2cada-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cada-122">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2cada-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cada-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cada-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cada-124">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2cada-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cada-125">Application</span></span> | <span data-ttu-id="2cada-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cada-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cada-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cada-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="2cada-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cada-128">Request headers</span></span>
| <span data-ttu-id="2cada-129">Имя</span><span class="sxs-lookup"><span data-stu-id="2cada-129">Name</span></span>       | <span data-ttu-id="2cada-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2cada-130">Type</span></span> | <span data-ttu-id="2cada-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2cada-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cada-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cada-132">Authorization</span></span>  | <span data-ttu-id="2cada-133">string</span><span class="sxs-lookup"><span data-stu-id="2cada-133">string</span></span>  | <span data-ttu-id="2cada-134">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2cada-134">Bearer {token}.</span></span>|
| <span data-ttu-id="2cada-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cada-135">Content-Type</span></span> | <span data-ttu-id="2cada-136">string</span><span class="sxs-lookup"><span data-stu-id="2cada-136">string</span></span>  | <span data-ttu-id="2cada-p102">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cada-p102">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="2cada-139">Использование `application/json` объекта JSON и `text/plain` контента MIME</span><span class="sxs-lookup"><span data-stu-id="2cada-139">Use `application/json` for a JSON object and `text/plain` for MIME content</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cada-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cada-140">Request body</span></span>
<span data-ttu-id="2cada-141">При использовании формата JSON предоформим JSON-представление объекта [сообщения.](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="2cada-141">When using JSON format, provide a JSON representation of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="2cada-142">При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными интернет-сообщениями ("To", "CC", "BCC", "Subject"), все закодированные в **формате base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="2cada-142">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="2cada-143">Чтобы использовать **упоминание,** чтобы вызвать другого пользователя в новом сообщении:</span><span class="sxs-lookup"><span data-stu-id="2cada-143">To use **mention** to call out another user in the new message:</span></span>
- <span data-ttu-id="2cada-144">Включай в текст запроса обязательное свойство **toRecipients,** свойство **mentions** и любые полезные свойства сообщений.</span><span class="sxs-lookup"><span data-stu-id="2cada-144">Include the required **toRecipients** property, the **mentions** property, and any writable message properties in the request body.</span></span>
- <span data-ttu-id="2cada-145">Для каждого упоминания в **свойстве упоминаний** необходимо указать **упомянутое** свойство.</span><span class="sxs-lookup"><span data-stu-id="2cada-145">For each mention in the **mentions** property, you must specify the **mentioned** property.</span></span>

<span data-ttu-id="2cada-146">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="2cada-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>


## <a name="response"></a><span data-ttu-id="2cada-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cada-147">Response</span></span>

<span data-ttu-id="2cada-148">В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [сообщения](../resources/message.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2cada-148">If successful, this method returns a `201 Created` response code and a [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="2cada-149">Если в тексте запроса содержится неправильное содержимое MIME, этот метод возвращается и следующее сообщение об ошибке: "Недействительные строки `400 Bad request` base64 для контента MIME".</span><span class="sxs-lookup"><span data-stu-id="2cada-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="2cada-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="2cada-150">Examples</span></span>
### <a name="example-1-create-a-message-draft-in-json-format"></a><span data-ttu-id="2cada-151">Пример 1. Создание черновика сообщений в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2cada-151">Example 1: Create a message draft in JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="2cada-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cada-152">Request</span></span>
<span data-ttu-id="2cada-153">Вот пример запроса на создание черновика нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="2cada-153">Here is an example of the request to create a draft of a new message.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cada-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cada-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"Did you see last night's game?",
    "importance":"Low",
    "body":{
        "contentType":"HTML",
        "content":"They were <b>awesome</b>!"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="2cada-155">C#</span><span class="sxs-lookup"><span data-stu-id="2cada-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cada-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cada-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cada-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cada-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cada-158">Java</span><span class="sxs-lookup"><span data-stu-id="2cada-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2cada-159">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cada-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="2cada-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cada-160">Response</span></span>
<span data-ttu-id="2cada-p103">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cada-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('ad787b4f-1fda-4523-8e48-ffedb7f4635f')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t\"",
    "id":"AAMkAGRWAAAFSmKXAAA=",
    "createdDateTime":"2017-12-23T07:29:57Z",
    "lastModifiedDateTime":"2017-12-23T07:29:58Z",
    "changeKey":"CQAAABYAAAAmXr9SsE/UR4PcnTZcg7qWAAAFS12t",
    "categories":[

    ],
    "receivedDateTime":"2017-12-23T07:29:58Z",
    "sentDateTime":"2017-12-23T07:29:58Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR130@MWHPR130.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkAGRWAAAAAAEPAAA=",
    "conversationId":"AAQkAGRVYAsRJrRdc_mWNaxU=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkAGRWAAAFSmKXAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"AdeleV@contoso.onmicrosoft.com",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-2-create-a-draft-message-that-includes-an--mention"></a><span data-ttu-id="2cada-163">Пример 2. Создание черновика сообщения с упоминанием @</span><span class="sxs-lookup"><span data-stu-id="2cada-163">Example 2: Create a draft message that includes an @-mention</span></span>
#### <a name="request"></a><span data-ttu-id="2cada-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cada-164">Request</span></span>
<span data-ttu-id="2cada-165">В следующем примере показан черновик электронной почты Ранди Уэлч в Samantha Booth.</span><span class="sxs-lookup"><span data-stu-id="2cada-165">The next example shows a draft email by Randi Welch to Samantha Booth.</span></span> <span data-ttu-id="2cada-166">В сообщении также содержится упоминание другого пользователя, Даны Swope.</span><span class="sxs-lookup"><span data-stu-id="2cada-166">The message also includes a mention of another user, Dana Swope.</span></span>

<span data-ttu-id="2cada-167">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cada-167">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cada-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cada-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_mentions_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject": "Party planning",
    "toRecipients":[
      {
          "emailAddress":{
              "name":"Samantha Booth",
              "address":"samanthab@contoso.onmicrosoft.com"
          }
      }
    ],
    "mentions":[
      {    
        "mentioned":{
          "name":"Dana Swope",
          "address":"danas@contoso.onmicrosoft.com"
         }
      }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="2cada-169">C#</span><span class="sxs-lookup"><span data-stu-id="2cada-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-mentions-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cada-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cada-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-mentions-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cada-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cada-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-mentions-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cada-172">Java</span><span class="sxs-lookup"><span data-stu-id="2cada-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-mentions-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2cada-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cada-173">Response</span></span>
<span data-ttu-id="2cada-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cada-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/Messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAbYj7\"",
  "id":"AQMkADJmMTUAAAW1fsAAAAA==",
  "body":{
    "contentType":"Text",
    "content":""
  },
  "bodyPreview":"",
  "sender":null,
  "from":null,
  "subject": "Party planning",
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      }
    }
  ],
  "mentionsPreview":{
    "isMentioned":false
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAW1fsAAAAA%3D%3D')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAW1fsAAAAA==')/mentions('4577bba4-b063-4cea-9073-6f7ca815fcec')",
      "id":"4577bba4-b063-4cea-9073-6f7ca815fcec",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-22T02:22:44Z",
      "serverCreatedDateTime":"2016-07-22T02:22:44.201Z",
      "deepLink":null,
      "application":null
    }
  ]
}

```

### <a name="example-3-create-a-draft-message-that-includes-custom-internet-message-headers"></a><span data-ttu-id="2cada-177">Пример 3. Создание черновика сообщения, которое включает настраиваемые заглавные сообщения в Интернете</span><span class="sxs-lookup"><span data-stu-id="2cada-177">Example 3: Create a draft message that includes custom Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="2cada-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cada-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2cada-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cada-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages
Content-type: application/json

{
    "subject":"9/8/2018: concert",
    "body":{
        "contentType":"HTML",
        "content":"The group represents Washington."
    },
    "toRecipients":[
        {
            "emailAddress":{
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "internetMessageHeaders":[
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="2cada-180">C#</span><span class="sxs-lookup"><span data-stu-id="2cada-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cada-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cada-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cada-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cada-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cada-183">Java</span><span class="sxs-lookup"><span data-stu-id="2cada-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2cada-184">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cada-184">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="2cada-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cada-185">Response</span></span>
<span data-ttu-id="2cada-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2cada-186">Here is an example of the response.</span></span> <span data-ttu-id="2cada-187">Примечание. Заголовки сообщений Интернета не возвращаются по умолчанию в ответе POST.</span><span class="sxs-lookup"><span data-stu-id="2cada-187">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="2cada-188">Примечание. Представленный здесь объект отклика также может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2cada-188">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="2cada-189">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cada-189">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_message_with_headers_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE\"",
    "id":"AAMkADhNmAAA=",
    "createdDateTime":"2018-09-09T02:54:56Z",
    "lastModifiedDateTime":"2018-09-09T02:54:56Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuE",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T02:54:56Z",
    "sentDateTime":"2018-09-09T02:54:56Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR220MB1120.namprd22.prod.outlook.com>",
    "subject":"9/8/2018: concert",
    "bodyPreview":"The group represents Washington.",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEPAAA=",
    "conversationId":"AAQkADhNCuP8OKSm-0NE=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhNmAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "mentionsPreview":null,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Washington.\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-4-create-a-message-draft-in-mime-format"></a><span data-ttu-id="2cada-190">Пример 4. Создание черновика сообщения в формате MIME</span><span class="sxs-lookup"><span data-stu-id="2cada-190">Example 4: Create a message draft in MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="2cada-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cada-191">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_create_draft_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM6IEludGVybmFsIFJlc3VtZSBTdWJtaXNzaW9uOiBT
YWxlcyBBc3NvY2lhdGUKVGhyZWFkLUluZGV4OiBjb2RlY29kZWNvZGVoZXJlaGVyZWhlcmUKRGF0
ZTogU3VuLCAyOCBGZWIgMjAyMSAwNzoxNTowMCArMDAwMApNZXNzYWdlLUlEOgoJPE1XSFBSMTMw
MU1CMjAwMDAwMDAwRDc2RDlDMjgyMjAwMDA5QUQ5QTlASFdIUFIxMzAxTUIwMDAwLmNvZGVudW0u
cHJvZC5vdXRsb29rLmNvbT4KQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1IYXMtQXR0YWNo
OgpYLU1TLVRORUYtQ29ycmVsYXRv
```

#### <a name="response"></a><span data-ttu-id="2cada-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cada-192">Response</span></span>
<span data-ttu-id="2cada-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2cada-193">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.message",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('0aaa0aa0-0000-0a00-a00a-0000009000a0')/messages/$entity",
    "@odata.etag": "W/\"AAAAAAAAAAAa00AAAa0aAaAa0a0AAAaAAAAaAa0a\"",
    "id": "AAMkADA1MTAAAAqldOAAA=",
    "createdDateTime": "2021-04-23T18:13:44Z",
    "lastModifiedDateTime": "2021-04-23T18:13:44Z",
    "changeKey": "AAAAAAAAAAAA00aaaa000aaA",
    "categories": [],
    "receivedDateTime": "2021-04-23T18:13:44Z",
    "sentDateTime": "2021-02-28T07:15:00Z",
    "hasAttachments": false,
    "internetMessageId": "<AAAAAAAAAA@AAAAAAA0001AA0000.codcod00.prod.outlook.com>",
    "subject": "Internal Resume Submission: Sales Associate",
    "bodyPreview": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here...",
    "importance": "normal",
    "parentFolderId": "LKJDSKJHkjhfakKJHFKWKKJHKJdhkjHDK==",
    "conversationId": "SDSFSmFSDGI5LWZhYjc4fsdfsd=",
    "conversationIndex": "Adfsdfsdfsdfw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": true,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkAGNhOWAvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "body": {
        "contentType": "text",
        "content": "Hi, Megan.I have an interest in the Sales Associate position. Please consider my resume, which you can access here... Regards,Alex"
    },
    "sender": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

<span data-ttu-id="2cada-194">Если в тексте запроса содержится недооформленное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2cada-194">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

## <a name="see-also"></a><span data-ttu-id="2cada-195">См. также</span><span class="sxs-lookup"><span data-stu-id="2cada-195">See also</span></span>

- [<span data-ttu-id="2cada-196">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="2cada-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2cada-197">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2cada-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2cada-198">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2cada-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
