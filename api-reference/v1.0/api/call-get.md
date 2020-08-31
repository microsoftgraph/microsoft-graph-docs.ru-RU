---
title: Получение вызова
description: Получение свойств и связей объекта Call.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 57b863b7593e54b9594ce748fea58bf24326c6a9
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311916"
---
# <a name="get-call"></a><span data-ttu-id="5f016-103">Получение вызова</span><span class="sxs-lookup"><span data-stu-id="5f016-103">Get call</span></span>

<span data-ttu-id="5f016-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f016-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f016-105">Получение свойств и связей объекта Call.</span><span class="sxs-lookup"><span data-stu-id="5f016-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f016-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f016-106">Permissions</span></span>
<span data-ttu-id="5f016-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f016-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f016-109">Permission type</span></span> | <span data-ttu-id="5f016-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f016-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5f016-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f016-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f016-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f016-112">Not Supported.</span></span>                         |
| <span data-ttu-id="5f016-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f016-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f016-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f016-114">Not Supported.</span></span>                         |
| <span data-ttu-id="5f016-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f016-115">Application</span></span>                            | <span data-ttu-id="5f016-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="5f016-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="5f016-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f016-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f016-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f016-118">Optional query parameters</span></span>
<span data-ttu-id="5f016-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5f016-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f016-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f016-120">Request headers</span></span>
| <span data-ttu-id="5f016-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5f016-121">Name</span></span>          | <span data-ttu-id="5f016-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5f016-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5f016-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f016-123">Authorization</span></span> | <span data-ttu-id="5f016-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f016-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f016-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f016-126">Request body</span></span>
<span data-ttu-id="5f016-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f016-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f016-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f016-128">Response</span></span>
<span data-ttu-id="5f016-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f016-129">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f016-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f016-130">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="5f016-131">Пример 1: как получить одноранговый Звонок</span><span class="sxs-lookup"><span data-stu-id="5f016-131">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="5f016-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f016-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f016-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f016-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="5f016-134">C#</span><span class="sxs-lookup"><span data-stu-id="5f016-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f016-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f016-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f016-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f016-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f016-137">Java</span><span class="sxs-lookup"><span data-stu-id="5f016-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5f016-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f016-138">Response</span></span>

> <span data-ttu-id="5f016-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f016-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="5f016-141">Пример 2: вызов групповой связи</span><span class="sxs-lookup"><span data-stu-id="5f016-141">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="5f016-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f016-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f016-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f016-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="5f016-144">C#</span><span class="sxs-lookup"><span data-stu-id="5f016-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f016-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f016-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f016-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f016-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f016-147">Java</span><span class="sxs-lookup"><span data-stu-id="5f016-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5f016-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f016-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "displayName": null
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": {
    "@odata.type": "#microsoft.graph.callTranscriptionInfo",
    "state": "inactive",
    "lastModifiedDateTime": "2020-05-28T00:10:54.104318Z"
  },
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "toneInfo": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
