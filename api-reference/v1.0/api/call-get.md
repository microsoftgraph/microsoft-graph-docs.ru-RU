---
title: Получение вызова
description: Получение свойств и связей объекта Call.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 219f80aa9bafcd5b5da30c3d03ef6c9c258fc598
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871438"
---
# <a name="get-call"></a><span data-ttu-id="04520-103">Получение вызова</span><span class="sxs-lookup"><span data-stu-id="04520-103">Get call</span></span>

<span data-ttu-id="04520-104">Получение свойств и связей объекта Call.</span><span class="sxs-lookup"><span data-stu-id="04520-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04520-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04520-105">Permissions</span></span>
<span data-ttu-id="04520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04520-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04520-108">Permission type</span></span> | <span data-ttu-id="04520-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04520-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="04520-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04520-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="04520-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04520-111">Not Supported.</span></span>                         |
| <span data-ttu-id="04520-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04520-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04520-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04520-113">Not Supported.</span></span>                         |
| <span data-ttu-id="04520-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="04520-114">Application</span></span>                            | <span data-ttu-id="04520-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="04520-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="04520-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04520-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04520-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04520-117">Optional query parameters</span></span>
<span data-ttu-id="04520-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="04520-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04520-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04520-119">Request headers</span></span>
| <span data-ttu-id="04520-120">Имя</span><span class="sxs-lookup"><span data-stu-id="04520-120">Name</span></span>          | <span data-ttu-id="04520-121">Описание</span><span class="sxs-lookup"><span data-stu-id="04520-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="04520-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04520-122">Authorization</span></span> | <span data-ttu-id="04520-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04520-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04520-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04520-125">Request body</span></span>
<span data-ttu-id="04520-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04520-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04520-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="04520-127">Response</span></span>
<span data-ttu-id="04520-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04520-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04520-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="04520-129">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="04520-130">Пример 1: как получить одноранговый Звонок</span><span class="sxs-lookup"><span data-stu-id="04520-130">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="04520-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04520-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04520-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="04520-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04520-133">C#</span><span class="sxs-lookup"><span data-stu-id="04520-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04520-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04520-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04520-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04520-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="04520-136">Java</span><span class="sxs-lookup"><span data-stu-id="04520-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04520-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="04520-137">Response</span></span>

> <span data-ttu-id="04520-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04520-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="04520-140">Пример 2: вызов групповой связи</span><span class="sxs-lookup"><span data-stu-id="04520-140">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="04520-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="04520-141">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04520-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="04520-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04520-143">C#</span><span class="sxs-lookup"><span data-stu-id="04520-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04520-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04520-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04520-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04520-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="04520-146">Java</span><span class="sxs-lookup"><span data-stu-id="04520-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04520-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="04520-147">Response</span></span>

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
