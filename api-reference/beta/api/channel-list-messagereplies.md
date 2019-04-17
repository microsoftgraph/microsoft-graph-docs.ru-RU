---
title: Список ответов на сообщения канала
description: ПереЧисление всех ответов на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ef844dc03b26e4f3184b138aa6f8a845453e0c7
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889977"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="4aa1d-103">Список ответов на сообщения канала</span><span class="sxs-lookup"><span data-stu-id="4aa1d-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aa1d-104">ПереЧисление всех ответов на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa1d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4aa1d-105">Permissions</span></span>
<span data-ttu-id="4aa1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aa1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aa1d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4aa1d-108">Permission Type</span></span>|<span data-ttu-id="4aa1d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4aa1d-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4aa1d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4aa1d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4aa1d-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aa1d-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="4aa1d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4aa1d-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aa1d-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4aa1d-113">Not supported</span></span>|
|<span data-ttu-id="4aa1d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4aa1d-114">Application</span></span>| <span data-ttu-id="4aa1d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aa1d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4aa1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4aa1d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4aa1d-117">Optional query parameters</span></span>
<span data-ttu-id="4aa1d-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aa1d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4aa1d-119">Request headers</span></span>
| <span data-ttu-id="4aa1d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4aa1d-120">Header</span></span>       | <span data-ttu-id="4aa1d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4aa1d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4aa1d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4aa1d-122">Authorization</span></span>  | <span data-ttu-id="4aa1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aa1d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4aa1d-125">Request body</span></span>
<span data-ttu-id="4aa1d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aa1d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aa1d-127">Response</span></span>
<span data-ttu-id="4aa1d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatmessage](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aa1d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4aa1d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aa1d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4aa1d-130">Request</span></span>
<span data-ttu-id="4aa1d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="4aa1d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aa1d-132">Response</span></span>
<span data-ttu-id="4aa1d-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4aa1d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4aa1d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
                "id": "id-value ",
                "mentionText": "Test User",
                "mentioned": {
                "user": {
                    "id": "id-value",
                    "displayName: "string"
                }
            }
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
