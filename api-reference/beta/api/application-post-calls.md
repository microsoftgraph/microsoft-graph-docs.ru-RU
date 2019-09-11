---
title: Создание звонка
description: Создание нового звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e99b1c20ce4666c945016190b7952b67b5c47fdb
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838779"
---
# <a name="create-call"></a><span data-ttu-id="15a09-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="15a09-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15a09-104">Создание [звонка](../resources/call.md) позволяет интерфейсу Bot создать новый исходящий вызов или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="15a09-104">Create [call](../resources/call.md) enables your bot to create a new outgoing call or join an existing meeting.</span></span> <span data-ttu-id="15a09-105">Вам потребуется [зарегистрировать запрашивающий абонент](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) и просмотреть список необходимых разрешений, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="15a09-105">You will need to [register the calling bot](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>


## <a name="permissions"></a><span data-ttu-id="15a09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15a09-106">Permissions</span></span>
<span data-ttu-id="15a09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="15a09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="15a09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15a09-109">Permission type</span></span>                        | <span data-ttu-id="15a09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15a09-110">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="15a09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15a09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15a09-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15a09-112">Not Supported</span></span>                                                                           |
| <span data-ttu-id="15a09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15a09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a09-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="15a09-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="15a09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15a09-115">Application</span></span>                            | <span data-ttu-id="15a09-116">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls. initiate. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="15a09-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="15a09-117">**Примечание:** Кроме того, для вызова с размещенными в приложении носителями требуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="15a09-117">**Note:** In addition, for a call with app hosted media, you need the Calls.AccessMedia.All permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="15a09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
```

## <a name="request-headers"></a><span data-ttu-id="15a09-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15a09-119">Request headers</span></span>
| <span data-ttu-id="15a09-120">Имя</span><span class="sxs-lookup"><span data-stu-id="15a09-120">Name</span></span>          | <span data-ttu-id="15a09-121">Описание</span><span class="sxs-lookup"><span data-stu-id="15a09-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="15a09-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15a09-122">Authorization</span></span> | <span data-ttu-id="15a09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15a09-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15a09-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15a09-125">Request body</span></span>
<span data-ttu-id="15a09-126">В тексте запроса добавьте представление объекта [Call](../resources/call.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15a09-126">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="15a09-127">**Примечание:** Свойства, отмеченные как `Server generated` , игнорируются при обработке. `POST` `app/calls`</span><span class="sxs-lookup"><span data-stu-id="15a09-127">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="15a09-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a09-128">Response</span></span>
<span data-ttu-id="15a09-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15a09-129">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15a09-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="15a09-130">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="15a09-131">Создание однорангового вызова VOIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="15a09-131">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="15a09-132">**Примечание:** Для этого вызова требуется разрешение Calls. initiate. ALL.</span><span class="sxs-lookup"><span data-stu-id="15a09-132">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15a09-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-133">Request</span></span>
<span data-ttu-id="15a09-134">В приведенном ниже примере показан запрос, который выполняет одноранговый вызов между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="15a09-134">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="15a09-135">В этом примере носитель размещается службой.</span><span class="sxs-lookup"><span data-stu-id="15a09-135">In this example the media is hosted by the service.</span></span> <span data-ttu-id="15a09-136">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="15a09-136">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15a09-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="15a09-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
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
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15a09-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15a09-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="15a09-139">C#</span><span class="sxs-lookup"><span data-stu-id="15a09-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15a09-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="15a09-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15a09-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a09-141">Response</span></span>

> <span data-ttu-id="15a09-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15a09-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json


{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
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
      "@odata.type": "#microsoft.graph.participantInfo",
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
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="15a09-144">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="15a09-144">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
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
##### <a name="notification---established"></a><span data-ttu-id="15a09-145">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="15a09-145">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="15a09-146">Создание однорангового вызова VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="15a09-146">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="15a09-147">Note: требуются вызовы. initiate. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="15a09-147">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15a09-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-148">Request</span></span>
<span data-ttu-id="15a09-149">В приведенном ниже примере показан запрос, который выполняет одноранговый вызов между Bot и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="15a09-149">The following example shows the request which makes a peer to peer call between the bot and the specified user.</span></span> <span data-ttu-id="15a09-150">В этом примере мультимедиа размещается локально приложением.</span><span class="sxs-lookup"><span data-stu-id="15a09-150">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="15a09-151">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="15a09-151">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
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
    "blob": "<Media Session Configuration>",
  }
}
```
<span data-ttu-id="15a09-152">`<Media Session Configuration>`— Это конфигурация сериализованного сеанса мультимедиа, содержащая сведения о сеансе в стеке мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="15a09-152">`<Media Session Configuration>` is the serialized media session configuration which contains the session information of the media stack.</span></span> <span data-ttu-id="15a09-153">Сведения о звуках, видео, VBSS ссессион должны передаваться здесь.</span><span class="sxs-lookup"><span data-stu-id="15a09-153">Specific information about audio, video, VBSS ssession information should be passed here.</span></span>

