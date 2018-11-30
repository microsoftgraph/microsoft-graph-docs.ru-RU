---
title: 'message: move'
description: Переместите сообщение в папку. Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.
ms.openlocfilehash: ea05cf2d07a9dc0719c4485f9dd940a0cc96ed24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080620"
---
# <a name="message-move"></a><span data-ttu-id="3a2c0-104">message: move</span><span class="sxs-lookup"><span data-stu-id="3a2c0-104">message: move</span></span>

> <span data-ttu-id="3a2c0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a2c0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a2c0-107">Переместите сообщение в папку.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-107">Move a message to a folder.</span></span> <span data-ttu-id="3a2c0-108">Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-108">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a2c0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2c0-109">Permissions</span></span>

<span data-ttu-id="3a2c0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a2c0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a2c0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2c0-112">Permission type</span></span> | <span data-ttu-id="3a2c0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a2c0-113">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="3a2c0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a2c0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3a2c0-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2c0-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a2c0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a2c0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a2c0-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2c0-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3a2c0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a2c0-118">Application</span></span> | <span data-ttu-id="3a2c0-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a2c0-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a2c0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a2c0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="3a2c0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a2c0-121">Request headers</span></span>

| <span data-ttu-id="3a2c0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a2c0-122">Header</span></span> | <span data-ttu-id="3a2c0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3a2c0-123">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="3a2c0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a2c0-124">Authorization</span></span> | <span data-ttu-id="3a2c0-125">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-125"></span></span> <span data-ttu-id="3a2c0-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-126">Required.</span></span> |
| <span data-ttu-id="3a2c0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a2c0-127">Content-Type</span></span> | <span data-ttu-id="3a2c0-128">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-128"></span></span> <span data-ttu-id="3a2c0-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a2c0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a2c0-130">Request body</span></span>

<span data-ttu-id="3a2c0-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a2c0-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a2c0-132">Parameter</span></span>   | <span data-ttu-id="3a2c0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3a2c0-133">Type</span></span> |<span data-ttu-id="3a2c0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2c0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a2c0-135">DestinationId</span><span class="sxs-lookup"><span data-stu-id="3a2c0-135">DestinationId</span></span>|<span data-ttu-id="3a2c0-136">String</span><span class="sxs-lookup"><span data-stu-id="3a2c0-136">String</span></span>|<span data-ttu-id="3a2c0-137">Идентификатор папки назначения, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-137">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="3a2c0-138">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3a2c0-138">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3a2c0-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a2c0-139">Response</span></span>

<span data-ttu-id="3a2c0-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-140">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a2c0-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3a2c0-141">Example</span></span>

<span data-ttu-id="3a2c0-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3a2c0-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a2c0-143">Request</span></span>

<span data-ttu-id="3a2c0-144">Следующий запрос перемещает указанное сообщение в папки «Удаленные», определяется именем известных папки `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-144">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3a2c0-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a2c0-145">Response</span></span>

<span data-ttu-id="3a2c0-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-146">Here is an example of the response.</span></span>

> <span data-ttu-id="3a2c0-147">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a2c0-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a2c0-148">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
