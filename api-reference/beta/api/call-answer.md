---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3735532ec12a1b11fad67aa6f1a19fe629324b62
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786582"
---
# <a name="call-answer"></a><span data-ttu-id="2f0e6-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="2f0e6-103">call: answer</span></span>

<span data-ttu-id="2f0e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f0e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f0e6-105">Включить бот для ответа на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="2f0e6-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="2f0e6-106">Входящий запрос может быть приглашением от участника группового звонка или одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="2f0e6-107">Если приглашение на групповой вызов получено, уведомление будет содержать [параметры chatInfo](../resources/chatinfo.md) и [meetingInfo.](../resources/meetinginfo.md)</span><span class="sxs-lookup"><span data-stu-id="2f0e6-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="2f0e6-108">Ожидается, что бот ответит, [отклоняет](./call-reject.md) или [перенаправляет](./call-redirect.md) вызов до времени вызова. Текущее значение времени времени — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-108">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span> <span data-ttu-id="2f0e6-109">Текущее значение расписки составляет 15 секунд для обычных сценариев и 5 секунд для сценариев записи на основе политики.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-109">The current timeout value is 15 seconds for regular scenarios, and 5 seconds for policy-based recording scenarios.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f0e6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f0e6-110">Permissions</span></span>
<span data-ttu-id="2f0e6-111">Для ответа на одноранговой вызов не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-111">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="2f0e6-112">Чтобы присоединиться к групповому вызову, необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-112">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="2f0e6-113">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f0e6-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f0e6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f0e6-114">Permission type</span></span> | <span data-ttu-id="2f0e6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f0e6-115">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="2f0e6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f0e6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f0e6-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2f0e6-117">Not Supported</span></span>                        |
| <span data-ttu-id="2f0e6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f0e6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f0e6-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2f0e6-119">Not Supported</span></span>                        |
| <span data-ttu-id="2f0e6-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f0e6-120">Application</span></span>     | <span data-ttu-id="2f0e6-121">Calls.JoinGroupCalls.All или Calls.JoinGroupCallsasGuest.All</span><span class="sxs-lookup"><span data-stu-id="2f0e6-121">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="2f0e6-122">**Примечание:** Для вызова, использующего средства массовой информации с использованием приложений, также требуется разрешение Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-122">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="2f0e6-123">Для расшифровки входящих уведомлений о вызове необходимо иметь по крайней мере одно из следующих `source` разрешений: Calls.AccessMedia.All, Calls.Initiate. Все, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-123">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="2f0e6-124">Это `source` информация вызываемой в уведомлении о входящих вызовах.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-124">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="2f0e6-125">Без по крайней мере одного из этих разрешений будет `source` оставаться зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-125">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f0e6-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f0e6-126">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="2f0e6-127">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-127">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2f0e6-128">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-128">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f0e6-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f0e6-129">Request headers</span></span>
| <span data-ttu-id="2f0e6-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2f0e6-130">Name</span></span>          | <span data-ttu-id="2f0e6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f0e6-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2f0e6-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f0e6-132">Authorization</span></span> | <span data-ttu-id="2f0e6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f0e6-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f0e6-135">Content-type</span></span>  | <span data-ttu-id="2f0e6-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f0e6-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f0e6-138">Request body</span></span>
<span data-ttu-id="2f0e6-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f0e6-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="2f0e6-140">Parameter</span></span>           | <span data-ttu-id="2f0e6-141">Тип</span><span class="sxs-lookup"><span data-stu-id="2f0e6-141">Type</span></span>                                                                                                                                 | <span data-ttu-id="2f0e6-142">Описание</span><span class="sxs-lookup"><span data-stu-id="2f0e6-142">Description</span></span>                                                                                                                                                                                                         |
| :-----------------  | :-----------------------------------------                                                                                           | :----------------------------------------------------------------------------------------------------------------------------------------------                                                                     |
| <span data-ttu-id="2f0e6-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="2f0e6-143">callbackUri</span></span>         | <span data-ttu-id="2f0e6-144">String</span><span class="sxs-lookup"><span data-stu-id="2f0e6-144">String</span></span>                                                                                                                               | <span data-ttu-id="2f0e6-145">Позволяет ботам предоставлять определенный URI вызова для параллельного вызова для получения более поздних уведомлений.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-145">Allows bots to provide a specific callback URI for the concurrent call to receive later notifications.</span></span> <span data-ttu-id="2f0e6-146">Если это свойство не установлено, вместо него будет использоваться глобальный URI вызова бота.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-146">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="2f0e6-147">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="2f0e6-147">This must be `https`.</span></span> |
| <span data-ttu-id="2f0e6-148">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="2f0e6-148">acceptedModalities</span></span>  | <span data-ttu-id="2f0e6-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f0e6-149">String collection</span></span>                                                                                                                    | <span data-ttu-id="2f0e6-150">Список модальных способов для приемки.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-150">The list of accept modalities.</span></span> <span data-ttu-id="2f0e6-151">Возможное значение: `audio` `video` , `videoBasedScreenSharing` .</span><span class="sxs-lookup"><span data-stu-id="2f0e6-151">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="2f0e6-152">Требуется для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-152">Required for answering a call.</span></span>                                                                                      |
| <span data-ttu-id="2f0e6-153">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="2f0e6-153">mediaConfig</span></span>         | <span data-ttu-id="2f0e6-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="2f0e6-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> | <span data-ttu-id="2f0e6-155">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-155">The media configuration.</span></span> <span data-ttu-id="2f0e6-156">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-156">Required.</span></span>                                                                                                                                                                                 |
| <span data-ttu-id="2f0e6-157">participantCapacity</span><span class="sxs-lookup"><span data-stu-id="2f0e6-157">participantCapacity</span></span> | <span data-ttu-id="2f0e6-158">Целое</span><span class="sxs-lookup"><span data-stu-id="2f0e6-158">Int</span></span>                                                                                                                                  | <span data-ttu-id="2f0e6-159">Число участников, которые приложение может обрабатывать для вызова, для Teams [сценарий](/MicrosoftTeams/teams-recording-policy) записи на основе политики.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-159">The number of participant that the application can handle for the call, for [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) scenario.</span></span>                                                     |

