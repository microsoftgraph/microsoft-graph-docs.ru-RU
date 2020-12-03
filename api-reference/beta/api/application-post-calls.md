---
title: Создание звонка
description: Создание нового звонка.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6d433987b1d0cd30e3eee0eb8a247d29ed37d950
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521406"
---
# <a name="create-call"></a><span data-ttu-id="58a96-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="58a96-103">Create call</span></span>

<span data-ttu-id="58a96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58a96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58a96-105">Создать [вызов](../resources/call.md) позволяет Bot создать новый исходящий одноранговый или групповой вызов или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="58a96-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="58a96-106">Вам потребуется [зарегистрировать запрашивающий абонент](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) и просмотреть список необходимых разрешений, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="58a96-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="58a96-107">**Примечание:** В настоящее время поддерживаются только звонки по протоколу VoIP.</span><span class="sxs-lookup"><span data-stu-id="58a96-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="58a96-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58a96-108">Permissions</span></span>

<span data-ttu-id="58a96-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="58a96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="58a96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58a96-111">Permission type</span></span>                        | <span data-ttu-id="58a96-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58a96-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="58a96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58a96-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="58a96-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58a96-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="58a96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58a96-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a96-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58a96-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="58a96-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58a96-117">Application</span></span>                            | <span data-ttu-id="58a96-118">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls.Iniтиате. Все, Calls.IniТиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="58a96-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="58a96-119">**Примечание:** Для вызова с использованием мультимедиа, размещаемого в приложении, вам потребуется разрешение Calls. Акцессмедиа. ALL в дополнение к одному из перечисленных разрешений.</span><span class="sxs-lookup"><span data-stu-id="58a96-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed.</span></span>

