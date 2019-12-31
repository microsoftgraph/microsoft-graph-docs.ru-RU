---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 723c9fff75e3e25d29468faf3bfbdf5cc2db064b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912785"
---
# <a name="call-answer"></a><span data-ttu-id="b5f0f-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="b5f0f-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5f0f-104">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="b5f0f-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="b5f0f-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="b5f0f-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="b5f0f-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="b5f0f-107">Ожидается, что Bot отвечает, [отклоняете](./call-reject.md) или [перенаправляете](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-107">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5f0f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f0f-108">Permissions</span></span>
<span data-ttu-id="b5f0f-109">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-109">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="b5f0f-110">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-110">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="b5f0f-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5f0f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5f0f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f0f-112">Permission type</span></span> | <span data-ttu-id="b5f0f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5f0f-113">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="b5f0f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5f0f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5f0f-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5f0f-115">Not Supported</span></span>                        |
| <span data-ttu-id="b5f0f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5f0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f0f-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b5f0f-117">Not Supported</span></span>                        |
| <span data-ttu-id="b5f0f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5f0f-118">Application</span></span>     | <span data-ttu-id="b5f0f-119">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="b5f0f-119">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="b5f0f-120">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-120">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="b5f0f-121">Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. Акцессмедиа. ALL, Calls. initiate. ALL, Calls. Инитиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-121">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="b5f0f-122">`source` Сведения о вызывающем абоненте в уведомлении о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-122">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="b5f0f-123">Без по крайней мере одного из этих разрешений `source` оно останется зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-123">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5f0f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5f0f-124">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="b5f0f-125">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-125">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b5f0f-126">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-126">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5f0f-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5f0f-127">Request headers</span></span>
| <span data-ttu-id="b5f0f-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b5f0f-128">Name</span></span>          | <span data-ttu-id="b5f0f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f0f-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b5f0f-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5f0f-130">Authorization</span></span> | <span data-ttu-id="b5f0f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5f0f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5f0f-133">Content-type</span></span>  | <span data-ttu-id="b5f0f-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f0f-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5f0f-136">Request body</span></span>
<span data-ttu-id="b5f0f-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5f0f-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5f0f-138">Parameter</span></span>        | <span data-ttu-id="b5f0f-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b5f0f-139">Type</span></span>                                     |<span data-ttu-id="b5f0f-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f0f-140">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b5f0f-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="b5f0f-141">callbackUri</span></span>       |<span data-ttu-id="b5f0f-142">String</span><span class="sxs-lookup"><span data-stu-id="b5f0f-142">String</span></span>                                    |<span data-ttu-id="b5f0f-143">Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-143">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="b5f0f-144">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="b5f0f-145">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-145">This must be `https`.</span></span>    |
|<span data-ttu-id="b5f0f-146">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="b5f0f-146">acceptedModalities</span></span>|<span data-ttu-id="b5f0f-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5f0f-147">String collection</span></span>                         |<span data-ttu-id="b5f0f-148">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-148">The list of accept modalities.</span></span> <span data-ttu-id="b5f0f-149">Возможные значения: `audio`, `video`,. `videoBasedScreenSharing`</span><span class="sxs-lookup"><span data-stu-id="b5f0f-149">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="b5f0f-150">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-150">Required for answering a call.</span></span> |
|<span data-ttu-id="b5f0f-151">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="b5f0f-151">mediaConfig</span></span>       | <span data-ttu-id="b5f0f-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="b5f0f-152">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="b5f0f-153">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-153">The media configuration.</span></span> <span data-ttu-id="b5f0f-154">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="b5f0f-154">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="b5f0f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f0f-155">Response</span></span>
<span data-ttu-id="b5f0f-156">Этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-156">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b5f0f-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5f0f-157">Examples</span></span>
<span data-ttu-id="b5f0f-158">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-158">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b5f0f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5f0f-159">Request</span></span>
<span data-ttu-id="b5f0f-160">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5f0f-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5f0f-161">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="b5f0f-162">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-162">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="b5f0f-163">C#</span><span class="sxs-lookup"><span data-stu-id="b5f0f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5f0f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5f0f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5f0f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5f0f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5f0f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f0f-166">Response</span></span>
<span data-ttu-id="b5f0f-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5f0f-167">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="b5f0f-168">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="b5f0f-168">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="b5f0f-169">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="b5f0f-169">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="b5f0f-170">Запросить</span><span class="sxs-lookup"><span data-stu-id="b5f0f-170">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="b5f0f-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5f0f-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="b5f0f-172">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="b5f0f-172">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="b5f0f-173">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="b5f0f-173">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="b5f0f-174">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="b5f0f-174">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="b5f0f-175">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="b5f0f-175">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="b5f0f-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5f0f-176">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5f0f-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5f0f-177">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5f0f-178">C#</span><span class="sxs-lookup"><span data-stu-id="b5f0f-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5f0f-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5f0f-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5f0f-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5f0f-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5f0f-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f0f-181">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="b5f0f-182">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="b5f0f-182">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="b5f0f-183">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="b5f0f-183">Notification - established</span></span>

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
