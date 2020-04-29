---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ca7cfb0a8f1851727138a21e92a3df8a2b968513
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518751"
---
# <a name="call-answer"></a><span data-ttu-id="41733-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="41733-103">call: answer</span></span>

<span data-ttu-id="41733-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41733-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41733-105">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="41733-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="41733-106">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="41733-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="41733-107">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="41733-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="41733-108">Ожидается, что Bot отвечает, [отклоняется](./call-reject.md)или [перенаправляется](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="41733-108">The bot is expected to answer, [reject](./call-reject.md), or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="41733-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41733-109">Permissions</span></span>
<span data-ttu-id="41733-110">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="41733-110">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="41733-111">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="41733-111">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="41733-112">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41733-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41733-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41733-113">Permission type</span></span> | <span data-ttu-id="41733-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41733-114">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="41733-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41733-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="41733-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="41733-116">Not Supported</span></span>                        |
| <span data-ttu-id="41733-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41733-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41733-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="41733-118">Not Supported</span></span>                        |
| <span data-ttu-id="41733-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41733-119">Application</span></span>     | <span data-ttu-id="41733-120">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="41733-120">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="41733-121">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="41733-121">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="41733-122">Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. Акцессмедиа. ALL, Calls. initiate. ALL, Calls. Инитиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="41733-122">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="41733-123">`source` Сведения о вызывающем абоненте в уведомлении о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="41733-123">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="41733-124">Без по крайней мере одного из этих разрешений `source` оно останется зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="41733-124">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="41733-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41733-125">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="41733-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41733-126">Request headers</span></span>
| <span data-ttu-id="41733-127">Имя</span><span class="sxs-lookup"><span data-stu-id="41733-127">Name</span></span>          | <span data-ttu-id="41733-128">Описание</span><span class="sxs-lookup"><span data-stu-id="41733-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="41733-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41733-129">Authorization</span></span> | <span data-ttu-id="41733-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41733-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41733-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41733-132">Content-type</span></span>  | <span data-ttu-id="41733-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41733-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41733-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41733-135">Request body</span></span>
<span data-ttu-id="41733-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="41733-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="41733-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="41733-137">Parameter</span></span>        | <span data-ttu-id="41733-138">Тип</span><span class="sxs-lookup"><span data-stu-id="41733-138">Type</span></span>                                     |<span data-ttu-id="41733-139">Описание</span><span class="sxs-lookup"><span data-stu-id="41733-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="41733-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="41733-140">callbackUri</span></span>       |<span data-ttu-id="41733-141">String</span><span class="sxs-lookup"><span data-stu-id="41733-141">String</span></span>                                    |<span data-ttu-id="41733-142">Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="41733-142">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="41733-143">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="41733-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="41733-144">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="41733-144">This must be `https`.</span></span>    |
|<span data-ttu-id="41733-145">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="41733-145">acceptedModalities</span></span>|<span data-ttu-id="41733-146">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="41733-146">String collection</span></span>                         |<span data-ttu-id="41733-147">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="41733-147">The list of accept modalities.</span></span> <span data-ttu-id="41733-148">Возможные значения: `audio`, `video`, `videoBasedScreenSharing`.</span><span class="sxs-lookup"><span data-stu-id="41733-148">Possible values are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="41733-149">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="41733-149">Required for answering a call.</span></span> |
|<span data-ttu-id="41733-150">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="41733-150">mediaConfig</span></span>       | <span data-ttu-id="41733-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="41733-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="41733-152">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="41733-152">The media configuration.</span></span> <span data-ttu-id="41733-153">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="41733-153">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="41733-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="41733-154">Response</span></span>
<span data-ttu-id="41733-155">Этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="41733-155">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="41733-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="41733-156">Examples</span></span>
<span data-ttu-id="41733-157">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="41733-157">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="41733-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="41733-158">Request</span></span>
<span data-ttu-id="41733-159">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41733-159">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="41733-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="41733-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/answer
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
<span data-ttu-id="41733-161">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="41733-161">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="41733-162">C#</span><span class="sxs-lookup"><span data-stu-id="41733-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41733-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41733-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41733-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41733-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41733-165">Java</span><span class="sxs-lookup"><span data-stu-id="41733-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41733-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="41733-166">Response</span></span>
<span data-ttu-id="41733-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41733-167">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="41733-168">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="41733-168">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="41733-169">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="41733-169">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="41733-170">Запросить</span><span class="sxs-lookup"><span data-stu-id="41733-170">Request</span></span>

<!-- {
  "blockType": "request",
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

##### <a name="response"></a><span data-ttu-id="41733-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="41733-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="41733-172">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="41733-172">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="41733-173">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="41733-173">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="41733-174">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="41733-174">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="41733-175">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="41733-175">Notification - incoming</span></span>

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
            }
          }
        ],
        "requestedModalities": [ "audio" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="41733-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="41733-176">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="41733-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="41733-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="41733-178">C#</span><span class="sxs-lookup"><span data-stu-id="41733-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41733-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41733-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41733-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41733-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41733-181">Java</span><span class="sxs-lookup"><span data-stu-id="41733-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41733-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="41733-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="41733-183">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="41733-183">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="41733-184">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="41733-184">Notification - established</span></span>

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
