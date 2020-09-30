---
title: Создание звонка
description: Создание нового звонка.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0f058c170a080dd0d3ed9028c6b66e31302f1fc3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312556"
---
# <a name="create-call"></a><span data-ttu-id="15646-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="15646-103">Create call</span></span>

<span data-ttu-id="15646-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15646-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15646-105">Создать [вызов](../resources/call.md) позволяет Bot создать новый исходящий одноранговый или групповой вызов или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="15646-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="15646-106">Вам потребуется [зарегистрировать запрашивающий абонент](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) и просмотреть список необходимых разрешений, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="15646-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="15646-107">**Примечание:** В настоящее время поддерживаются только звонки по протоколу VoIP.</span><span class="sxs-lookup"><span data-stu-id="15646-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="15646-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15646-108">Permissions</span></span>

<span data-ttu-id="15646-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="15646-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="15646-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15646-111">Permission type</span></span>                        | <span data-ttu-id="15646-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15646-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="15646-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15646-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="15646-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15646-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="15646-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15646-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15646-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15646-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="15646-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15646-117">Application</span></span>                            | <span data-ttu-id="15646-118">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls.Iniтиате. Все, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="15646-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="15646-119">**Примечание:** Для вызова с использованием мультимедиа, размещаемого в приложении, вам потребуется разрешение Calls. Акцессмедиа. ALL в дополнение к одному из перечисленных разрешений.</span><span class="sxs-lookup"><span data-stu-id="15646-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="15646-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15646-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="15646-121">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="15646-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="15646-122">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="15646-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15646-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15646-123">Request headers</span></span>
| <span data-ttu-id="15646-124">Имя</span><span class="sxs-lookup"><span data-stu-id="15646-124">Name</span></span>          | <span data-ttu-id="15646-125">Описание</span><span class="sxs-lookup"><span data-stu-id="15646-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="15646-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15646-126">Authorization</span></span> | <span data-ttu-id="15646-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15646-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15646-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15646-129">Content-type</span></span>  | <span data-ttu-id="15646-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15646-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15646-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15646-132">Request body</span></span>
<span data-ttu-id="15646-133">В тексте запроса добавьте представление объекта [Call](../resources/call.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15646-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15646-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="15646-134">Response</span></span>
<span data-ttu-id="15646-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15646-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15646-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="15646-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="15646-137">Пример 1: создание однорангового звонка VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="15646-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="15646-138">**Примечание:** Для этого вызова требуется Calls.Iniтиате. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="15646-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-139">Request</span></span>
<span data-ttu-id="15646-140">В следующем примере показан запрос, который выполняет одноранговый звонок между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="15646-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="15646-141">В этом примере носитель размещается службой.</span><span class="sxs-lookup"><span data-stu-id="15646-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="15646-142">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="15646-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="15646-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="15646-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="15646-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15646-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="15646-145">C#</span><span class="sxs-lookup"><span data-stu-id="15646-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15646-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15646-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15646-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="15646-147">Response</span></span>

> <span data-ttu-id="15646-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="15646-148">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

##### <a name="notification---establishing"></a><span data-ttu-id="15646-149">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="15646-149">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="15646-150">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="15646-150">Notification - established</span></span>

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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="15646-151">Пример 2: создание однорангового звонка VoIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="15646-151">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="15646-152">**Примечание**: в этом примере требуется Calls.Iniтиате. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="15646-152">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-153">Request</span></span>
<span data-ttu-id="15646-154">В следующем примере показан запрос, который выполняет одноранговый звонок между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="15646-154">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="15646-155">В этом примере мультимедиа размещается локально приложением.</span><span class="sxs-lookup"><span data-stu-id="15646-155">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="15646-156">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="15646-156">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="15646-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="15646-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="15646-158">C#</span><span class="sxs-lookup"><span data-stu-id="15646-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15646-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15646-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15646-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15646-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="15646-161">`<Media Session Configuration>` — Это конфигурация сериализованного сеанса мультимедиа, содержащая сведения о сеансе в стеке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="15646-161">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="15646-162">Сведения о звуках, видео, VBSS ссессион должны передаваться здесь.</span><span class="sxs-lookup"><span data-stu-id="15646-162">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="15646-163">Ниже показан пример большого двоичного объекта для сеанса аудио мультимедиа</span><span class="sxs-lookup"><span data-stu-id="15646-163">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="15646-164">**Примечание:** Для одноранговых вызовов ожидаемые уведомления относятся только к изменениям состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="15646-164">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="15646-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="15646-165">Response</span></span>

> <span data-ttu-id="15646-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15646-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="15646-168">Пример 3: Создание группового звонка с размещенными у службы носителями</span><span class="sxs-lookup"><span data-stu-id="15646-168">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="15646-169">Поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="15646-169">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="15646-170">В этом примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="15646-170">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="15646-171">**Примечание:** В этом примере для вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="15646-171">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="15646-172">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="15646-172">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-173">Request</span></span>
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

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="15646-174">Пример 4: создание групповой связи с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="15646-174">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="15646-175">Поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="15646-175">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="15646-176">В этом примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="15646-176">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="15646-177">**Примечание:** В этом примере для вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="15646-177">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="15646-178">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="15646-178">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-179">Request</span></span>
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

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="15646-180">Пример 5: присоединение к запланированному собранию с размещенными на службах носителями</span><span class="sxs-lookup"><span data-stu-id="15646-180">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="15646-181">Чтобы присоединиться к запланированному собранию, необходимо получить идентификатор потока, идентификатор сообщения, идентификатор организатора и идентификатор клиента, на котором запланировано собрание.</span><span class="sxs-lookup"><span data-stu-id="15646-181">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="15646-182">Эту информацию можно получить из [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="15646-182">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="15646-183">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от  [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="15646-183">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="15646-184">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="15646-184">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-185">Request</span></span>

<!-- {
  "blockType": "ignored",
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
##### <a name="response"></a><span data-ttu-id="15646-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="15646-186">Response</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="15646-187">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="15646-187">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="15646-188">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="15646-188">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="15646-189">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="15646-189">Notification - roster</span></span>

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

><span data-ttu-id="15646-190">**Примечание:** При объединении сценариев собраний, отличных от уведомлений о состоянии вызовов, мы получаем уведомления списков.</span><span class="sxs-lookup"><span data-stu-id="15646-190">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="15646-191">Пример 6: присоединение к запланированному собранию с размещенными носителями приложений</span><span class="sxs-lookup"><span data-stu-id="15646-191">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="15646-192">Чтобы присоединиться к собранию с размещенными в приложении носителями, обновите конфигурацию мультимедиа с помощью [апфостедмедиаконфиг](../resources/apphostedmediaconfig.md) , как показано ниже, в приведенном выше примере.</span><span class="sxs-lookup"><span data-stu-id="15646-192">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

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


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="15646-193">Пример 7: присоединение к собранию канала с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="15646-193">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="15646-194">Для собрания в канале требуются определенные сведения, такие как идентификатор потока, идентификатор MessageId и сведения об организаторе, которые можно получить с помощью [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="15646-194">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="15646-195">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от  [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="15646-195">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="15646-196">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="15646-196">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-197">Request</span></span>

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

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="15646-198">Пример 8: присоединение к собранию канала в качестве гостя с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="15646-198">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="15646-199">Для присоединения к собранию по каналу в качестве гостя необходимо создать гостевой [идентификацию](../resources/identityset.md) и добавить ее в качестве источника звонка в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="15646-199">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="15646-200">Отображаемое имя — это имя, которое должно отображаться на собрании для удостоверения гостей.</span><span class="sxs-lookup"><span data-stu-id="15646-200">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="15646-201">Идентификатором может быть уникальный идентификатор, идентифицирующий гостевую идентификацию.</span><span class="sxs-lookup"><span data-stu-id="15646-201">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="15646-202">**Примечание:** В этом примере требуется `Calls.JoinGroupCallsAsGuest.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="15646-202">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15646-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="15646-203">Request</span></span>

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
> <span data-ttu-id="15646-204">**Примечание:** Присоединение к гостевой учету зависит от параметров клиента для собрания.</span><span class="sxs-lookup"><span data-stu-id="15646-204">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="15646-205">Приложение может быть помещено в "зале ожидания" в ожидании, которое может быть допущено пользователем.</span><span class="sxs-lookup"><span data-stu-id="15646-205">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="15646-206">Определяется `isInLobby` свойством.</span><span class="sxs-lookup"><span data-stu-id="15646-206">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="15646-207">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="15646-207">Notification - roster</span></span>

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
> <span data-ttu-id="15646-208">**Примечание:** Приложение не будет получать список участников собрания, пока его допустить в "зале ожидания"</span><span class="sxs-lookup"><span data-stu-id="15646-208">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

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