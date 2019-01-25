---
title: 'message: move'
description: Переместите сообщение в папку. Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: efe2bcf262ef91b4684bc812fa19bdbe52f12564
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526860"
---
# <a name="message-move"></a><span data-ttu-id="16f42-104">message: move</span><span class="sxs-lookup"><span data-stu-id="16f42-104">message: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16f42-105">Переместите сообщение в папку.</span><span class="sxs-lookup"><span data-stu-id="16f42-105">Move a message to a folder.</span></span> <span data-ttu-id="16f42-106">Это создает новую копию сообщения в папке назначения и удаляет исходное сообщение.</span><span class="sxs-lookup"><span data-stu-id="16f42-106">This creates a new copy of the message in the destination folder and removes the original message.</span></span>

## <a name="permissions"></a><span data-ttu-id="16f42-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16f42-107">Permissions</span></span>

<span data-ttu-id="16f42-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16f42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16f42-110">Permission type</span></span> | <span data-ttu-id="16f42-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16f42-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="16f42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16f42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16f42-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f42-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16f42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16f42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16f42-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f42-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="16f42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16f42-116">Application</span></span> | <span data-ttu-id="16f42-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16f42-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="16f42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16f42-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="16f42-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16f42-119">Request headers</span></span>

| <span data-ttu-id="16f42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16f42-120">Header</span></span> | <span data-ttu-id="16f42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16f42-121">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="16f42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16f42-122">Authorization</span></span> | <span data-ttu-id="16f42-123">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="16f42-123"></span></span> <span data-ttu-id="16f42-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16f42-124">Required.</span></span> |
| <span data-ttu-id="16f42-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16f42-125">Content-Type</span></span> | <span data-ttu-id="16f42-126">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="16f42-126"></span></span> <span data-ttu-id="16f42-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16f42-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16f42-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16f42-128">Request body</span></span>

<span data-ttu-id="16f42-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="16f42-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16f42-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="16f42-130">Parameter</span></span>   | <span data-ttu-id="16f42-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16f42-131">Type</span></span> |<span data-ttu-id="16f42-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16f42-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16f42-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="16f42-133">DestinationId</span></span>|<span data-ttu-id="16f42-134">String</span><span class="sxs-lookup"><span data-stu-id="16f42-134">String</span></span>|<span data-ttu-id="16f42-135">Идентификатор папки назначения, или имя известных папки.</span><span class="sxs-lookup"><span data-stu-id="16f42-135">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="16f42-136">Список поддерживаемых известных имен см. в статье [Тип ресурса mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="16f42-136">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="16f42-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="16f42-137">Response</span></span>

<span data-ttu-id="16f42-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и ресурсов [сообщения](../resources/message.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16f42-138">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f42-139">Пример</span><span class="sxs-lookup"><span data-stu-id="16f42-139">Example</span></span>

<span data-ttu-id="16f42-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="16f42-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="16f42-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="16f42-141">Request</span></span>

<span data-ttu-id="16f42-142">Следующий запрос перемещает указанное сообщение в папки «Удаленные», определяется именем известных папки `deleteditems`.</span><span class="sxs-lookup"><span data-stu-id="16f42-142">The following request moves the specified message to the Deleted Items folder, identified by its well-known folder name `deleteditems`.</span></span>
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

##### <a name="response"></a><span data-ttu-id="16f42-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="16f42-143">Response</span></span>

<span data-ttu-id="16f42-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16f42-144">Here is an example of the response.</span></span>

> <span data-ttu-id="16f42-145">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16f42-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16f42-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16f42-146">All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/message-move.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
