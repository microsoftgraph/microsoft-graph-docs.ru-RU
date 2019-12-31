---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4df2ddafad5dc2dd22852101f32ba46f8f15fe56
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913375"
---
# <a name="call-answer"></a><span data-ttu-id="6435a-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="6435a-103">call: answer</span></span>

<span data-ttu-id="6435a-104">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="6435a-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="6435a-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="6435a-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="6435a-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="6435a-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="6435a-107">Ожидается, что Bot отвечает, [отклоняется](./call-reject.md)или [перенаправляется](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="6435a-107">The bot is expected to answer, [reject](./call-reject.md), or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="6435a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6435a-108">Permissions</span></span>
<span data-ttu-id="6435a-109">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="6435a-109">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="6435a-110">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="6435a-110">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="6435a-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6435a-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6435a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6435a-112">Permission type</span></span> | <span data-ttu-id="6435a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6435a-113">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="6435a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6435a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="6435a-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6435a-115">Not Supported</span></span>                        |
| <span data-ttu-id="6435a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6435a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6435a-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6435a-117">Not Supported</span></span>                        |
| <span data-ttu-id="6435a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6435a-118">Application</span></span>     | <span data-ttu-id="6435a-119">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="6435a-119">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="6435a-120">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="6435a-120">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="6435a-121">Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. Акцессмедиа. ALL, Calls. initiate. ALL, Calls. Инитиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="6435a-121">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="6435a-122">`source` Сведения о вызывающем абоненте в уведомлении о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="6435a-122">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="6435a-123">Без по крайней мере одного из этих разрешений `source` оно останется зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="6435a-123">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="6435a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6435a-124">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /communications/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="6435a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6435a-125">Request headers</span></span>
| <span data-ttu-id="6435a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="6435a-126">Name</span></span>          | <span data-ttu-id="6435a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6435a-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6435a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6435a-128">Authorization</span></span> | <span data-ttu-id="6435a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6435a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6435a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6435a-131">Content-type</span></span>  | <span data-ttu-id="6435a-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6435a-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6435a-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6435a-134">Request body</span></span>
<span data-ttu-id="6435a-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6435a-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6435a-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="6435a-136">Parameter</span></span>        | <span data-ttu-id="6435a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6435a-137">Type</span></span>                                     |<span data-ttu-id="6435a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6435a-138">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6435a-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="6435a-139">callbackUri</span></span>       |<span data-ttu-id="6435a-140">String</span><span class="sxs-lookup"><span data-stu-id="6435a-140">String</span></span>                                    |<span data-ttu-id="6435a-141">Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="6435a-141">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="6435a-142">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="6435a-142">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="6435a-143">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="6435a-143">This must be `https`.</span></span>    |
|<span data-ttu-id="6435a-144">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="6435a-144">acceptedModalities</span></span>|<span data-ttu-id="6435a-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6435a-145">String collection</span></span>                         |<span data-ttu-id="6435a-146">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="6435a-146">The list of accept modalities.</span></span> <span data-ttu-id="6435a-147">Возможные значения: `audio`, `video`, `videoBasedScreenSharing`.</span><span class="sxs-lookup"><span data-stu-id="6435a-147">Possible values are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="6435a-148">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="6435a-148">Required for answering a call.</span></span> |
|<span data-ttu-id="6435a-149">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="6435a-149">mediaConfig</span></span>       | <span data-ttu-id="6435a-150">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="6435a-150">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="6435a-151">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="6435a-151">The media configuration.</span></span> <span data-ttu-id="6435a-152">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="6435a-152">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="6435a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6435a-153">Response</span></span>
<span data-ttu-id="6435a-154">Этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="6435a-154">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6435a-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="6435a-155">Examples</span></span>
<span data-ttu-id="6435a-156">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6435a-156">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6435a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6435a-157">Request</span></span>
<span data-ttu-id="6435a-158">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6435a-158">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6435a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="6435a-159">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="6435a-160">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="6435a-160">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="6435a-161">C#</span><span class="sxs-lookup"><span data-stu-id="6435a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6435a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6435a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6435a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6435a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6435a-164">Java</span><span class="sxs-lookup"><span data-stu-id="6435a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6435a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6435a-165">Response</span></span>
<span data-ttu-id="6435a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6435a-166">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="6435a-167">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="6435a-167">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6435a-168">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6435a-168">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6435a-169">Запросить</span><span class="sxs-lookup"><span data-stu-id="6435a-169">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="6435a-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6435a-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6435a-171">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="6435a-171">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="6435a-172">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="6435a-172">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="6435a-173">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="6435a-173">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="6435a-174">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="6435a-174">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="6435a-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="6435a-175">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6435a-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="6435a-176">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6435a-177">C#</span><span class="sxs-lookup"><span data-stu-id="6435a-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6435a-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6435a-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6435a-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6435a-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6435a-180">Java</span><span class="sxs-lookup"><span data-stu-id="6435a-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6435a-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="6435a-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="6435a-182">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="6435a-182">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="6435a-183">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="6435a-183">Notification - established</span></span>

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
