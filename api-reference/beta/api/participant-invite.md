---
title: 'участник: пригласить'
description: Приглашение участников в активный вызов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1c3f0e7ea4a5fab6b29b0c1db1f7b8b72db3ca3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453938"
---
# <a name="participant-invite"></a><span data-ttu-id="3d6c3-103">участник: пригласить</span><span class="sxs-lookup"><span data-stu-id="3d6c3-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d6c3-104">Приглашение участников в активный вызов.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-104">Invite participants to the active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d6c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d6c3-105">Permissions</span></span>
<span data-ttu-id="3d6c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d6c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d6c3-108">Permission type</span></span> | <span data-ttu-id="3d6c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d6c3-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="3d6c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d6c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d6c3-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3d6c3-111">Not Supported</span></span>                       |
| <span data-ttu-id="3d6c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d6c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d6c3-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3d6c3-113">Not Supported</span></span>                       |
| <span data-ttu-id="3d6c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d6c3-114">Application</span></span>     | <span data-ttu-id="3d6c3-115">Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="3d6c3-115">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="3d6c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d6c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /applications/{id}/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="3d6c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d6c3-117">Request headers</span></span>
| <span data-ttu-id="3d6c3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3d6c3-118">Name</span></span>          | <span data-ttu-id="3d6c3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3d6c3-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3d6c3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d6c3-120">Authorization</span></span> | <span data-ttu-id="3d6c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d6c3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d6c3-123">Request body</span></span>
<span data-ttu-id="3d6c3-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3d6c3-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="3d6c3-125">Parameter</span></span>      | <span data-ttu-id="3d6c3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3d6c3-126">Type</span></span>    |<span data-ttu-id="3d6c3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3d6c3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d6c3-128">participants</span><span class="sxs-lookup"><span data-stu-id="3d6c3-128">participants</span></span>|<span data-ttu-id="3d6c3-129">Коллекция [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="3d6c3-129">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="3d6c3-130">Участники, которые необходимо пригласить.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-130">The participants to invite.</span></span>|
|<span data-ttu-id="3d6c3-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="3d6c3-131">clientContext</span></span>|<span data-ttu-id="3d6c3-132">String</span><span class="sxs-lookup"><span data-stu-id="3d6c3-132">String</span></span>|<span data-ttu-id="3d6c3-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="3d6c3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-134">Response</span></span>
<span data-ttu-id="3d6c3-135">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="examples"></a><span data-ttu-id="3d6c3-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d6c3-136">Examples</span></span>
<span data-ttu-id="3d6c3-137">В приведенных ниже примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-137">The following examples shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3d6c3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d6c3-138">Request</span></span>
<span data-ttu-id="3d6c3-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-139">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3d6c3-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d6c3-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value",
      "replacesCallId": "replacesCallId-value"
    }
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d6c3-141">C#</span><span class="sxs-lookup"><span data-stu-id="3d6c3-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d6c3-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d6c3-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d6c3-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3d6c3-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3d6c3-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-144">Response</span></span>

> <span data-ttu-id="3d6c3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

```
<br/>

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="3d6c3-147">Приглашение участников в существующем собрании P2P</span><span class="sxs-lookup"><span data-stu-id="3d6c3-147">Invite Participants in Existing P2P meeting</span></span>

##### <a name="request"></a><span data-ttu-id="3d6c3-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d6c3-148">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "endpointType": "default",
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "en-US",
      "region": "westus"
    }
  ],
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="response"></a><span data-ttu-id="3d6c3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-149">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "running",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="3d6c3-150">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="3d6c3-150">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="3d6c3-151">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="3d6c3-151">Notification - roster updated with participant added</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
          "info": {
            "identity": {
              "user": {
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
          "info": {
            "identity": {
              "application": {
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="invite-participants-in-existing-p2p-meeting"></a><span data-ttu-id="3d6c3-152">Приглашение участников в существующем собрании P2P</span><span class="sxs-lookup"><span data-stu-id="3d6c3-152">Invite Participants in Existing P2P meeting</span></span>

<span data-ttu-id="3d6c3-153">В этом примере показан полный E2Eный процесс для [приглашения участников](../api/participant-invite.md) в существующем собрании P2P.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-153">This example shows a complete E2E flow for [Invite Participants](../api/participant-invite.md) in an existing P2P meeting.</span></span>

##### <a name="answer-incoming-voip-call-with-service-hosted-media"></a><span data-ttu-id="3d6c3-154">Ответ на входящий вызов VOIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="3d6c3-154">Answer Incoming VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="3d6c3-155">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="3d6c3-155">Notification - Incoming</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "language": "en-US",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          }
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "language": "en-US",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="3d6c3-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d6c3-156">Request</span></span>

``` http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "callback": "https://bot.contoso.com/api/calls",
  "acceptModalities": [ "audio", "video" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "url": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "url": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="3d6c3-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-157">Response</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="3d6c3-158">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="3d6c3-158">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="3d6c3-159">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="3d6c3-159">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": [ "audio", "video" ],
        "requestedModalities": []
      }
    }
  ]
}
```

### <a name="join-channel-meeting-without-media"></a><span data-ttu-id="3d6c3-160">Присоединение к собранию канала без мультимедиа</span><span class="sxs-lookup"><span data-stu-id="3d6c3-160">Join channel meeting without media</span></span>

> <span data-ttu-id="3d6c3-161">**Важно!** если экземпляр Bot присоединяется только в целях облегчения передачи, следует избегать согласования мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-161">**IMPORTANT**: If the bot instance is joining only for the purpose of facilitating the transfer, it should avoid media negotiations.</span></span>  <span data-ttu-id="3d6c3-162">Поэтому лучше всего добавлять его без `requestedModalities` или. `mediaConfig`</span><span class="sxs-lookup"><span data-stu-id="3d6c3-162">Therefore, it is best to add it without any `requestedModalities` or `mediaConfig`.</span></span>

##### <a name="request"></a><span data-ttu-id="3d6c3-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d6c3-163">Request</span></span>

``` http
POST /app/calls
Content-Type: application/json

