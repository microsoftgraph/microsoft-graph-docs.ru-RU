---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1892a7f6f0331cad2b0ef74adfba857dd21b2b2
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302383"
---
# <a name="call-answer"></a><span data-ttu-id="b92a4-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="b92a4-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b92a4-104">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="b92a4-104">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="b92a4-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="b92a4-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="b92a4-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="b92a4-106">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="b92a4-107">Ожидается, что Bot отвечает или [отклоняет](./call-reject.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="b92a4-107">The bot is expected to answer or [reject](./call-reject.md) the call before the call times out. The current timeout value is 15 seconds.</span></span>

> <span data-ttu-id="b92a4-108">**Примечание:** С помощью протокола VoIP можно получить доступ только с помощью протокола VoIP.</span><span class="sxs-lookup"><span data-stu-id="b92a4-108">**Note:** The bot can only be reached by VoIP.</span></span> <span data-ttu-id="b92a4-109">Звонки по PSTN не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b92a4-109">PSTN calling isn't supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="b92a4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b92a4-110">Permissions</span></span>
<span data-ttu-id="b92a4-111">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="b92a4-111">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="b92a4-112">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b92a4-112">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="b92a4-113">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92a4-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b92a4-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b92a4-114">Permission type</span></span> | <span data-ttu-id="b92a4-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b92a4-115">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="b92a4-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b92a4-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b92a4-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b92a4-117">Not Supported</span></span>                        |
| <span data-ttu-id="b92a4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b92a4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b92a4-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b92a4-119">Not Supported</span></span>                        |
| <span data-ttu-id="b92a4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b92a4-120">Application</span></span>     | <span data-ttu-id="b92a4-121">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="b92a4-121">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span>                                                         |

> <span data-ttu-id="b92a4-122">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="b92a4-122">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="b92a4-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b92a4-123">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="b92a4-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b92a4-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b92a4-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b92a4-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b92a4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b92a4-126">Request headers</span></span>
| <span data-ttu-id="b92a4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b92a4-127">Name</span></span>          | <span data-ttu-id="b92a4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b92a4-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b92a4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b92a4-129">Authorization</span></span> | <span data-ttu-id="b92a4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b92a4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b92a4-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b92a4-132">Content-type</span></span>  | <span data-ttu-id="b92a4-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b92a4-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b92a4-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b92a4-135">Request body</span></span>
<span data-ttu-id="b92a4-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b92a4-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b92a4-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="b92a4-137">Parameter</span></span>        | <span data-ttu-id="b92a4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="b92a4-138">Type</span></span>                                     |<span data-ttu-id="b92a4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b92a4-139">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b92a4-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="b92a4-140">callbackUri</span></span>       |<span data-ttu-id="b92a4-141">String</span><span class="sxs-lookup"><span data-stu-id="b92a4-141">String</span></span>                                    |<span data-ttu-id="b92a4-142">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="b92a4-142">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="b92a4-143">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="b92a4-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="b92a4-144">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="b92a4-144">This must be `https`.</span></span>    |
|<span data-ttu-id="b92a4-145">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="b92a4-145">acceptedModalities</span></span>|<span data-ttu-id="b92a4-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b92a4-146">String collection</span></span>                         |<span data-ttu-id="b92a4-147">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="b92a4-147">The list of accept modalities.</span></span> <span data-ttu-id="b92a4-148">Возможные значения: `audio`, `video`,. `videoBasedScreenSharing`</span><span class="sxs-lookup"><span data-stu-id="b92a4-148">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="b92a4-149">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="b92a4-149">Required for answering a call.</span></span> |
|<span data-ttu-id="b92a4-150">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="b92a4-150">mediaConfig</span></span>       | <span data-ttu-id="b92a4-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="b92a4-151">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="b92a4-152">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b92a4-152">The media configuration.</span></span> <span data-ttu-id="b92a4-153">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="b92a4-153">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="b92a4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b92a4-154">Response</span></span>
<span data-ttu-id="b92a4-155">Этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="b92a4-155">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b92a4-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="b92a4-156">Examples</span></span>
<span data-ttu-id="b92a4-157">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b92a4-157">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b92a4-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b92a4-158">Request</span></span>
<span data-ttu-id="b92a4-159">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b92a4-159">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b92a4-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="b92a4-160">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="b92a4-161">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="b92a4-161">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="ctabcsharp"></a>[<span data-ttu-id="b92a4-162">C#</span><span class="sxs-lookup"><span data-stu-id="b92a4-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b92a4-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b92a4-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b92a4-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b92a4-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b92a4-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b92a4-165">Response</span></span>
<span data-ttu-id="b92a4-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b92a4-166">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="b92a4-167">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="b92a4-167">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="b92a4-168">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="b92a4-168">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="b92a4-169">Запросить</span><span class="sxs-lookup"><span data-stu-id="b92a4-169">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="b92a4-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="b92a4-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="b92a4-171">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="b92a4-171">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="b92a4-172">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="b92a4-172">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="b92a4-173">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="b92a4-173">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="b92a4-174">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="b92a4-174">Notification - incoming</span></span>

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
            "@odata.type": "#microsoft.graph.participantInfo",
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

##### <a name="request"></a><span data-ttu-id="b92a4-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b92a4-175">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b92a4-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="b92a4-176">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b92a4-177">C#</span><span class="sxs-lookup"><span data-stu-id="b92a4-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b92a4-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b92a4-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b92a4-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b92a4-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b92a4-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="b92a4-180">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="b92a4-181">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="b92a4-181">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="b92a4-182">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="b92a4-182">Notification - established</span></span>

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
