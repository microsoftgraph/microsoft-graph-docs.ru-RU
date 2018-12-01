---
title: 'message: move'
description: Переместите сообщение в папку. Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.
ms.openlocfilehash: 3266eb93ab5d0fe95a3c1ba0dc8e5004b6302e03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028336"
---
# <a name="message-move"></a><span data-ttu-id="c43f3-104">message: move</span><span class="sxs-lookup"><span data-stu-id="c43f3-104">message: move</span></span>

<span data-ttu-id="c43f3-105">Переместите сообщение в папку.</span><span class="sxs-lookup"><span data-stu-id="c43f3-105">Move a message to a folder.</span></span> <span data-ttu-id="c43f3-106">Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="c43f3-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="c43f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c43f3-107">Permissions</span></span>

<span data-ttu-id="c43f3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c43f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c43f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c43f3-110">Permission type</span></span> | <span data-ttu-id="c43f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c43f3-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c43f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c43f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c43f3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c43f3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c43f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c43f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c43f3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c43f3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c43f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c43f3-116">Application</span></span> | <span data-ttu-id="c43f3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c43f3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c43f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c43f3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="c43f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c43f3-119">Request headers</span></span>

| <span data-ttu-id="c43f3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c43f3-120">Header</span></span> | <span data-ttu-id="c43f3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c43f3-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c43f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c43f3-122">Authorization</span></span> | <span data-ttu-id="c43f3-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c43f3-123"></span></span> <span data-ttu-id="c43f3-124">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c43f3-124">Required.</span></span> |
| <span data-ttu-id="c43f3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c43f3-125">Content-Type</span></span> | <span data-ttu-id="c43f3-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c43f3-126"></span></span> <span data-ttu-id="c43f3-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c43f3-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c43f3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c43f3-128">Request body</span></span>

<span data-ttu-id="c43f3-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c43f3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c43f3-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c43f3-130">Parameter</span></span>   | <span data-ttu-id="c43f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c43f3-131">Type</span></span> |<span data-ttu-id="c43f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c43f3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c43f3-133">destinationId</span><span class="sxs-lookup"><span data-stu-id="c43f3-133">destinationId</span></span>|<span data-ttu-id="c43f3-134">String</span><span class="sxs-lookup"><span data-stu-id="c43f3-134">String</span></span>|<span data-ttu-id="c43f3-135">Идентификатор папки назначения, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="c43f3-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="c43f3-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c43f3-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c43f3-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c43f3-137">Response</span></span>

<span data-ttu-id="c43f3-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c43f3-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c43f3-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c43f3-139">Example</span></span>

<span data-ttu-id="c43f3-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c43f3-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c43f3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="c43f3-141">Request</span></span>

<span data-ttu-id="c43f3-142">Следующий запрос перемещает указанное сообщение в папки «Удаленные», определяется именем известных папки `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="c43f3-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c43f3-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="c43f3-143">Response</span></span>

<span data-ttu-id="c43f3-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c43f3-144">Here is an example of the response.</span></span>

> <span data-ttu-id="c43f3-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="c43f3-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c43f3-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c43f3-146">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
