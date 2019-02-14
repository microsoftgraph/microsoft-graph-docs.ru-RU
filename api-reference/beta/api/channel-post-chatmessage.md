---
title: Создайте сообщение в канале
description: Создайте новое сообщение в указанный канал.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 891181c8797563fac6afb7862a27bd8b49628b5f
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "30039568"
---
# <a name="create-a-message-in-a-channel"></a><span data-ttu-id="4a41f-103">Создайте сообщение в канале</span><span class="sxs-lookup"><span data-stu-id="4a41f-103">Create a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a41f-104">Создайте новое [сообщение](../resources/chatmessage.md) в указанном [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4a41f-104">Create a new [message](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a41f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a41f-105">Permissions</span></span>
<span data-ttu-id="4a41f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a41f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a41f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a41f-108">Permission type</span></span>      | <span data-ttu-id="4a41f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a41f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a41f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a41f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a41f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a41f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a41f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a41f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a41f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a41f-113">Not supported.</span></span>    |
|<span data-ttu-id="4a41f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a41f-114">Application</span></span> | <span data-ttu-id="4a41f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a41f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a41f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a41f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="4a41f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a41f-117">Request headers</span></span>
| <span data-ttu-id="4a41f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a41f-118">Name</span></span>       | <span data-ttu-id="4a41f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4a41f-119">Type</span></span> | <span data-ttu-id="4a41f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a41f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a41f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a41f-121">Authorization</span></span>  | <span data-ttu-id="4a41f-122">string</span><span class="sxs-lookup"><span data-stu-id="4a41f-122">string</span></span>  | <span data-ttu-id="4a41f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a41f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a41f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a41f-125">Request body</span></span>
<span data-ttu-id="4a41f-126">В тексте запроса укажите представление JSON объекта [сообщения](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="4a41f-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="4a41f-127">Свойство body является обязательным, остальные свойства являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="4a41f-127">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="4a41f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a41f-128">Response</span></span>

<span data-ttu-id="4a41f-129">Успешно завершена, этот метод возвращает `201 Created` код ответа с помощью [сообщения](../resources/chatmessage.md) , которая была создана.</span><span class="sxs-lookup"><span data-stu-id="4a41f-129">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="4a41f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4a41f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a41f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a41f-131">Request</span></span>
<span data-ttu-id="4a41f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a41f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

##### <a name="response"></a><span data-ttu-id="4a41f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a41f-133">Response</span></span>

<span data-ttu-id="4a41f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a41f-134">Here is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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
  "description": "Create message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
