---
title: 'message: move'
description: Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения и удаляется исходное сообщение.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: baa03f7c2442c4ce624a5f581c699bfa4af63611
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511518"
---
# <a name="message-move"></a><span data-ttu-id="ed9f7-104">message: move</span><span class="sxs-lookup"><span data-stu-id="ed9f7-104">message: move</span></span>

<span data-ttu-id="ed9f7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed9f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed9f7-106">Перемещение сообщения в другую папку в почтовом ящике указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-106">Move a message to another folder within the specified user's mailbox.</span></span> <span data-ttu-id="ed9f7-107">При этом в целевой папке создается новая копия сообщения и удаляется исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-107">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed9f7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed9f7-108">Permissions</span></span>

<span data-ttu-id="ed9f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed9f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed9f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed9f7-111">Permission type</span></span> | <span data-ttu-id="ed9f7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed9f7-112">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ed9f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed9f7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ed9f7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed9f7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ed9f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed9f7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed9f7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed9f7-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ed9f7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed9f7-117">Application</span></span> | <span data-ttu-id="ed9f7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed9f7-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed9f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed9f7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="ed9f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed9f7-120">Request headers</span></span>

| <span data-ttu-id="ed9f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed9f7-121">Header</span></span> | <span data-ttu-id="ed9f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ed9f7-122">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ed9f7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed9f7-123">Authorization</span></span> | <span data-ttu-id="ed9f7-124">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-124">`Bearer {token}`.</span></span> <span data-ttu-id="ed9f7-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-125">Required.</span></span> |
| <span data-ttu-id="ed9f7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed9f7-126">Content-Type</span></span> | <span data-ttu-id="ed9f7-127">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-127">`application/json`.</span></span> <span data-ttu-id="ed9f7-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed9f7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed9f7-129">Request body</span></span>

<span data-ttu-id="ed9f7-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ed9f7-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ed9f7-131">Parameter</span></span>   | <span data-ttu-id="ed9f7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ed9f7-132">Type</span></span> |<span data-ttu-id="ed9f7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ed9f7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed9f7-134">destinationId</span><span class="sxs-lookup"><span data-stu-id="ed9f7-134">destinationId</span></span>|<span data-ttu-id="ed9f7-135">String</span><span class="sxs-lookup"><span data-stu-id="ed9f7-135">String</span></span>|<span data-ttu-id="ed9f7-136">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-136">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ed9f7-137">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ed9f7-137">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ed9f7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed9f7-138">Response</span></span>

<span data-ttu-id="ed9f7-139">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-139">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed9f7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ed9f7-140">Example</span></span>

<span data-ttu-id="ed9f7-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-141">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ed9f7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed9f7-142">Request</span></span>

<span data-ttu-id="ed9f7-143">Приведенный ниже запрос перемещает указанное сообщение в папку "Удаленные", указанную по ее известному имени `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-143">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed9f7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed9f7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```
# <a name="c"></a>[<span data-ttu-id="ed9f7-145">C#</span><span class="sxs-lookup"><span data-stu-id="ed9f7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-move-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed9f7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed9f7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-move-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed9f7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed9f7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-move-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed9f7-148">Java</span><span class="sxs-lookup"><span data-stu-id="ed9f7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-move-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed9f7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed9f7-149">Response</span></span>

<span data-ttu-id="ed9f7-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-150">Here is an example of the response.</span></span>

> <span data-ttu-id="ed9f7-151">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ed9f7-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed9f7-152">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#message",
    "@odata.type":"#microsoft.graph.message",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "createdDateTime":"2018-08-12T08:43:22Z",
    "lastModifiedDateTime":"2018-08-15T19:47:54Z",
    "changeKey":"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB",
    "categories":[

    ],
    "receivedDateTime":"2018-08-12T08:43:22Z",
    "sentDateTime":"2018-08-12T08:43:20Z",
    "hasAttachments":false,
    "internetMessageId":"<00535324-5988-4b6a-b9af-d44cf2d0b691@MWHPR2201MB1022.namprd22.prod.outlook.com>",
    "subject":"Undeliverable: Meet for lunch?",
    "bodyPreview":"Delivery has failed to these recipients or groups:\r\n\r\nfannyd@contoso.onmicrosoft.com (fannyd@contoso.onmicrosoft.com)\r\nYour message couldn't be delivered. Despite repeated attempts to deliver your message, querying the Domain Name System (DNS) for the rec",
    "importance":"normal",
    "parentFolderId":"AAMkADhAAAAAAEKAAA=",
    "conversationId":"AAQkADhJzfbkARFhe5kKhjihSA=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADhAAAW%2FVPeAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html></html>"
    },
    "sender":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Microsoft Outlook",
            "address":"MicrosoftExchange329e71ec88ae4615bbc36ab6ce41109e@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"fannyd@contoso.onmicrosoft.com",
                "address":"fannyd@contoso.onmicrosoft.com"
            }
        },
        {
            "emailAddress":{
                "name":"danas@contoso.onmicrosoft.com",
                "address":"danas@contoso.onmicrosoft.com"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
