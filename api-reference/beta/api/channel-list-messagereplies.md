---
title: Список ответов на сообщения канала
description: ПереЧисление всех ответов на сообщение в канале команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 377d574a037010e4a441406506af4764784145e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328143"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="bfa46-103">Список ответов на сообщения канала</span><span class="sxs-lookup"><span data-stu-id="bfa46-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa46-104">ПереЧисление всех ответов на [сообщение](../resources/chatmessage.md) в [канале](../resources/channel.md) команды.</span><span class="sxs-lookup"><span data-stu-id="bfa46-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="bfa46-105">Этот метод перечисляет только ответы на заданное сообщение, если таковые имеются.</span><span class="sxs-lookup"><span data-stu-id="bfa46-105">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="bfa46-106">Чтобы получить само сообщение, просто вызовите [сообщение Get Channel](channel-get-message.md).</span><span class="sxs-lookup"><span data-stu-id="bfa46-106">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bfa46-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfa46-107">Permissions</span></span>
<span data-ttu-id="bfa46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfa46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfa46-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfa46-110">Permission Type</span></span>|<span data-ttu-id="bfa46-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfa46-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="bfa46-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfa46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bfa46-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa46-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="bfa46-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfa46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfa46-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bfa46-115">Not supported</span></span>|
|<span data-ttu-id="bfa46-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfa46-116">Application</span></span>| <span data-ttu-id="bfa46-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfa46-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfa46-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfa46-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfa46-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfa46-119">Optional query parameters</span></span>

<span data-ttu-id="bfa46-120">Вы можете использовать параметр запроса [$top](/graph/query-parameters#top-parameter) для управления количеством элементов в одном отклике.</span><span class="sxs-lookup"><span data-stu-id="bfa46-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="bfa46-121">Другие [параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bfa46-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfa46-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfa46-122">Request headers</span></span>
| <span data-ttu-id="bfa46-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfa46-123">Header</span></span>       | <span data-ttu-id="bfa46-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bfa46-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfa46-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfa46-125">Authorization</span></span>  | <span data-ttu-id="bfa46-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfa46-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfa46-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfa46-128">Request body</span></span>
<span data-ttu-id="bfa46-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfa46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfa46-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfa46-130">Response</span></span>
<span data-ttu-id="bfa46-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [chatmessage](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfa46-131">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfa46-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bfa46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfa46-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfa46-133">Request</span></span>
<span data-ttu-id="bfa46-134">В этом примере указанное сообщение имеет два ответа.</span><span class="sxs-lookup"><span data-stu-id="bfa46-134">In this example, the specified message has two replies.</span></span> <span data-ttu-id="bfa46-135">Каждый ответ содержит один или несколько объектов [чатмессажементион](../resources/chatmessagemention.md) .</span><span class="sxs-lookup"><span data-stu-id="bfa46-135">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
##### <a name="response"></a><span data-ttu-id="bfa46-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfa46-136">Response</span></span>
<span data-ttu-id="bfa46-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bfa46-137">Here is an example of the response.</span></span> 

><span data-ttu-id="bfa46-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfa46-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies",
    "@odata.count": 2,
    "value": [
        {
            "id": "1555377090002",
            "replyToId": "1555375673184",
            "etag": "1555377090002",
            "messageType": "message",
            "createdDateTime": "2019-04-16T01:11:30.002Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
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
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Megan",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                            "displayName": "Megan",
                            "userIdentityType": "aadUser"
                        }
                    }
                },
                {
                    "id": 1,
                    "mentionText": "Alex",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1555375848360",
            "replyToId": "1555375673184",
            "etag": "1555375848360",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:50:48.36Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
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
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div>And, <at id=\"0\">Alex Wilber</at>, can we see the February report as well?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Alex Wilber",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex Wilber",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
