---
title: Создание звонка
description: Создайте новый вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2ad6842c4956c10b46421a99c9647f313eec20cd
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472287"
---
# <a name="create-call"></a><span data-ttu-id="fd94b-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="fd94b-103">Create call</span></span>

<span data-ttu-id="fd94b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd94b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd94b-105">Создание [вызова](../resources/call.md) позволяет боту создать новый исходяющий одноранговой или групповой вызов или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="fd94b-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="fd94b-106">Вам потребуется [зарегистрировать вызываемого бота](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) и пройти список разрешений, необходимых, как упоминалось ниже.</span><span class="sxs-lookup"><span data-stu-id="fd94b-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="fd94b-107">**Примечание:** В настоящее время поддерживаются только вызовы VoIP.</span><span class="sxs-lookup"><span data-stu-id="fd94b-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fd94b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd94b-108">Permissions</span></span>

<span data-ttu-id="fd94b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="fd94b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="fd94b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd94b-111">Permission type</span></span>                        | <span data-ttu-id="fd94b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd94b-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="fd94b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd94b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd94b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd94b-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="fd94b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd94b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd94b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd94b-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="fd94b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd94b-117">Application</span></span>                            | <span data-ttu-id="fd94b-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate. Все, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="fd94b-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="fd94b-119">**Примечание:** Для вызова в средствах массовой информации с использованием приложений требуется разрешение Calls.AccessMedia.All в дополнение к одному из перечисленных разрешений.</span><span class="sxs-lookup"><span data-stu-id="fd94b-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd94b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="fd94b-121">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="fd94b-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="fd94b-122">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="fd94b-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd94b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd94b-123">Request headers</span></span>
| <span data-ttu-id="fd94b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="fd94b-124">Name</span></span>          | <span data-ttu-id="fd94b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fd94b-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fd94b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd94b-126">Authorization</span></span> | <span data-ttu-id="fd94b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd94b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd94b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd94b-129">Content-type</span></span>  | <span data-ttu-id="fd94b-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd94b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd94b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd94b-132">Request body</span></span>
<span data-ttu-id="fd94b-133">В теле запроса поставляем JSON-представление объекта [вызова.](../resources/call.md)</span><span class="sxs-lookup"><span data-stu-id="fd94b-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fd94b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-134">Response</span></span>
<span data-ttu-id="fd94b-135">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [вызова](../resources/call.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fd94b-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd94b-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd94b-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="fd94b-137">Пример 1. Создание одноранговых вызовов VoIP с помощью средств массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="fd94b-138">**Примечание:** Этот вызов требует Calls.Initiate. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="fd94b-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-139">Request</span></span>
<span data-ttu-id="fd94b-140">В следующем примере показан запрос, который делает одноранговой вызов между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="fd94b-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="fd94b-141">В этом примере носители хозяйской службы.</span><span class="sxs-lookup"><span data-stu-id="fd94b-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="fd94b-142">Значения маркера авторизации, URL-адреса, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="fd94b-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="fd94b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd94b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
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
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="fd94b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd94b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fd94b-145">C#</span><span class="sxs-lookup"><span data-stu-id="fd94b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd94b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd94b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd94b-147">Java</span><span class="sxs-lookup"><span data-stu-id="fd94b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd94b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-148">Response</span></span>

> <span data-ttu-id="fd94b-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd94b-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "countryCode": null,
    "endpointType": null,
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
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
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
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="fd94b-150">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="fd94b-150">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "id": "2e1a0b00-2db4-4022-9570-243709c565ab"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="fd94b-151">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="fd94b-151">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "direction": "outgoing",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="fd94b-152">Пример 2. Создание одноранговых вызовов VoIP с помощью средств массовой информации приложения</span><span class="sxs-lookup"><span data-stu-id="fd94b-152">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="fd94b-153">**Примечание.** В этом примере Calls.Initiate. Все разрешения и разрешения Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="fd94b-153">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-154">Request</span></span>
<span data-ttu-id="fd94b-155">В следующем примере показан запрос, который делает одноранговой вызов между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="fd94b-155">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="fd94b-156">В этом примере средства массовой информации локализованы приложением.</span><span class="sxs-lookup"><span data-stu-id="fd94b-156">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="fd94b-157">Значения маркера авторизации, URL-адреса вызова, id приложения, имени приложения, пользовательского именем пользователя и id клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="fd94b-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="fd94b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd94b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
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
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="fd94b-159">C#</span><span class="sxs-lookup"><span data-stu-id="fd94b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd94b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd94b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd94b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd94b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd94b-162">Java</span><span class="sxs-lookup"><span data-stu-id="fd94b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fd94b-163">`<Media Session Configuration>` — это конфигурация сеанса сеанса мультимедиа, которая содержит сведения о сеансах стека мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="fd94b-163">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="fd94b-164">Конкретные сведения о аудио, видео, сведения о Ssession VBSS должны быть переданы здесь.</span><span class="sxs-lookup"><span data-stu-id="fd94b-164">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="fd94b-165">Пример blob сеанса сеанса аудио мультимедиа показан ниже</span><span class="sxs-lookup"><span data-stu-id="fd94b-165">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="fd94b-166">**Примечание:** Для одноранговых вызовов ожидаемые уведомления только для изменения состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="fd94b-166">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="fd94b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-167">Response</span></span>

> <span data-ttu-id="fd94b-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd94b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
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
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="fd94b-170">Пример 3. Создание группового вызова с помощью средства массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-170">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="fd94b-171">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="fd94b-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="fd94b-172">В примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="fd94b-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="fd94b-173">**Примечание:** В этом примере вызову требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd94b-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="fd94b-174">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="fd94b-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-175">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="fd94b-176">Пример 4. Создание группового вызова с помощью средства массовой информации с хостингом приложения</span><span class="sxs-lookup"><span data-stu-id="fd94b-176">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="fd94b-177">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="fd94b-177">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="fd94b-178">В примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="fd94b-178">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="fd94b-179">**Примечание:** В этом примере вызову требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd94b-179">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="fd94b-180">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="fd94b-180">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-181">Request</span></span>
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
    "removeFromDefaultAudioGroup": false
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="fd94b-182">Пример 5. Присоединиться к запланированной встрече с средствами массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-182">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="fd94b-183">Чтобы присоединиться к запланированному собранию, нам необходимо получить потоковый id, id сообщения, id организатора и id клиента, в котором планируется собрание.</span><span class="sxs-lookup"><span data-stu-id="fd94b-183">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="fd94b-184">Эти сведения можно получить из [API Get Online Meetings.](../api/onlinemeeting-get.md)</span><span class="sxs-lookup"><span data-stu-id="fd94b-184">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="fd94b-185">Значения маркера авторизации, URL-адреса вызова, id приложения, имени приложения, пользовательского именем пользователя и id клиента должны быть заменены вместе с сведениями, полученными из API Get  [Online Meetings,](../api/onlinemeeting-get.md) фактическими значениями для работы в примере.</span><span class="sxs-lookup"><span data-stu-id="fd94b-185">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="fd94b-186">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd94b-186">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-187">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fd94b-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd94b-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "join-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
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
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob",
        "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
}
```
# <a name="c"></a>[<span data-ttu-id="fd94b-189">C#</span><span class="sxs-lookup"><span data-stu-id="fd94b-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/join-meeting-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd94b-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd94b-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/join-meeting-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd94b-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd94b-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/join-meeting-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd94b-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-192">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": null,
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="fd94b-193">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="fd94b-193">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
        "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}

```
##### <a name="notification---established"></a><span data-ttu-id="fd94b-194">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="fd94b-194">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}
```
##### <a name="notification---roster"></a><span data-ttu-id="fd94b-195">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="fd94b-195">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "John",
                "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
              }
            },
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "sourceId": "2",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "sourceId": "8",
              "direction": "receiveOnly",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false,
          "id": "0d7664b6-6432-43ed-8d27-d9e7adec188c"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```