## <a name="http-request"></a><span data-ttu-id="58a96-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /communications/calls
```
> <span data-ttu-id="58a96-121">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="58a96-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="58a96-122">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="58a96-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58a96-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58a96-123">Request headers</span></span>
| <span data-ttu-id="58a96-124">Имя</span><span class="sxs-lookup"><span data-stu-id="58a96-124">Name</span></span>          | <span data-ttu-id="58a96-125">Описание</span><span class="sxs-lookup"><span data-stu-id="58a96-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="58a96-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58a96-126">Authorization</span></span> | <span data-ttu-id="58a96-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58a96-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58a96-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58a96-129">Content-type</span></span>  | <span data-ttu-id="58a96-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58a96-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a96-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58a96-132">Request body</span></span>
<span data-ttu-id="58a96-133">В тексте запроса добавьте представление объекта [Call](../resources/call.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58a96-133">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="58a96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-134">Response</span></span>
<span data-ttu-id="58a96-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58a96-135">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58a96-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="58a96-136">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="58a96-137">Пример 1: создание однорангового звонка VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-137">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="58a96-138">**Примечание:** Для этого вызова требуется Calls.Iniтиате. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="58a96-138">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-139">Request</span></span>
<span data-ttu-id="58a96-140">В следующем примере показан запрос, который выполняет одноранговый звонок между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="58a96-140">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="58a96-141">В этом примере носитель размещается службой.</span><span class="sxs-lookup"><span data-stu-id="58a96-141">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="58a96-142">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="58a96-142">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="58a96-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="58a96-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="58a96-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58a96-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="58a96-145">C#</span><span class="sxs-lookup"><span data-stu-id="58a96-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58a96-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58a96-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58a96-147">Java</span><span class="sxs-lookup"><span data-stu-id="58a96-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="58a96-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-148">Response</span></span>

> <span data-ttu-id="58a96-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58a96-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

##### <a name="notification---establishing"></a><span data-ttu-id="58a96-150">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="58a96-150">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="58a96-151">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="58a96-151">Notification - established</span></span>

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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="58a96-152">Пример 2: создание однорангового звонка VoIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-152">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="58a96-153">**Примечание**: в этом примере требуется Calls.Iniтиате. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="58a96-153">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-154">Request</span></span>
<span data-ttu-id="58a96-155">В следующем примере показан запрос, который выполняет одноранговый звонок между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="58a96-155">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="58a96-156">В этом примере мультимедиа размещается локально приложением.</span><span class="sxs-lookup"><span data-stu-id="58a96-156">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="58a96-157">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="58a96-157">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="58a96-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="58a96-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="58a96-159">C#</span><span class="sxs-lookup"><span data-stu-id="58a96-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58a96-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58a96-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58a96-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58a96-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58a96-162">Java</span><span class="sxs-lookup"><span data-stu-id="58a96-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="58a96-163">`<Media Session Configuration>` — Это конфигурация сериализованного сеанса мультимедиа, содержащая сведения о сеансе в стеке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="58a96-163">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="58a96-164">Сведения о звуках, видео, VBSS ссессион должны передаваться здесь.</span><span class="sxs-lookup"><span data-stu-id="58a96-164">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="58a96-165">Ниже показан пример большого двоичного объекта для сеанса аудио мультимедиа</span><span class="sxs-lookup"><span data-stu-id="58a96-165">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="58a96-166">**Примечание:** Для одноранговых вызовов ожидаемые уведомления относятся только к изменениям состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="58a96-166">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="58a96-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-167">Response</span></span>

> <span data-ttu-id="58a96-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58a96-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="58a96-170">Пример 3: Создание группового звонка с размещенными у службы носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-170">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="58a96-171">Поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="58a96-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="58a96-172">В этом примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="58a96-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="58a96-173">**Примечание:** В этом примере для вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="58a96-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="58a96-174">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="58a96-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-175">Request</span></span>
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

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="58a96-176">Пример 4: создание групповой связи с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-176">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="58a96-177">Поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="58a96-177">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="58a96-178">В этом примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="58a96-178">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="58a96-179">**Примечание:** В этом примере для вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="58a96-179">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="58a96-180">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="58a96-180">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-181">Request</span></span>
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

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="58a96-182">Пример 5: присоединение к запланированному собранию с размещенными на службах носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-182">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="58a96-183">Чтобы присоединиться к запланированному собранию, необходимо получить идентификатор потока, идентификатор сообщения, идентификатор организатора и идентификатор клиента, на котором запланировано собрание.</span><span class="sxs-lookup"><span data-stu-id="58a96-183">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="58a96-184">Эту информацию можно получить из [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="58a96-184">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="58a96-185">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от  [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="58a96-185">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="58a96-186">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="58a96-186">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-187">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="58a96-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-188">Response</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="58a96-189">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="58a96-189">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="58a96-190">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="58a96-190">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="58a96-191">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="58a96-191">Notification - roster</span></span>

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

><span data-ttu-id="58a96-192">**Примечание:** При объединении сценариев собраний, отличных от уведомлений о состоянии вызовов, мы получаем уведомления списков.</span><span class="sxs-lookup"><span data-stu-id="58a96-192">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="58a96-193">Пример 6: присоединение к запланированному собранию с размещенными носителями приложений</span><span class="sxs-lookup"><span data-stu-id="58a96-193">Example 6: Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="58a96-194">Чтобы присоединиться к собранию с размещенными в приложении носителями, обновите конфигурацию мультимедиа с помощью [апфостедмедиаконфиг](../resources/apphostedmediaconfig.md) , как показано ниже, в приведенном выше примере.</span><span class="sxs-lookup"><span data-stu-id="58a96-194">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

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


### <a name="example-7-join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="58a96-195">Пример 7: присоединение к собранию канала с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-195">Example 7: Join channel meeting with service hosted media</span></span>
<span data-ttu-id="58a96-196">Для собрания в канале требуются определенные сведения, такие как идентификатор потока, идентификатор MessageId и сведения об организаторе, которые можно получить с помощью [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="58a96-196">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="58a96-197">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от  [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="58a96-197">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="58a96-198">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="58a96-198">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-199">Request</span></span>

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

### <a name="example-8-join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="58a96-200">Пример 8: присоединение к собранию канала в качестве гостя с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-200">Example 8: Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="58a96-201">Для присоединения к собранию по каналу в качестве гостя необходимо создать гостевой [идентификацию](../resources/identityset.md) и добавить ее в качестве источника звонка в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="58a96-201">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="58a96-202">Отображаемое имя — это имя, которое должно отображаться на собрании для удостоверения гостей.</span><span class="sxs-lookup"><span data-stu-id="58a96-202">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="58a96-203">Идентификатором может быть уникальный идентификатор, идентифицирующий гостевую идентификацию.</span><span class="sxs-lookup"><span data-stu-id="58a96-203">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="58a96-204">**Примечание:** В этом примере требуется `Calls.JoinGroupCallsAsGuest.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="58a96-204">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="58a96-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-205">Request</span></span>

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
> <span data-ttu-id="58a96-206">**Примечание:** Присоединение к гостевой учету зависит от параметров клиента для собрания.</span><span class="sxs-lookup"><span data-stu-id="58a96-206">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="58a96-207">Приложение может быть помещено в "зале ожидания" в ожидании, которое может быть допущено пользователем.</span><span class="sxs-lookup"><span data-stu-id="58a96-207">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="58a96-208">Определяется `isInLobby` свойством.</span><span class="sxs-lookup"><span data-stu-id="58a96-208">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="58a96-209">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="58a96-209">Notification - roster</span></span>

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
> <span data-ttu-id="58a96-210">**Примечание:** Приложение не будет получать список участников собрания, пока его допустить в "зале ожидания"</span><span class="sxs-lookup"><span data-stu-id="58a96-210">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>

