---
title: Получение вызова
description: Извлечение свойств и связей объекта вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 035dfff2d7189f67f05de241997391fb86437dce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948572"
---
# <a name="get-call"></a><span data-ttu-id="e305c-103">Получение вызова</span><span class="sxs-lookup"><span data-stu-id="e305c-103">Get call</span></span>

<span data-ttu-id="e305c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e305c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e305c-105">Извлечение свойств и связей объекта вызова.</span><span class="sxs-lookup"><span data-stu-id="e305c-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e305c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e305c-106">Permissions</span></span>
<span data-ttu-id="e305c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e305c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e305c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e305c-109">Permission type</span></span> | <span data-ttu-id="e305c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e305c-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e305c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e305c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e305c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e305c-112">Not Supported.</span></span>                         |
| <span data-ttu-id="e305c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e305c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e305c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e305c-114">Not Supported.</span></span>                         |
| <span data-ttu-id="e305c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e305c-115">Application</span></span>                            | <span data-ttu-id="e305c-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e305c-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e305c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e305c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="e305c-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e305c-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e305c-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e305c-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e305c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e305c-120">Optional query parameters</span></span>
<span data-ttu-id="e305c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e305c-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e305c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e305c-122">Request headers</span></span>
| <span data-ttu-id="e305c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e305c-123">Name</span></span>          | <span data-ttu-id="e305c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e305c-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e305c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e305c-125">Authorization</span></span> | <span data-ttu-id="e305c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e305c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e305c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e305c-128">Request body</span></span>
<span data-ttu-id="e305c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e305c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e305c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e305c-130">Response</span></span>
<span data-ttu-id="e305c-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [вызова](../resources/call.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e305c-131">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e305c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e305c-132">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="e305c-133">Пример 1. Получение одноранговых вызовов</span><span class="sxs-lookup"><span data-stu-id="e305c-133">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="e305c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e305c-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e305c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e305c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="e305c-136">C#</span><span class="sxs-lookup"><span data-stu-id="e305c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e305c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e305c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e305c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e305c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e305c-139">Java</span><span class="sxs-lookup"><span data-stu-id="e305c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e305c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e305c-140">Response</span></span>

> <span data-ttu-id="e305c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e305c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "callRoutes": [],
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
      },
      "region": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
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
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="e305c-143">Пример 2. Получение группового вызова</span><span class="sxs-lookup"><span data-stu-id="e305c-143">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="e305c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e305c-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e305c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e305c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="e305c-146">C#</span><span class="sxs-lookup"><span data-stu-id="e305c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e305c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e305c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e305c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e305c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e305c-149">Java</span><span class="sxs-lookup"><span data-stu-id="e305c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e305c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e305c-150">Response</span></span>

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
  "callRoutes": [],
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
  "activeModalities": [],
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
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
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
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
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


