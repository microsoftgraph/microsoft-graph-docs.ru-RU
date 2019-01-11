---
title: Список сообщения
description: 'Получаете список сообщений в канале команды (без ответов). Чтобы получить ответы на сообщения, вызовите ответов сообщения списка или ответе на сообщение get API. '
localization_priority: Priority
ms.openlocfilehash: c972b84b0ec4de9389f8a0e861cafb74d7b23020
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867097"
---
# <a name="list-channel-messages"></a><span data-ttu-id="b7e40-104">Список сообщения</span><span class="sxs-lookup"><span data-stu-id="b7e40-104">List channel messages</span></span>

> <span data-ttu-id="b7e40-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7e40-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7e40-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7e40-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7e40-107">Получаете список [сообщений](../resources/chatmessage.md) (без ответов) на [канал](../resources/channel.md) [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b7e40-107">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="b7e40-108">Чтобы получить ответы на сообщения, вызовите [список сообщений ответов](channel-get-messagereply.md) или [получить ответ на сообщение](channel-list-messagereplies.md) API.</span><span class="sxs-lookup"><span data-stu-id="b7e40-108">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b7e40-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e40-109">Permissions</span></span>
<span data-ttu-id="b7e40-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7e40-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e40-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7e40-112">Permission Type</span></span>|<span data-ttu-id="b7e40-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7e40-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b7e40-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7e40-114">Delegated (work or school account)</span></span>|<span data-ttu-id="b7e40-115">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e40-115">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="b7e40-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7e40-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7e40-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b7e40-117">Not supported</span></span>|
|<span data-ttu-id="b7e40-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7e40-118">Application</span></span>| <span data-ttu-id="b7e40-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7e40-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7e40-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7e40-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7e40-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7e40-121">Optional query parameters</span></span>
<span data-ttu-id="b7e40-122">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b7e40-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7e40-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7e40-123">Request headers</span></span>
| <span data-ttu-id="b7e40-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7e40-124">Header</span></span>       | <span data-ttu-id="b7e40-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b7e40-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7e40-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7e40-126">Authorization</span></span>  | <span data-ttu-id="b7e40-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7e40-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7e40-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7e40-129">Request body</span></span>
<span data-ttu-id="b7e40-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7e40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7e40-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7e40-131">Response</span></span>

<span data-ttu-id="b7e40-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [chatmessage](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b7e40-132">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7e40-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b7e40-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7e40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7e40-134">Request</span></span>
<span data-ttu-id="b7e40-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7e40-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="b7e40-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7e40-136">Response</span></span>
<span data-ttu-id="b7e40-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7e40-137">Here is an example of the response.</span></span> 

><span data-ttu-id="b7e40-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7e40-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "content": "Hello World",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
