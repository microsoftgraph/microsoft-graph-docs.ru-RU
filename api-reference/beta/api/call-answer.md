---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b5adda4a535987f7a23066911ad2e45ad89871eb
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563236"
---
# <a name="call-answer"></a><span data-ttu-id="25f7c-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="25f7c-103">call: answer</span></span>

<span data-ttu-id="25f7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25f7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25f7c-105">Разрешить интерфейсу Bot ответить на входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="25f7c-105">Enable a bot to answer an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="25f7c-106">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="25f7c-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="25f7c-107">При получении приглашения на вызов группы в уведомлении будут содержаться параметры [чатинфо](../resources/chatinfo.md) и [митингинфо](../resources/meetinginfo.md) .</span><span class="sxs-lookup"><span data-stu-id="25f7c-107">If an invite to a group call is received, the notification will contain the [chatInfo](../resources/chatinfo.md) and [meetingInfo](../resources/meetinginfo.md) parameters.</span></span>

<span data-ttu-id="25f7c-108">Ожидается, что Bot отвечает, [отклоняете](./call-reject.md) или [перенаправляете](./call-redirect.md) вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="25f7c-108">The bot is expected to answer, [reject](./call-reject.md) or [redirect](./call-redirect.md) the call before the call times out. The current timeout value is 15 seconds.</span></span> <span data-ttu-id="25f7c-109">Текущее значение времени ожидания составляет 15 секунд для обычных сценариев и 5 секунд для сценариев записи на основе политик.</span><span class="sxs-lookup"><span data-stu-id="25f7c-109">The current timeout value is 15 seconds for regular scenarios, and 5 seconds for policy-based recording scenarios.</span></span>

## <a name="permissions"></a><span data-ttu-id="25f7c-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="25f7c-110">Permissions</span></span>
<span data-ttu-id="25f7c-111">Для ответа на одноранговый звонок не требуется никаких разрешений.</span><span class="sxs-lookup"><span data-stu-id="25f7c-111">You do not need any permissions to answer a peer-to-peer call.</span></span> <span data-ttu-id="25f7c-112">Для присоединения к группе необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="25f7c-112">You need one of the following permissions to join a group call.</span></span> <span data-ttu-id="25f7c-113">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f7c-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25f7c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25f7c-114">Permission type</span></span> | <span data-ttu-id="25f7c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25f7c-115">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="25f7c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25f7c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="25f7c-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="25f7c-117">Not Supported</span></span>                        |
| <span data-ttu-id="25f7c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25f7c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25f7c-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="25f7c-119">Not Supported</span></span>                        |
| <span data-ttu-id="25f7c-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="25f7c-120">Application</span></span>     | <span data-ttu-id="25f7c-121">Calls. Жоинграупкаллс. ALL или Calls. Жоинграупкаллсасгуест. ALL</span><span class="sxs-lookup"><span data-stu-id="25f7c-121">Calls.JoinGroupCalls.All or Calls.JoinGroupCallsasGuest.All</span></span> |

> <span data-ttu-id="25f7c-122">**Примечание:** Для вызова, использующего носитель с размещением приложений, вам также потребуется разрешение Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="25f7c-122">**Note:** For a call that uses application-hosted media, you also need the Calls.AccessMedia.All permission.</span></span> <span data-ttu-id="25f7c-123">Необходимо иметь по крайней мере одно из следующих разрешений, чтобы обеспечить `source` расшифровку уведомления о входящем вызове: Calls. акцессмедиа. ALL, Calls.Iniтиате. ALL, Calls.IniТиатеграупкалл. ALL, Calls. Жоинграупкалл. ALL, Calls. Жоинграупкалласгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="25f7c-123">You must have at least one of the following permissions to ensure that the `source` in the incoming call notification is decrypted: Calls.AccessMedia.All, Calls.Initiate.All, Calls.InitiateGroupCall.All, Calls.JoinGroupCall.All, Calls.JoinGroupCallAsGuest.All.</span></span> <span data-ttu-id="25f7c-124">`source`Сведения о вызывающем абоненте в уведомлении о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="25f7c-124">The `source` is the caller info in the incoming call notification.</span></span> <span data-ttu-id="25f7c-125">Без по крайней мере одного из этих разрешений оно `source` останется зашифрованным.</span><span class="sxs-lookup"><span data-stu-id="25f7c-125">Without at least one of these permissions, the `source` will remain encrypted.</span></span>

