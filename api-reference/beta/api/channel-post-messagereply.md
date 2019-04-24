---
title: Ответ на сообщение в канале
description: Ответ на существующее сообщение в канале.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 15e1bfffe7d7634092937a0605debfd5294b142b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456467"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="9ce80-103">Ответ на сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="9ce80-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce80-104">Создание нового ответа на [сообщение](../resources/chatmessage.md) в указанном канале [](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9ce80-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce80-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce80-105">Permissions</span></span>
<span data-ttu-id="9ce80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce80-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce80-108">Permission type</span></span>      | <span data-ttu-id="9ce80-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ce80-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce80-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ce80-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ce80-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce80-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ce80-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ce80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ce80-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce80-113">Not supported.</span></span>    |
|<span data-ttu-id="9ce80-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ce80-114">Application</span></span> | <span data-ttu-id="9ce80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce80-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ce80-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ce80-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="9ce80-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ce80-117">Request headers</span></span>
| <span data-ttu-id="9ce80-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9ce80-118">Name</span></span>       | <span data-ttu-id="9ce80-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce80-119">Type</span></span> | <span data-ttu-id="9ce80-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce80-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ce80-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce80-121">Authorization</span></span>  | <span data-ttu-id="9ce80-122">string</span><span class="sxs-lookup"><span data-stu-id="9ce80-122">string</span></span>  | <span data-ttu-id="9ce80-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce80-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ce80-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ce80-125">Request body</span></span>
<span data-ttu-id="9ce80-126">В тексте запроса добавьте представление объекта [Message](../resources/chatmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ce80-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="9ce80-127">Только свойство Body является обязательным, другие свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="9ce80-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="9ce80-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce80-128">Response</span></span>

<span data-ttu-id="9ce80-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика с созданным [сообщением](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="9ce80-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="9ce80-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9ce80-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ce80-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce80-131">Request</span></span>
<span data-ttu-id="9ce80-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce80-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="9ce80-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce80-133">Response</span></span>

<span data-ttu-id="9ce80-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce80-134">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
    "Error: /api-reference/beta/api/channel-post-reply_chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