><span data-ttu-id="fd94b-196">**Примечание:** Для сценариев присоединиться к собраниям, кроме уведомлений состояния вызовов, мы получаем уведомления реестра.</span><span class="sxs-lookup"><span data-stu-id="fd94b-196">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="fd94b-197">Пример 6. Присоединяйтесь к запланированной встрече с средствами массовой информации, на которые было организовано приложение</span><span class="sxs-lookup"><span data-stu-id="fd94b-197">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="fd94b-198">Чтобы присоединиться к собранию с ведущими средствами массовой информации приложения, обновить медиафайл с [appHostedMediaConfig,](../resources/apphostedmediaconfig.md) как показано ниже, в приведенном выше примере.</span><span class="sxs-lookup"><span data-stu-id="fd94b-198">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a"
}
```


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="fd94b-199">Пример 7. Регистрация собрания каналов со средствами массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-199">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="fd94b-200">Собрание внутри канала требует определенных сведений, таких как потоковые id, messageid и сведения организатора, которые можно получить с помощью [API Get Online Meetings](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="fd94b-200">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="fd94b-201">Значения маркера авторизации, URL-адреса вызова, id приложения, имени приложения, пользовательского именем пользователя и id клиента должны быть заменены вместе с сведениями, полученными из API Get  [Online Meetings,](../api/onlinemeeting-get.md) фактическими значениями для работы в примере.</span><span class="sxs-lookup"><span data-stu-id="fd94b-201">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="fd94b-202">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd94b-202">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-203">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
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
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="fd94b-204">Пример 8. Регистрация собрания канала в качестве гостя со средствами массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-204">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="fd94b-205">Для присоединения к собранию канала в качестве [](../resources/identityset.md) гостя необходимо создать удостоверение гостя и добавить его в качестве источника вызова в запросе на присоединение к собранию.</span><span class="sxs-lookup"><span data-stu-id="fd94b-205">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="fd94b-206">Имя отображения — это имя, которое необходимо отобразить на собрании для удостоверения гостя.</span><span class="sxs-lookup"><span data-stu-id="fd94b-206">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="fd94b-207">Идентификатор может быть уникальным идентификатором, идентифицирующий личность гостя.</span><span class="sxs-lookup"><span data-stu-id="fd94b-207">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="fd94b-208">**Примечание:** В этом примере требуется `Calls.JoinGroupCallsAsGuest.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd94b-208">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="fd94b-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-209">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-channel-meeting-as-guest-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "guest": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Guest User",
        "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
      }
    }
  },
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
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
> <span data-ttu-id="fd94b-210">**Примечание:** Регистрация гостей зависит от параметров клиента для собрания.</span><span class="sxs-lookup"><span data-stu-id="fd94b-210">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="fd94b-211">Приложение может быть положено в вестибюль, ожидая, чтобы его допустил пользователь.</span><span class="sxs-lookup"><span data-stu-id="fd94b-211">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="fd94b-212">Это определяется `isInLobby` свойством</span><span class="sxs-lookup"><span data-stu-id="fd94b-212">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="fd94b-213">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="fd94b-213">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "guest": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Guest User",
                "id": "d7a3b999-17ac-4bca-9e77-e6a730d2ec2e"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": true,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```
