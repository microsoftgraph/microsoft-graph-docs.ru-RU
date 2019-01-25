---
title: Ответы на сообщение канала списка
description: Список всех ответов на сообщение в канал группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ac3b068e93e370ce981d478c87e573f248695c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512299"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="9080c-103">Ответы на сообщение канала списка</span><span class="sxs-lookup"><span data-stu-id="9080c-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9080c-104">Список всех ответов на [сообщения](../resources/chatmessage.md) в [канал](../resources/channel.md) группы.</span><span class="sxs-lookup"><span data-stu-id="9080c-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="9080c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9080c-105">Permissions</span></span>
<span data-ttu-id="9080c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9080c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9080c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9080c-108">Permission Type</span></span>|<span data-ttu-id="9080c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9080c-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9080c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9080c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9080c-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9080c-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="9080c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9080c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9080c-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9080c-113">Not supported</span></span>|
|<span data-ttu-id="9080c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9080c-114">Application</span></span>| <span data-ttu-id="9080c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9080c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9080c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9080c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9080c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9080c-117">Optional query parameters</span></span>
<span data-ttu-id="9080c-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="9080c-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9080c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9080c-119">Request headers</span></span>
| <span data-ttu-id="9080c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9080c-120">Header</span></span>       | <span data-ttu-id="9080c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9080c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9080c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9080c-122">Authorization</span></span>  | <span data-ttu-id="9080c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9080c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9080c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9080c-125">Request body</span></span>
<span data-ttu-id="9080c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9080c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9080c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9080c-127">Response</span></span>
<span data-ttu-id="9080c-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [chatmessage](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9080c-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9080c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9080c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9080c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9080c-130">Request</span></span>
<span data-ttu-id="9080c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9080c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="9080c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9080c-132">Response</span></span>
<span data-ttu-id="9080c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9080c-133">Here is an example of the response.</span></span> 

><span data-ttu-id="9080c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9080c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "replyToId": "id-value",
        "from" : {
            "user": { 
            "id":  "id-value",
            "displayName": "John Doe"
            }  
        },
        "etag": "id-value",
        "messageType": "message",
        "createdDateTime": "2018-07-09T07:40:20.152Z",
        "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
        "body": {
            "content": "This is a response to a message.",
            "contentType": "Text"
        },
        "attachments": [
          {
              "id": "5e32f195-168a-474f-a273-123123123",
              "contentType": "reference",
              "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
              "content": null,
              "name": "Test.txt",
              "thumbnailUrl": null
          }
        ],
        "mentions": [
            {
                "type": "user",
                "id": "id-value ",
                "mentionText": "Test User"
            }
        ],
        "importance": "normal",
        "reactions": [
            {
                "reactionType": "like",
                "user": {
                    "id": "id-value",
                    "displayName": "John Doe"
                },
                "createdDateTime": "2018-07-09T07:40:20.152Z"
            }
        ],
        "locale": "en-us"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