## <a name="http-request"></a><span data-ttu-id="25f7c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25f7c-126">HTTP request</span></span>
<!-- {"blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /communications/calls/{id}/answer
```
> <span data-ttu-id="25f7c-127">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="25f7c-127">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="25f7c-128">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="25f7c-128">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25f7c-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25f7c-129">Request headers</span></span>
| <span data-ttu-id="25f7c-130">Имя</span><span class="sxs-lookup"><span data-stu-id="25f7c-130">Name</span></span>          | <span data-ttu-id="25f7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25f7c-131">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="25f7c-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25f7c-132">Authorization</span></span> | <span data-ttu-id="25f7c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25f7c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25f7c-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25f7c-135">Content-type</span></span>  | <span data-ttu-id="25f7c-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25f7c-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25f7c-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25f7c-138">Request body</span></span>
<span data-ttu-id="25f7c-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="25f7c-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="25f7c-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="25f7c-140">Parameter</span></span>        | <span data-ttu-id="25f7c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="25f7c-141">Type</span></span>                                     |<span data-ttu-id="25f7c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="25f7c-142">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="25f7c-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="25f7c-143">callbackUri</span></span>       |<span data-ttu-id="25f7c-144">String</span><span class="sxs-lookup"><span data-stu-id="25f7c-144">String</span></span>                                    |<span data-ttu-id="25f7c-145">Позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления в дальнейшем.</span><span class="sxs-lookup"><span data-stu-id="25f7c-145">Allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="25f7c-146">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="25f7c-146">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="25f7c-147">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="25f7c-147">This must be `https`.</span></span>    |
|<span data-ttu-id="25f7c-148">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="25f7c-148">acceptedModalities</span></span>|<span data-ttu-id="25f7c-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="25f7c-149">String collection</span></span>                         |<span data-ttu-id="25f7c-150">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="25f7c-150">The list of accept modalities.</span></span> <span data-ttu-id="25f7c-151">Возможные значения: `audio` , `video` , `videoBasedScreenSharing` .</span><span class="sxs-lookup"><span data-stu-id="25f7c-151">Possible value are: `audio`, `video`, `videoBasedScreenSharing`.</span></span> <span data-ttu-id="25f7c-152">Необходимо для ответа на вызов.</span><span class="sxs-lookup"><span data-stu-id="25f7c-152">Required for answering a call.</span></span> |
|<span data-ttu-id="25f7c-153">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="25f7c-153">mediaConfig</span></span>       | <span data-ttu-id="25f7c-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) или [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span><span class="sxs-lookup"><span data-stu-id="25f7c-154">[appHostedMediaConfig](../resources/apphostedmediaconfig.md) or [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md)</span></span> |<span data-ttu-id="25f7c-155">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="25f7c-155">The media configuration.</span></span> <span data-ttu-id="25f7c-156">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="25f7c-156">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="25f7c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f7c-157">Response</span></span>
<span data-ttu-id="25f7c-158">Этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="25f7c-158">This method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25f7c-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="25f7c-159">Examples</span></span>
<span data-ttu-id="25f7c-160">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="25f7c-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="25f7c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="25f7c-161">Request</span></span>
<span data-ttu-id="25f7c-162">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25f7c-162">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25f7c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="25f7c-163">HTTP</span></span>](#tab/http)
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
<span data-ttu-id="25f7c-164">Этот большой двоичный объект является сериализованной конфигурацией для сеансов мультимедиа, которая создается из пакета SDK для Media.</span><span class="sxs-lookup"><span data-stu-id="25f7c-164">This blob is the serialized configuration for media sessions which is generated from the media SDK.</span></span>

# <a name="c"></a>[<span data-ttu-id="25f7c-165">C#</span><span class="sxs-lookup"><span data-stu-id="25f7c-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25f7c-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25f7c-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25f7c-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25f7c-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25f7c-168">Java</span><span class="sxs-lookup"><span data-stu-id="25f7c-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25f7c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f7c-169">Response</span></span>
<span data-ttu-id="25f7c-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25f7c-170">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-1-answer-a-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="25f7c-171">Пример 1: ответ одноранговый звонок VoIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="25f7c-171">Example 1: Answer a Peer-to-Peer VoIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="25f7c-172">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="25f7c-172">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="25f7c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="25f7c-173">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="25f7c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f7c-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="25f7c-175">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="25f7c-175">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="25f7c-176">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="25f7c-176">Notification - established</span></span>

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

### <a name="example-2-answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="25f7c-177">Пример 2: ответ на звонок VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="25f7c-177">Example 2: Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="25f7c-178">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="25f7c-178">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="25f7c-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="25f7c-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25f7c-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="25f7c-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="25f7c-181">C#</span><span class="sxs-lookup"><span data-stu-id="25f7c-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25f7c-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25f7c-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25f7c-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25f7c-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25f7c-184">Java</span><span class="sxs-lookup"><span data-stu-id="25f7c-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-answer-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="25f7c-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f7c-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="25f7c-186">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="25f7c-186">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="25f7c-187">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="25f7c-187">Notification - established</span></span>

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

### <a name="example-3-answer-a-policy-based-recording-call"></a><span data-ttu-id="25f7c-188">Пример 3: ответ на вызов записи на основе политики</span><span class="sxs-lookup"><span data-stu-id="25f7c-188">Example 3: Answer a policy-based recording call</span></span>

<span data-ttu-id="25f7c-189">В [сценарии записи на основе политик](/microsoftteams/teams-recording-policy), прежде чем участник политики присоединяется к вызову, на Bot, связанном с политикой, будет отправлено уведомление о входящем звонке.</span><span class="sxs-lookup"><span data-stu-id="25f7c-189">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under policy joins a call, an incoming call notification will be sent to the bot associated with the policy.</span></span>
<span data-ttu-id="25f7c-190">Сведения о присоединении можно найти в свойстве **ботдата** .</span><span class="sxs-lookup"><span data-stu-id="25f7c-190">The join information can be found under the **botData** property.</span></span> <span data-ttu-id="25f7c-191">С помощью Bot можно выбрать ответ на вызов и соответствующим образом [Обновить состояние записи](call-updaterecordingstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="25f7c-191">The bot can then choose to answer the call and [update the recording status](call-updaterecordingstatus.md) accordingly.</span></span>

<span data-ttu-id="25f7c-192">Ниже приведен пример уведомления о входящем вызове, которое получит робота в этом случае.</span><span class="sxs-lookup"><span data-stu-id="25f7c-192">The following is an example of the incoming call notification that a bot would recieve in this case.</span></span>

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
