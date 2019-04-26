---
title: 'message: move'
description: Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения и удаляется исходное сообщение.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c30c6b55f1abceabd093b25b4b551b8c66d91d11
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333175"
---
# <a name="message-move"></a><span data-ttu-id="ca69b-104">message: move</span><span class="sxs-lookup"><span data-stu-id="ca69b-104">message: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca69b-105">Перемещение сообщения в папку.</span><span class="sxs-lookup"><span data-stu-id="ca69b-105">Move a message to a folder.</span></span> <span data-ttu-id="ca69b-106">При этом в целевой папке создается новая копия сообщения и удаляется исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="ca69b-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca69b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca69b-107">Permissions</span></span>

<span data-ttu-id="ca69b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca69b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca69b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca69b-110">Permission type</span></span> | <span data-ttu-id="ca69b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca69b-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="ca69b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca69b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca69b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca69b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca69b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca69b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca69b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca69b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca69b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca69b-116">Application</span></span> | <span data-ttu-id="ca69b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca69b-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca69b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca69b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="ca69b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca69b-119">Request headers</span></span>

| <span data-ttu-id="ca69b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca69b-120">Header</span></span> | <span data-ttu-id="ca69b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ca69b-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="ca69b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca69b-122">Authorization</span></span> | <span data-ttu-id="ca69b-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="ca69b-123">`Bearer {token}`.</span></span> <span data-ttu-id="ca69b-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ca69b-124">Required.</span></span> |
| <span data-ttu-id="ca69b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca69b-125">Content-Type</span></span> | <span data-ttu-id="ca69b-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="ca69b-126">`application/json`.</span></span> <span data-ttu-id="ca69b-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ca69b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca69b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca69b-128">Request body</span></span>

<span data-ttu-id="ca69b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ca69b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca69b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca69b-130">Parameter</span></span>   | <span data-ttu-id="ca69b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca69b-131">Type</span></span> |<span data-ttu-id="ca69b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca69b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca69b-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="ca69b-133">DestinationId</span></span>|<span data-ttu-id="ca69b-134">String</span><span class="sxs-lookup"><span data-stu-id="ca69b-134">String</span></span>|<span data-ttu-id="ca69b-135">Идентификатор целевой папки либо имя известной папки.</span><span class="sxs-lookup"><span data-stu-id="ca69b-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="ca69b-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ca69b-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ca69b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca69b-137">Response</span></span>

<span data-ttu-id="ca69b-138">В случае успеха этот метод возвращает код отклика `201 Created` и ресурс [message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca69b-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca69b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ca69b-139">Example</span></span>

<span data-ttu-id="ca69b-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ca69b-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ca69b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca69b-141">Request</span></span>

<span data-ttu-id="ca69b-142">Приведенный ниже запрос перемещает указанное сообщение в папку "Удаленные", указанную по ее известному имени `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="ca69b-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAATs28OAAA="],
  "name": "message_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADhAAATs28OAAA=/move
Content-type: application/json

{
  "destinationId": "deleteditems"
}
```

##### <a name="response"></a><span data-ttu-id="ca69b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca69b-143">Response</span></span>

<span data-ttu-id="ca69b-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca69b-144">Here is an example of the response.</span></span>

> <span data-ttu-id="ca69b-145">**Примечание.**  Представленный здесь объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca69b-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ca69b-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca69b-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#message",
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
<!--
{
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