{
  "subject": "Test Call",
  "callback": "https://bot.contoso.com/api/calls",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targetDisposition": "default",
  "requestedModalities": [],
  "chatInfo": {
    "threadId": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
    "messageId": "1507228578052",
    "replyChainMessageId": "1507228578052"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="3d6c3-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-164">Response</span></span>

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F
```

##### <a name="notification---establishing"></a><span data-ttu-id="3d6c3-165">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="3d6c3-165">Notification - Establishing</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="3d6c3-166">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="3d6c3-166">Notification - Established</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F",
        "@odata.etag": "W/\"5445\"",
        "state": "established",
        "activeModalities": []
      }
    }
  ]
}
```

### <a name="invite-participant-from-initial-incoming-call"></a><span data-ttu-id="3d6c3-167">Приглашение участника от начального входящего звонка</span><span class="sxs-lookup"><span data-stu-id="3d6c3-167">Invite participant from initial incoming call</span></span>

``` http
POST /app/calls/90ED37DCD8E34E119DE330A955DDA06F/participants/invite
Authorization: Bearer <TOKEN>
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "user": {
          "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
        }
      },
      "replacesCallId": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896"
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="3d6c3-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d6c3-168">Response</span></span>

``` http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5
Content-Type: application/json
Content-Length: 306

{
  "clientContext": "clientContext-value",
  "createdDateTime": "2018-03-19T09:46:02Z",
  "id": "id-value",
  "lastActionDateTime": "2018-03-19T09:46:02Z",
  "status": "Running"
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="3d6c3-169">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="3d6c3-169">Notification - Operation Completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "@odata.id": "/app/calls/90ED37DCD8E34E119DE330A955DDA06F/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"51\"",
        "clientContext": "A904FBD5A31041E881E861877A3DE3CD",
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="3d6c3-170">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="3d6c3-170">Notification - Roster Updated With Participant Added</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/8A34A46B3D174ADC8DCEDC4E7D572698",
          "@odata.etag": "W/\"51\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "user": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test User",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ]
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants/123456W77E24E4D85F80597083CB830",
          "@odata.etag": "W/\"55\"",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "application": {
                "region": "westus",
                "languageId": "en-US",
                "displayName": "Test Bot",
                "id": "1234A46B-3D17-4ADC-8DCE-DC4E7D556789"
              }
            }
          },
          "mediaStreams": [
            {
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "2",
              "direction": "sendReceive"
            }
          ]
        }
      ]
    }
  ]
}
```

##### <a name="notification---terminated-the-original-p2p-call"></a><span data-ttu-id="3d6c3-171">Уведомление — завершен первоначальный Звонок P2P</span><span class="sxs-lookup"><span data-stu-id="3d6c3-171">Notification - terminated the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

##### <a name="notification---deleted-the-original-p2p-call"></a><span data-ttu-id="3d6c3-172">Уведомление: Исходный вызов P2P удален</span><span class="sxs-lookup"><span data-stu-id="3d6c3-172">Notification - Deleted the original P2P call</span></span>

``` http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
``` json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\""
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
