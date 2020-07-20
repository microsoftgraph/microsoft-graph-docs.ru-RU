---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ccb98b3e194026c8f3fc7760a51567d2198306e3
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183885"
---
# <a name="call-answer"></a><span data-ttu-id="fddb6-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="fddb6-103">call: answer</span></span>

<span data-ttu-id="fddb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fddb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fddb6-105">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="fddb6-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="fddb6-106">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="fddb6-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="fddb6-107">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="fddb6-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="fddb6-108">Ожидается, что Bot отвечает, [отклоняете](./call-reject.md) или [перенаправляете](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="fddb6-108">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="fddb6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fddb6-109">Permissions</span></span>
<span data-ttu-id="fddb6-110">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="fddb6-110">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="fddb6-111">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="fddb6-111">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="fddb6-112">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fddb6-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fddb6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fddb6-113">Permission type</span></span> | <span data-ttu-id="fddb6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fddb6-114">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="fddb6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fddb6-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="fddb6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fddb6-116">Not Supported</span></span>                        |
| <span data-ttu-id="fddb6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fddb6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fddb6-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fddb6-118">Not Supported</span></span>                        |
| <span data-ttu-id="fddb6-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="fddb6-119">Application</span></span>     | <span data-ttu-id="fddb6-120">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="fddb6-120">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="fddb6-121">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="fddb6-121">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="fddb6-122">Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. акцессмедиа. ALL, Calls.Iniтиате. ALL, Calls.IniТиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="fddb6-122">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="fddb6-123">`source`Сведения о вызывающем абоненте в уведомлении о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="fddb6-123">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="fddb6-124">Без по крайней мере одного из этих разрешений оно `source` останется зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="fddb6-124">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="fddb6-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fddb6-125">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="fddb6-126">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="fddb6-126">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="fddb6-127">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="fddb6-127">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fddb6-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fddb6-128">Request headers</span></span>
| <span data-ttu-id="fddb6-129">Имя</span><span class="sxs-lookup"><span data-stu-id="fddb6-129">Name</span></span>          | <span data-ttu-id="fddb6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fddb6-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fddb6-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fddb6-131">Authorization</span></span> | <span data-ttu-id="fddb6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fddb6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fddb6-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fddb6-134">Content-type</span></span>  | <span data-ttu-id="fddb6-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fddb6-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fddb6-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fddb6-137">Request body</span></span>
<span data-ttu-id="fddb6-138">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fddb6-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fddb6-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="fddb6-139">Parameter</span></span>        | <span data-ttu-id="fddb6-140">Тип</span><span class="sxs-lookup"><span data-stu-id="fddb6-140">Type</span></span>                                     |<span data-ttu-id="fddb6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="fddb6-141">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fddb6-142">callbackUri</span><span class="sxs-lookup"><span data-stu-id="fddb6-142">callbackUri</span></span>       |<span data-ttu-id="fddb6-143">String</span><span class="sxs-lookup"><span data-stu-id="fddb6-143">String</span></span>                                    |<span data-ttu-id="fddb6-144">Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="fddb6-144">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="fddb6-145">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="fddb6-145">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="fddb6-146">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="fddb6-146">This must be `https`.</span></span>    |
|<span data-ttu-id="fddb6-147">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="fddb6-147">acceptedModalities</span></span>|<span data-ttu-id="fddb6-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fddb6-148">String collection</span></span>                         |<span data-ttu-id="fddb6-149">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="fddb6-149">The list of accept modalities.</span></span> <span data-ttu-id="fddb6-150">Возможные значения: `audio` , `video` , `videoBasedScreenSharing` .</span><span class="sxs-lookup"><span data-stu-id="fddb6-150">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="fddb6-151">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="fddb6-151">Required for answering a call.</span></span> |
|<span data-ttu-id="fddb6-152">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="fddb6-152">mediaConfig</span></span>       | <span data-ttu-id="fddb6-153">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="fddb6-153">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="fddb6-154">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="fddb6-154">The media configuration.</span></span> <span data-ttu-id="fddb6-155">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="fddb6-155">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="fddb6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fddb6-156">Response</span></span>
<span data-ttu-id="fddb6-157">Этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="fddb6-157">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fddb6-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="fddb6-158">Examples</span></span>
<span data-ttu-id="fddb6-159">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fddb6-159">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fddb6-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="fddb6-160">Request</span></span>
<span data-ttu-id="fddb6-161">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fddb6-161">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fddb6-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="fddb6-162">HTTP</span></span>](#tab/http)
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
  ]
}
```
<span data-ttu-id="fddb6-163">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="fddb6-163">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="fddb6-164">C#</span><span class="sxs-lookup"><span data-stu-id="fddb6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fddb6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fddb6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fddb6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fddb6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fddb6-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="fddb6-167">Response</span></span>
<span data-ttu-id="fddb6-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fddb6-168">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="fddb6-169">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="fddb6-169">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="fddb6-170">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="fddb6-170">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="fddb6-171">Запросить</span><span class="sxs-lookup"><span data-stu-id="fddb6-171">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="fddb6-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="fddb6-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="fddb6-173">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="fddb6-173">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="fddb6-174">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="fddb6-174">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="fddb6-175">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="fddb6-175">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="fddb6-176">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="fddb6-176">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="fddb6-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="fddb6-177">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fddb6-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="fddb6-178">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fddb6-179">C#</span><span class="sxs-lookup"><span data-stu-id="fddb6-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fddb6-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fddb6-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fddb6-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fddb6-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fddb6-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="fddb6-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="fddb6-183">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="fddb6-183">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="fddb6-184">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="fddb6-184">Notification - established</span></span>

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

### <a name="example-3-answer-a-policy-based-recording-call"></a><span data-ttu-id="fddb6-185">Пример 3: ответ на вызов записи на основе политики</span><span class="sxs-lookup"><span data-stu-id="fddb6-185">Example 3: Answer a policy-based recording call</span></span>

<span data-ttu-id="fddb6-186">В [сценарии записи на основе политик](https://docs.microsoft.com/microsoftteams/teams-recording-policy), прежде чем участник политики присоединяется к вызову, на Bot, связанном с политикой, будет отправлено уведомление о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="fddb6-186">Under the [Policy-based recording scenario](https://docs.microsoft.com/microsoftteams/teams-recording-policy), before a participant under policy joins a call, an incoming call notification will be sent to the bot associated with the policy.</span></span>
<span data-ttu-id="fddb6-187">Сведения о присоединении можно найти в свойстве **ботдата** .</span><span class="sxs-lookup"><span data-stu-id="fddb6-187">The join information can be found under the **botData** property.</span></span> <span data-ttu-id="fddb6-188">С помощью Bot можно выбрать ответ на вызов и соответствующим образом [Обновить состояние записи](call-updaterecordingstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="fddb6-188">The bot can then choose to answer the call and [update the recording status](call-updaterecordingstatus.md) accordingly.</span></span>

<span data-ttu-id="fddb6-189">Ниже приведен пример уведомления о входящем вызове, которое получит робота в этом случае.</span><span class="sxs-lookup"><span data-stu-id="fddb6-189">The following is an example of the incoming call notification that a bot would recieve in this case.</span></span>

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
