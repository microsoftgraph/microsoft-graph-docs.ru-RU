---
title: Создание сообщения
description: Создание черновика нового сообщения в формате JSON или MIME.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d10c07c433b3d8456c574519aa497fc163dde09
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645635"
---
# <a name="create-message"></a><span data-ttu-id="35255-103">Создание сообщения</span><span class="sxs-lookup"><span data-stu-id="35255-103">Create message</span></span>

<span data-ttu-id="35255-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35255-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35255-105">Создание черновика нового [сообщения](../resources/message.md) в формате JSON или MIME.</span><span class="sxs-lookup"><span data-stu-id="35255-105">Create a draft of a new [message](../resources/message.md) in either JSON or MIME format.</span></span>

<span data-ttu-id="35255-106">При использовании формата JSON можно:</span><span class="sxs-lookup"><span data-stu-id="35255-106">When using JSON format, you can:</span></span>
- <span data-ttu-id="35255-107">Включать [вложение](../resources/attachment.md) в **сообщение**.</span><span class="sxs-lookup"><span data-stu-id="35255-107">Include an [attachment](../resources/attachment.md) to the **message**.</span></span>
- <span data-ttu-id="35255-108">[Обновите](../api/message-update.md) черновике позже, чтобы добавить **текст** или изменить другие свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="35255-108">[Update](../api/message-update.md) the draft later to add content to the **body** or change other message properties.</span></span>

<span data-ttu-id="35255-109">При использовании формата MIME:</span><span class="sxs-lookup"><span data-stu-id="35255-109">When using MIME format:</span></span>
- <span data-ttu-id="35255-110">Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="35255-110">Provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), all encoded in **base64** format in the request body.</span></span>
- <span data-ttu-id="35255-111">Добавьте все вложения и свойства S/MIME в содержимое MIME.</span><span class="sxs-lookup"><span data-stu-id="35255-111">Add any attachments and S/MIME properties to the MIME content.</span></span>

<span data-ttu-id="35255-112">По умолчанию эта операция сохраняет черновик в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="35255-112">By default, this operation saves the draft in the Drafts folder.</span></span>

<span data-ttu-id="35255-113">[Отправьте](/graph/api-reference/beta/api/message-send.md) черновик сообщения в ходе последующей операции.</span><span class="sxs-lookup"><span data-stu-id="35255-113">[Send](/graph/api-reference/beta/api/message-send.md) the draft message in a subsequent operation.</span></span>

<span data-ttu-id="35255-114">Или [отправьте новое сообщение](../api/user-sendmail.md) за одну операцию или создайте черновик для [пересылки](../api/message-createforward.md), [ответа](../api/message-createreply.md) и [ответа всем](../api/message-createreplyall.md) на существующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="35255-114">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation, or create a draft to [forward](../api/message-createforward.md), [reply](../api/message-createreply.md) and [reply-all](../api/message-createreplyall.md) to an existing message.</span></span>

## <a name="permissions"></a><span data-ttu-id="35255-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35255-115">Permissions</span></span>
<span data-ttu-id="35255-116">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="35255-116">One of the following permissions are required to call this API.</span></span> <span data-ttu-id="35255-117">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35255-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35255-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35255-118">Permission type</span></span>      | <span data-ttu-id="35255-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35255-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35255-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35255-120">Delegated (work or school account)</span></span> | <span data-ttu-id="35255-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35255-121">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35255-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35255-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35255-123">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35255-123">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="35255-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35255-124">Application</span></span> | <span data-ttu-id="35255-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35255-125">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35255-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35255-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="35255-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35255-127">Request headers</span></span>
| <span data-ttu-id="35255-128">Имя</span><span class="sxs-lookup"><span data-stu-id="35255-128">Name</span></span>       | <span data-ttu-id="35255-129">Тип</span><span class="sxs-lookup"><span data-stu-id="35255-129">Type</span></span> | <span data-ttu-id="35255-130">Описание</span><span class="sxs-lookup"><span data-stu-id="35255-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="35255-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="35255-131">Authorization</span></span>  | <span data-ttu-id="35255-132">string</span><span class="sxs-lookup"><span data-stu-id="35255-132">string</span></span>  | <span data-ttu-id="35255-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35255-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35255-135">Content-Length</span><span class="sxs-lookup"><span data-stu-id="35255-135">Content-Length</span></span> | <span data-ttu-id="35255-136">число</span><span class="sxs-lookup"><span data-stu-id="35255-136">number</span></span> | <span data-ttu-id="35255-137">0. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35255-137">0. Required.</span></span> |
| <span data-ttu-id="35255-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35255-138">Content-Type</span></span> | <span data-ttu-id="35255-139">string</span><span class="sxs-lookup"><span data-stu-id="35255-139">string</span></span>  | <span data-ttu-id="35255-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35255-p103">Nature of the data in the body of an entity. Required. </span></span><br/> <span data-ttu-id="35255-142">Используйте `application/json` для объекта JSON и `text/plain` для содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="35255-142">Use `application/json` for a JSON object and `text/plain` for MIME content.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35255-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35255-143">Request body</span></span>
<span data-ttu-id="35255-144">При использовании формата JSON предоставьте представление JSON объекта [Message](../resources/message.md).</span><span class="sxs-lookup"><span data-stu-id="35255-144">When using JSON format, provide a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="35255-145">При указании текста в формате MIME укажите содержимое MIME с применимыми заголовками сообщений Интернета ("Кому", "Копия", "Скрытая копия", "Тема"), все закодированные сообщения в формате **Base64** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="35255-145">When specifying the body in MIME format, provide the MIME content with the applicable Internet message headers ("To", "CC", "BCC", "Subject"), all encoded in **base64** format in the request body.</span></span>

