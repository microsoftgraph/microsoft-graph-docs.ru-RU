---
title: Получение сообщения в канале
description: Получение одного сообщения (без ответов) в канале команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 26b59ac395af3de314469fdb419095bcb6133d6b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523206"
---
# <a name="get-channel-message"></a><span data-ttu-id="5c85e-103">Получение сообщения в канале</span><span class="sxs-lookup"><span data-stu-id="5c85e-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c85e-104">Получение одного [сообщения](../resources/chatmessage.md) (без ответов) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="5c85e-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c85e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c85e-105">Permissions</span></span>
<span data-ttu-id="5c85e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c85e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c85e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c85e-108">Permission type</span></span>|<span data-ttu-id="5c85e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c85e-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5c85e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c85e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5c85e-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c85e-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="5c85e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c85e-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c85e-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5c85e-113">Not supported</span></span>|
|<span data-ttu-id="5c85e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c85e-114">Application</span></span>| <span data-ttu-id="5c85e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c85e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c85e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c85e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c85e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c85e-117">Optional query parameters</span></span>
<span data-ttu-id="5c85e-118">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5c85e-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c85e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c85e-119">Request headers</span></span>
| <span data-ttu-id="5c85e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c85e-120">Header</span></span>       | <span data-ttu-id="5c85e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c85e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c85e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c85e-122">Authorization</span></span>  | <span data-ttu-id="5c85e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c85e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c85e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c85e-125">Request body</span></span>
<span data-ttu-id="5c85e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c85e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c85e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c85e-127">Response</span></span>

<span data-ttu-id="5c85e-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatmessage](../resources/chatmessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c85e-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c85e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5c85e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c85e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c85e-130">Request</span></span>
<span data-ttu-id="5c85e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c85e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="5c85e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c85e-132">Response</span></span>
<span data-ttu-id="5c85e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c85e-133">Here is an example of the response.</span></span> 

><span data-ttu-id="5c85e-134">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c85e-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="5c85e-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c85e-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