> <span data-ttu-id="fd94b-214">**Примечание:** Приложение не будет получать реестр участников собрания, пока его не впустят из лобби</span><span class="sxs-lookup"><span data-stu-id="fd94b-214">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

### <a name="example-9-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="fd94b-215">Пример 9. Создание одноранговых вызовов PSTN с помощью средства массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="fd94b-215">Example 9: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="fd94b-216">**Примечание:** Этот вызов требует Calls.Initiate. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="fd94b-216">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="fd94b-217">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="fd94b-217">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="fd94b-218">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="fd94b-218">Step 1: Create application instance</span></span>
<span data-ttu-id="fd94b-219">Используя учетные данные администратора клиента, для создания экземпляра приложения вызывайте следующие cmdlets на удаленной PowerShell клиента.</span><span class="sxs-lookup"><span data-stu-id="fd94b-219">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="fd94b-220">Дополнительные сведения см. [в new-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="fd94b-220">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="fd94b-221">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fd94b-221">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="fd94b-222">Используйте учетные данные администратора клиента, чтобы войти на вкладку https://admin.microsoft.com/ **Пользователи -> активных пользователей.**</span><span class="sxs-lookup"><span data-stu-id="fd94b-222">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="fd94b-223">Выберите экземпляр приложения, назначьте План внутренних и международных вызовов **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите **кнопку Сохранить изменения.**</span><span class="sxs-lookup"><span data-stu-id="fd94b-223">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="fd94b-224">Если в клиенте не доступны необходимые лицензии, их можно получить на вкладке Службы > **покупки.**</span><span class="sxs-lookup"><span data-stu-id="fd94b-224">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="fd94b-225">Шаг 3. Приобретение номера PSTN</span><span class="sxs-lookup"><span data-stu-id="fd94b-225">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="fd94b-226">Используйте учетные данные администратора клиента, чтобы войти и щелкнуть вкладку https://admin.teams.microsoft.com/ **Портал Legacy** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="fd94b-226">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="fd94b-227">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="fd94b-227">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="fd94b-228">Нажмите **+** кнопку, **выберите новые номера служб** и перейдите на страницу Добавить новые **номера** службы.</span><span class="sxs-lookup"><span data-stu-id="fd94b-228">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="fd94b-229">Выберите **Country/Region,** **State/Region,** **City,** input **Quantity** и **щелкните добавить в** поиск.</span><span class="sxs-lookup"><span data-stu-id="fd94b-229">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="fd94b-230">Нажмите **кнопку получение номеров**.</span><span class="sxs-lookup"><span data-stu-id="fd94b-230">Click **acquire numbers**.</span></span> <span data-ttu-id="fd94b-231">Недавно приобретенный номер будет показываться на **вкладке номера** телефонов.</span><span class="sxs-lookup"><span data-stu-id="fd94b-231">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="fd94b-232">Шаг 4. Назначение номера PSTN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="fd94b-232">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="fd94b-233">С учетными данными администратора клиента вызываем следующие cmdlets на удаленной PowerShell клиента, чтобы назначить номер PSTN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="fd94b-233">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="fd94b-234">Дополнительные сведения см. [в рублях Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="fd94b-234">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="fd94b-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-235">Request</span></span>
<span data-ttu-id="fd94b-236">В следующем примере показан запрос на одноранговой вызов между ботом и номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="fd94b-236">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="fd94b-237">В этом примере носители хозяйской службы.</span><span class="sxs-lookup"><span data-stu-id="fd94b-237">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="fd94b-238">Значения маркера авторизации, URL-адреса, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="fd94b-238">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```

#### <a name="response"></a><span data-ttu-id="fd94b-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-239">Response</span></span>

> <span data-ttu-id="fd94b-240">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd94b-240">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
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
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-10-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="fd94b-241">Пример 10. Создание одноранговых вызовов PSTN с помощью носите-</span><span class="sxs-lookup"><span data-stu-id="fd94b-241">Example 10: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="fd94b-242">**Примечание.** В этом примере Calls.Initiate. Все разрешения и разрешения Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="fd94b-242">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="fd94b-243">Этот вызов требует экземпляра приложения с присвоенным номером PSTN, как описано в примере 9.</span><span class="sxs-lookup"><span data-stu-id="fd94b-243">This call needs application instance with PSTN number assigned, as described in Example 9.</span></span>

#### <a name="request"></a><span data-ttu-id="fd94b-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd94b-244">Request</span></span>
<span data-ttu-id="fd94b-245">В следующем примере показан запрос на одноранговой вызов между ботом и номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="fd94b-245">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="fd94b-246">В этом примере средства массовой информации локализованы приложением.</span><span class="sxs-lookup"><span data-stu-id="fd94b-246">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="fd94b-247">Замените значения маркера авторизации, URL-адреса вызова, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="fd94b-247">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```

#### <a name="response"></a><span data-ttu-id="fd94b-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd94b-248">Response</span></span>

> <span data-ttu-id="fd94b-249">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fd94b-249">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