<span data-ttu-id="35255-146">Так как ресурс **message** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными в сообщение при его создании.</span><span class="sxs-lookup"><span data-stu-id="35255-146">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="35255-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="35255-147">Response</span></span>

<span data-ttu-id="35255-148">В случае успеха этот метод возвращает код отклика `201 Created` и объект [message](../resources/message.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35255-148">If successful, this method returns `201 Created` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="35255-149">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".</span><span class="sxs-lookup"><span data-stu-id="35255-149">If the request body includes malformed MIME content, this method returns `400 Bad request` and the following error message: "Invalid base64 string for MIME content".</span></span>

## <a name="examples"></a><span data-ttu-id="35255-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="35255-150">Examples</span></span>
### <a name="example-1-create-a-new-message-draft-using-json-format"></a><span data-ttu-id="35255-151">Пример 1. Создание черновика сообщения в формате JSON</span><span class="sxs-lookup"><span data-stu-id="35255-151">Example 1: Create a new message draft using JSON format</span></span>
#### <a name="request"></a><span data-ttu-id="35255-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="35255-152">Request</span></span> 
<span data-ttu-id="35255-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35255-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35255-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="35255-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
# <a name="c"></a>[<span data-ttu-id="35255-155">C#</span><span class="sxs-lookup"><span data-stu-id="35255-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35255-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35255-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35255-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35255-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35255-158">Java</span><span class="sxs-lookup"><span data-stu-id="35255-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="35255-159">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35255-159">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="35255-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="35255-160">Response</span></span> 
<span data-ttu-id="35255-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35255-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti\"",
    "id":"AAMkADNlNYjSAAA=",
    "createdDateTime":"2017-07-22T01:53:56Z",
    "lastModifiedDateTime":"2017-07-22T01:53:57Z",
    "changeKey":"CQAAABYAAABK4UfANE/UR5clSilZtIuWAAC1vdti",
    "categories":[

    ],
    "receivedDateTime":"2017-07-22T01:53:57Z",
    "sentDateTime":"2017-07-22T01:53:57Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB@MWHPR1301MB.namprd13.prod.outlook.com>",
    "subject":"Did you see last night's game?",
    "bodyPreview":"They were awesome!",
    "importance":"low",
    "parentFolderId":"AAMkADNlNWAAAAAAEPAAA=",
    "conversationId":"AAQkADNlNFdXGBnqtY=",
    "conversationIndex":"AQHTe7/VAniOJVgCxEmtF1z6ZY1rFQ==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":true,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADNlNYjSAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThey were <b>awesome</b>!\r\n</body>\r\n</html>\r\n"
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

### <a name="example-2-create-message-draft-that-includes-custom-message-headers"></a><span data-ttu-id="35255-163">Пример 2. Создание черновика сообщения, который включает настраиваемые заголовки</span><span class="sxs-lookup"><span data-stu-id="35255-163">Example 2: Create message draft that includes custom message headers</span></span>
#### <a name="request"></a><span data-ttu-id="35255-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="35255-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="35255-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="35255-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_message_with_headers_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
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
# <a name="c"></a>[<span data-ttu-id="35255-166">C#</span><span class="sxs-lookup"><span data-stu-id="35255-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-message-with-headers-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35255-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35255-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-message-with-headers-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35255-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35255-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-message-with-headers-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35255-169">Java</span><span class="sxs-lookup"><span data-stu-id="35255-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-message-with-headers-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="35255-170">Предоставьте в теле запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35255-170">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="35255-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="35255-171">Response</span></span>
<span data-ttu-id="35255-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35255-172">Here is an example of the response.</span></span> <span data-ttu-id="35255-173">Примечание. Заголовки сообщений Интернета не возвращаются по умолчанию в ответе POST.</span><span class="sxs-lookup"><span data-stu-id="35255-173">Note: Internet message headers are not returned by default in a POST response.</span></span> <span data-ttu-id="35255-174">Примечание. Представленный здесь объект отклика также может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="35255-174">The response object shown here may also be truncated for brevity.</span></span> <span data-ttu-id="35255-175">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35255-175">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
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

### <a name="example-3-create-a-new-message-draft-using-mime-format"></a><span data-ttu-id="35255-176">Пример 3. Создание черновика сообщения в формате MIME</span><span class="sxs-lookup"><span data-stu-id="35255-176">Example 3: Create a new message draft using MIME format</span></span>
#### <a name="request"></a><span data-ttu-id="35255-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="35255-177">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "message_create_draft_mime_v1"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: text/plain

Q29udGVudC1UeXBlOiBhcHBsaWNhdGlvbi9wa2NzNy1taW1lOw0KCW5hbWU9c21pbWUucDdtOw0KCXNtaW1lLXR5cGU9ZW52ZWxvcGVkLWRhdGENCk1pbWUtVmVyc2lvbjogMS4wIChNYWMgT1MgWCBNYWlsIDEzLjAgXCgzNjAxLjAuMTBcKSkNClN1YmplY3Q6IFJlOiBUZXN0aW5nIFMvTUlNRQ0KQ29udGVudC1EaXNwb3Np...

```

#### <a name="response"></a><span data-ttu-id="35255-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="35255-178">Response</span></span>
<span data-ttu-id="35255-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35255-179">Here is an example of the response.</span></span>
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

<span data-ttu-id="35255-180">Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="35255-180">If the request body includes malformed MIME content, this method returns the following error message.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="35255-181">См. также</span><span class="sxs-lookup"><span data-stu-id="35255-181">See also</span></span>

- [<span data-ttu-id="35255-182">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="35255-182">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="35255-183">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="35255-183">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