### <a name="example-9-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="58a96-211">Пример 9: создание однорангового звонка PSTN с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-211">Example 9: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="58a96-212">**Примечание:** Для этого вызова требуется Calls.Iniтиате. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="58a96-212">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="58a96-213">Для этого вызова требуется экземпляр приложения с назначенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="58a96-213">This call needs application instance with PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="58a96-214">Шаг 1: создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="58a96-214">Step 1: Create application instance</span></span>
<span data-ttu-id="58a96-215">Чтобы создать экземпляр приложения, администратору клиента необходимо вызвать следующие командлеты в удаленной оболочке PowerShell клиента.</span><span class="sxs-lookup"><span data-stu-id="58a96-215">The tenant admin should call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="58a96-216">Дополнительные сведения см. в статье [New/ксонлинеаппликатионинстанце](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync — ксонлинеаппликатионинстанце](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="58a96-216">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="58a96-217">Шаг 2: Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="58a96-217">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="58a96-218">Используйте учетные данные администратора клиента для входа https://admin.microsoft.com/ и перейдите на вкладку **пользователи и > активные пользователи** .</span><span class="sxs-lookup"><span data-stu-id="58a96-218">Use tenant admin credential to sign in https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="58a96-219">Выберите экземпляр приложения, назначьте **план microsoft 365 для внутренних и международных звонков** , а также **Microsoft 365 телефонную систему — лицензии виртуальных пользователей** и нажмите кнопку **сохранить изменения**.</span><span class="sxs-lookup"><span data-stu-id="58a96-219">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="58a96-220">Если клиенту не хватает этих лицензий, перейдите на вкладку **Услуги по выставлению счетов-> покупок** для приобретения.</span><span class="sxs-lookup"><span data-stu-id="58a96-220">If the tenant is running out of those licenses, go to the **Billing -> Purchase services** tab to purchase.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="58a96-221">Шаг 3: получение номера PSTN</span><span class="sxs-lookup"><span data-stu-id="58a96-221">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="58a96-222">Используйте учетные данные администратора клиента, чтобы войти в систему https://admin.teams.microsoft.com/ и щелкнуть вкладку **портал прежней версии** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="58a96-222">Use tenant admin credential to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="58a96-223">На новой странице перейдите на вкладку **номера телефонов > голосовых вызовов** .</span><span class="sxs-lookup"><span data-stu-id="58a96-223">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="58a96-224">Нажмите кнопку **+** , выберите пункт **новые номера служб** и перейдите на страницу **Добавление новых номеров служб** .</span><span class="sxs-lookup"><span data-stu-id="58a96-224">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="58a96-225">Выберите **страна/регион**, область, **регион**, **город**, входное **количество** и щелкните **Добавить** для поиска.</span><span class="sxs-lookup"><span data-stu-id="58a96-225">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="58a96-226">Щелкните **получить номера**.</span><span class="sxs-lookup"><span data-stu-id="58a96-226">click **acquire numbers**.</span></span> <span data-ttu-id="58a96-227">Вновь приобретенный номер будет отображаться на вкладке **номера телефонов** .</span><span class="sxs-lookup"><span data-stu-id="58a96-227">The newly acquired number will be shown on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="58a96-228">Шаг 4: назначение номера PSTN для экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="58a96-228">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="58a96-229">Администратор клиента должен вызвать следующие командлеты в удаленной оболочке PowerShell клиента для назначения номера PSTN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="58a96-229">The tenant admin should call the following cmdlets on the tenant remote PowerShell to assign PSTN number to  application instance.</span></span> <span data-ttu-id="58a96-230">Дополнительные сведения см. в статье [Set/ксонлиневоицеаппликатионинстанце](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync — ксонлинеаппликатионинстанце](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="58a96-230">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="58a96-231">**Примечание:** Если клиент имеет австралийские номера PSTN, назначенные любому экземпляру приложения, этот вызов может не работать.</span><span class="sxs-lookup"><span data-stu-id="58a96-231">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might not work.</span></span> <span data-ttu-id="58a96-232">Если клиент создан недавно, для него ммигхт требуется несколько дней, чтобы эта функция была доступна.</span><span class="sxs-lookup"><span data-stu-id="58a96-232">If a tenant is newly created, it mmight take several days for this feature to be available.</span></span>

#### <a name="request"></a><span data-ttu-id="58a96-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-233">Request</span></span>
<span data-ttu-id="58a96-234">В приведенном ниже примере показан запрос на выполнение однорангового звонка между Bot и PSTN.</span><span class="sxs-lookup"><span data-stu-id="58a96-234">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="58a96-235">В этом примере носитель размещается службой.</span><span class="sxs-lookup"><span data-stu-id="58a96-235">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="58a96-236">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="58a96-236">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

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

#### <a name="response"></a><span data-ttu-id="58a96-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-237">Response</span></span>

> <span data-ttu-id="58a96-238">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58a96-238">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-10-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="58a96-239">Пример 10: создание однорангового КОММУТИРУЕМого звонка с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="58a96-239">Example 10: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="58a96-240">**Примечание**. для этого примера требуется Calls.Iniтиате. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="58a96-240">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="58a96-241">Для этого вызова требуется экземпляр приложения с назначенным номером PSTN, как описано в примере 9.</span><span class="sxs-lookup"><span data-stu-id="58a96-241">This call needs application instance with PSTN number assigned, as described in Example 9.</span></span>

> <span data-ttu-id="58a96-242">**Примечание:** Если клиент имеет австралийские номера PSTN, назначенные любому экземпляру приложения, этот вызов может не работать.</span><span class="sxs-lookup"><span data-stu-id="58a96-242">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might not work.</span></span> <span data-ttu-id="58a96-243">Если клиент создан заново, для этой функции может потребоваться несколько дней.</span><span class="sxs-lookup"><span data-stu-id="58a96-243">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="request"></a><span data-ttu-id="58a96-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a96-244">Request</span></span>
<span data-ttu-id="58a96-245">В приведенном ниже примере показан запрос на одноранговый звонок между Bot и номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="58a96-245">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="58a96-246">В этом примере мультимедиа размещается локально приложением.</span><span class="sxs-lookup"><span data-stu-id="58a96-246">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="58a96-247">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="58a96-247">The values of authorization token, callback url, application id, application name, user id, user name, and tenant id must be replaced with actual values to make the example work.</span></span>

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

#### <a name="response"></a><span data-ttu-id="58a96-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a96-248">Response</span></span>

> <span data-ttu-id="58a96-249">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58a96-249">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