## <a name="response"></a><span data-ttu-id="2f0e6-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f0e6-160">Response</span></span>
<span data-ttu-id="2f0e6-161">Этот метод возвращает код `202 Accepted` ответа.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-161">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2f0e6-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f0e6-162">Examples</span></span>
<span data-ttu-id="2f0e6-163">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-163">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2f0e6-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f0e6-164">Request</span></span>
<span data-ttu-id="2f0e6-165">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-165">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f0e6-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f0e6-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  },
  "acceptedModalities": [
    "audio"
  ],
  "participantCapacity": 200
}
```
<span data-ttu-id="2f0e6-167">Эта blob — это сериализованная конфигурация сеансов мультимедиа, которая создается из SDK мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-167">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="2f0e6-168">C#</span><span class="sxs-lookup"><span data-stu-id="2f0e6-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f0e6-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f0e6-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f0e6-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f0e6-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f0e6-171">Java</span><span class="sxs-lookup"><span data-stu-id="2f0e6-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f0e6-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f0e6-172">Response</span></span>
<span data-ttu-id="2f0e6-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-173">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="2f0e6-174">Пример 1. Ответ на вызов VoIP одноранговой службы с помощью средства массовой информации службы.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-174">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="2f0e6-175">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="2f0e6-175">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "callRoutes": [
          {
            "routingType": "lookup",
            "original": {
              "phone": {
                "id": "+14258828080"
              }
            },
            "final": {
              "user": {
                "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
                "displayName": "Heidi Steen"
              }
            }
          }
        ],
        "source": {
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="2f0e6-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f0e6-176">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "call-answer-service-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
      {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        "uri": "https://cdn.contoso.com/cool.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="2f0e6-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f0e6-177">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="2f0e6-178">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="2f0e6-178">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="2f0e6-179">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="2f0e6-179">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="2f0e6-180">Пример 2. Отвечать на вызов VOIP с помощью носители, на которые было организовано приложение.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-180">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="2f0e6-181">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="2f0e6-181">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "changeType": "created",
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "@odata.type": "#microsoft.graph.participantInfo",
          "identity": {
            "user": {
              "displayName": "Test User",
              "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "application": {
                "displayName": "Test BOT",
                "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="2f0e6-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f0e6-182">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2f0e6-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f0e6-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer-app-hosted-media"
}-->
```http
POST /communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration Blob>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2f0e6-184">C#</span><span class="sxs-lookup"><span data-stu-id="2f0e6-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f0e6-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f0e6-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f0e6-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f0e6-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f0e6-187">Java</span><span class="sxs-lookup"><span data-stu-id="2f0e6-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f0e6-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f0e6-188">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="2f0e6-189">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="2f0e6-189">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="2f0e6-190">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="2f0e6-190">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="example-3-answer-a-policy-based-recording-call"></a><span data-ttu-id="2f0e6-191">Пример 3. Ответ на вызов записи на основе политики</span><span class="sxs-lookup"><span data-stu-id="2f0e6-191">Example 3: Answer a policy-based recording call</span></span>