<span data-ttu-id="15a09-154">Ниже показан пример большого двоичного объекта для сеанса аудио мультимедиа</span><span class="sxs-lookup"><span data-stu-id="15a09-154">Sample audio media session blob is shown below</span></span>
```json
{\"mpUri\":\"net.tcp://bot.contoso.com:18732/MediaProcessor\",\"audioRenderContexts\":[\"14778cc4-f54c-43c7-989f-9092e34ef784\"],\"videoRenderContexts\":[],\"audioSourceContexts\":[\"a5dcfc9b-5a54-48ef-86f5-1fdd8508741a\"],\"videoSourceContexts\":[],\"dataRenderContexts\":null,\"dataSourceContexts\":null,\"supportedAudioFormat\":\"Pcm16K\",\"videoSinkEncodingFormats\":[],\"mpMediaSessionId\":\"2379cf46-acf3-4fef-a914-be9627075320\",\"regionAffinity\":null,\"skypeMediaBotsVersion\":\"1.11.1.0086\",\"mediaStackVersion\":\"2018.53.1.1\",\"mpVersion\":\"7.2.0.3881\",\"callId\":\"1b69b141-7f1a-4033-9c34-202737190a20\"}
```

><span data-ttu-id="15a09-155">**Примечание:** Для одноранговых вызовов ожидаемые уведомления относятся только к изменениям состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="15a09-155">**Note:** For peer to peer calls, the expected notifications are for call state changes only.</span></span>

### <a name="join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="15a09-156">Присоединение запланированного собрания с размещенными на службах носителями</span><span class="sxs-lookup"><span data-stu-id="15a09-156">Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="15a09-157">Чтобы присоединиться к запланированному собранию, необходимо получить идентификатор потока, идентификатор сообщения, идентификатор организатора и идентификатор клиента, на котором запланировано собрание.</span><span class="sxs-lookup"><span data-stu-id="15a09-157">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="15a09-158">Эту информацию можно получить из [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="15a09-158">This information can be obtained from [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="15a09-159">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="15a09-159">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>
> <span data-ttu-id="15a09-160">**Примечание:** В `Calls.JoinGroupCalls.All` этом примере требуется разрешение.</span><span class="sxs-lookup"><span data-stu-id="15a09-160">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15a09-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-161">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```
##### <a name="response"></a><span data-ttu-id="15a09-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a09-162">Response</span></span>

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
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
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
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

##### <a name="notification---establishing"></a><span data-ttu-id="15a09-163">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="15a09-163">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---established"></a><span data-ttu-id="15a09-164">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="15a09-164">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
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
##### <a name="notification---roster"></a><span data-ttu-id="15a09-165">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="15a09-165">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
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

><span data-ttu-id="15a09-166">**Примечание:** При объединении сценариев собраний, отличных от уведомлений о состоянии вызовов, мы получаем уведомления списков.</span><span class="sxs-lookup"><span data-stu-id="15a09-166">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="join-scheduled-meeting-with-app-hosted-media"></a><span data-ttu-id="15a09-167">Присоединение к запланированному собранию с размещенными носителями приложений</span><span class="sxs-lookup"><span data-stu-id="15a09-167">Join scheduled meeting with app hosted media</span></span>
<span data-ttu-id="15a09-168">Чтобы присоединиться к собранию с размещенными в приложении носителями, обновите конфигурацию мультимедиа с помощью [апфостедмедиаконфиг](../resources/apphostedmediaconfig.md) , как показано ниже, в приведенном выше примере.</span><span class="sxs-lookup"><span data-stu-id="15a09-168">To join the meeting with application hosted media update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below, In the sample provided above.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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


### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="15a09-169">Присоединение к собранию канала с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="15a09-169">Join channel meeting with service hosted media</span></span>
<span data-ttu-id="15a09-170">Для собрания в канале требуются определенные сведения, такие как идентификатор потока, идентификатор MessageId и сведения об организаторе, которые можно получить с помощью [API получения Интернет-собраний](../api/onlinemeeting-get.md).</span><span class="sxs-lookup"><span data-stu-id="15a09-170">Meeting inside a channel requires specific details like thread id, messageid, and organizer details that can be obtained using the [Get Online Meetings API](../api/onlinemeeting-get.md).</span></span>

<span data-ttu-id="15a09-171">Значения маркера авторизации, URL-адреса обратного вызова, идентификатора приложения, имени приложения, идентификатора пользователя, имени пользователя и идентификатора клиента должны быть заменены вместе со сведениями, полученными от [получения API собраний по сети](../api/onlinemeeting-get.md) с фактическими значениями, чтобы сделать пример работать.</span><span class="sxs-lookup"><span data-stu-id="15a09-171">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) with actual values to make the example work.</span></span>

> <span data-ttu-id="15a09-172">**Примечание:** В `Calls.JoinGroupCalls.All` этом примере требуется разрешение.</span><span class="sxs-lookup"><span data-stu-id="15a09-172">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15a09-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-173">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="15a09-174">Присоединение к собранию канала в качестве гостя с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="15a09-174">Join channel meeting as a guest with service hosted media</span></span>
<span data-ttu-id="15a09-175">Для присоединения к собранию по каналу в качестве гостя необходимо создать гостевой [идентификацию](../resources/identityset.md) и добавить ее в качестве источника звонка в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="15a09-175">For joining a channel meeting as a guest you will need to create a guest [identity](../resources/identityset.md) and add it as the call source in the join meeting request.</span></span>
<span data-ttu-id="15a09-176">Отображаемое имя — это имя, которое должно отображаться на собрании для удостоверения гостей.</span><span class="sxs-lookup"><span data-stu-id="15a09-176">The display name is the name you want to be displayed in the meeting for your guest identity.</span></span> <span data-ttu-id="15a09-177">Идентификатором может быть уникальный идентификатор, идентифицирующий гостевую идентификацию.</span><span class="sxs-lookup"><span data-stu-id="15a09-177">The id may be a unique id identifying the guest identity.</span></span>

> <span data-ttu-id="15a09-178">**Примечание:** В `Calls.JoinGroupCallsAsGuest.All` этом примере требуется разрешение.</span><span class="sxs-lookup"><span data-stu-id="15a09-178">**Note:** This example needs the `Calls.JoinGroupCallsAsGuest.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="15a09-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a09-179">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
Authorization: Bearer <Token>
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
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
> <span data-ttu-id="15a09-180">**Примечание:** Присоединение к гостевой учету зависит от параметров клиента для собрания.</span><span class="sxs-lookup"><span data-stu-id="15a09-180">**Note:** The guest join depends on the tenant settings for meeting.</span></span> <span data-ttu-id="15a09-181">Приложение может быть помещено в "зале ожидания" в ожидании, которое может быть допущено пользователем.</span><span class="sxs-lookup"><span data-stu-id="15a09-181">The application might be put in lobby waiting to be admitted by a user.</span></span> <span data-ttu-id="15a09-182">Определяется `isInLobby` свойством.</span><span class="sxs-lookup"><span data-stu-id="15a09-182">This is defined by the `isInLobby` property</span></span>

##### <a name="notification---roster"></a><span data-ttu-id="15a09-183">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="15a09-183">Notification - Roster</span></span>

```http
POST https://bot.contoso.com/callback
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/2f1a1100-726f-4705-a071-30fb8f6b568f/participants",
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
> <span data-ttu-id="15a09-184">**Примечание:** Приложение не будет получать список участников собрания, пока его допустить в "зале ожидания"</span><span class="sxs-lookup"><span data-stu-id="15a09-184">**Note:** The application will not receive the roster for participants in the meeting until its admitted from lobby</span></span>
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