<span data-ttu-id="2f0e6-192">В [сценарии записи](/microsoftteams/teams-recording-policy)на основе политики перед тем, как участник политики присоединяется к вызову, боту, связанному с политикой, будет отправлено уведомление о входящих вызовах.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-192">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under policy joins a call, an incoming call notification will be sent to the bot associated with the policy.</span></span>
<span data-ttu-id="2f0e6-193">Сведения о присоединиться можно найти в свойстве **botData.**</span><span class="sxs-lookup"><span data-stu-id="2f0e6-193">The join information can be found under the **botData** property.</span></span> <span data-ttu-id="2f0e6-194">Затем бот может ответить на вызов и [соответствующим образом обновить состояние](call-updaterecordingstatus.md) записи.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-194">The bot can then choose to answer the call and [update the recording status](call-updaterecordingstatus.md) accordingly.</span></span>

<span data-ttu-id="2f0e6-195">Если указано в запросе на уведомление о записи на основе политики, последующее присоединение участника к той же группе политик будет отправлено в качестве `participantCpapacity` `Answer` [участникаJoiningNotification](../resources/participantJoiningNotification.md) вместо нового уведомления о входящих вызовах, пока число участников, которые обработка текущего экземпляра вызовов не достигла указанного в `participantCapacity` номере .</span><span class="sxs-lookup"><span data-stu-id="2f0e6-195">When `participantCpapacity` is specified in the `Answer` request for a policy-based recording notification, subsequent participant joining event belonging to the same policy group will be sent out as [participantJoiningNotification](../resources/participantJoiningNotification.md) instead of new incoming call notification, until number of participants that current call instance is handling has reached the number specified in `participantCapacity`.</span></span>

<span data-ttu-id="2f0e6-196">Ниже приводится пример входящих уведомлений о вызове, которые бот получит в этом случае.</span><span class="sxs-lookup"><span data-stu-id="2f0e6-196">The following is an example of the incoming call notification that a bot would recieve in this case.</span></span>

```json
{
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"created",
         "resource":"/app/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceUrl":"/communications/calls/e71f0300-9c1f-4d99-b5f4-2722e877d497",
         "resourceData":{
            "@odata.type":"#microsoft.graph.call",
            "state":"incoming",
            "direction":"incoming",
            "source":{
               "@odata.type":"#microsoft.graph.participantInfo",
               "id":"90fad2ce-8989-41a1-8a66-f6636e629a2a",
               "identity":{
                  "@odata.type":"#microsoft.graph.identitySet",
                  "user":{
                     "@odata.type":"#microsoft.graph.identity",
                     "id":"8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
                     "identityProvider":"AAD"
                  }
               },
               "endpointType":"default",
               "region":"amer"
            },
            "targets":[
               {
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "applicationInstance":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"832899f8-2ea1-4604-8413-27bd2892079f",
                        "identityProvider":"AAD"
                     }
                  },
                  "endpointType":"default",
                  "id":"4520a1a5-5394-5a41-aa12-9ee6fa18cfc8",
                  "region":null,
                  "languageId":null
               }
            ],
            "meetingInfo":{
               "@odata.type":"#microsoft.graph.tokenMeetingInfo",
               "token":"join token"
            },
            "tenantId":"932899f8-2ea1-4604-8413-27bd2892079f",
            "myParticipantId":"1520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
            "callChainId":"05f2f70f-3a9c-47c1-80a9-cc79e91d8cec",
            "incomingContext":{
               "@odata.type":"#microsoft.graph.incomingContext",
               "sourceParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a",
               "observedParticipantId":"30fad2ce-8989-41a1-8a66-f6636e629a2a"
            },
            "id":"e71f0300-9c1f-4d99-b5f4-2722e877d497",
            "applicationMetadata":{
               "botData":{
                  "mediaHostedRegion":"USEA",
                  "user":{
                     "participationMethod":"callee",
                     "clientLocation":"US"
                  },
                  "otherSideUser":{
                     "id":"971f0300-9c1f-4d99-b5f4-2722e877d490",
                     "participantId":"3520a1a5-5394-4a41-aa72-9ee6fa18cfc8",
                     "tenantId":"1540a1a5-2394-4a41-aa72-9ee6fa18cfc8",
                     "onBehalfOf":{
                        "id":"871f0300-9c1f-4d99-b5f4-2722e877d490"
                     },
                     "participationMethod":"caller",
                     "clientLocation":"EUNO"
                  },
                  "inviteReasons":[
                     "PolicyBasedRecording"
                  ],
                  "policyIdentifier":"Test Policy",
                  "pairedRecorders":[
                     {
                        "id":"471f0300-5c1f-4d99-b5f4-2722e877d490",
                        "participantId":"371f0300-2c1f-4d99-b5f4-2722e877d490"
                     }
                  ],
                  "otherRecorders":[
                     {
                        "id":"671f0300-9c1f-4d99-b5f4-2722e877d490",
                        "participantId":"a71f0300-ec1f-4d99-b5f4-2722e877d490"
                     }
                  ]
               }
            }
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
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
