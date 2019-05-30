---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ce79ff0e471882576ed885e4ab85d686a6cdb0de
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536059"
---
# <a name="call-answer"></a><span data-ttu-id="58f4a-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="58f4a-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58f4a-104">Ответ на входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="58f4a-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="58f4a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58f4a-105">Permissions</span></span>
<span data-ttu-id="58f4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58f4a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58f4a-108">Permission type</span></span> | <span data-ttu-id="58f4a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58f4a-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="58f4a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58f4a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="58f4a-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58f4a-111">Not Supported</span></span>                        |
| <span data-ttu-id="58f4a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58f4a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58f4a-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="58f4a-113">Not Supported</span></span>                        |
| <span data-ttu-id="58f4a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58f4a-114">Application</span></span>     | <span data-ttu-id="58f4a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="58f4a-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="58f4a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58f4a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="58f4a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58f4a-117">Request headers</span></span>
| <span data-ttu-id="58f4a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="58f4a-118">Name</span></span>          | <span data-ttu-id="58f4a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="58f4a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="58f4a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58f4a-120">Authorization</span></span> | <span data-ttu-id="58f4a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58f4a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58f4a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58f4a-123">Request body</span></span>
<span data-ttu-id="58f4a-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="58f4a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58f4a-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="58f4a-125">Parameter</span></span>        | <span data-ttu-id="58f4a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="58f4a-126">Type</span></span>                                     |<span data-ttu-id="58f4a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="58f4a-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="58f4a-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="58f4a-128">callbackUri</span></span>       |<span data-ttu-id="58f4a-129">String</span><span class="sxs-lookup"><span data-stu-id="58f4a-129">String</span></span>                                    |<span data-ttu-id="58f4a-130">Идентификатор обратного вызова или подписки, для которой будут предоставляться обратные вызовы.</span><span class="sxs-lookup"><span data-stu-id="58f4a-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="58f4a-131">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="58f4a-131">(Required)</span></span>                                                               |
|<span data-ttu-id="58f4a-132">Акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="58f4a-132">acceptedModalities</span></span>|<span data-ttu-id="58f4a-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58f4a-133">String collection</span></span>                         |<span data-ttu-id="58f4a-134">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="58f4a-134">The list of accept modalities.</span></span> <span data-ttu-id="58f4a-135">Возможные `unknown`значения:, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="58f4a-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="58f4a-136">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="58f4a-136">(Required)</span></span> |
|<span data-ttu-id="58f4a-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="58f4a-137">mediaConfig</span></span>       |[<span data-ttu-id="58f4a-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="58f4a-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="58f4a-139">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="58f4a-139">The media configuration.</span></span> <span data-ttu-id="58f4a-140">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="58f4a-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="58f4a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f4a-141">Response</span></span>
<span data-ttu-id="58f4a-142">Этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="58f4a-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="58f4a-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="58f4a-143">Examples</span></span>
<span data-ttu-id="58f4a-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="58f4a-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="58f4a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="58f4a-145">Request</span></span>
<span data-ttu-id="58f4a-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58f4a-146">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-answer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/answer
Content-Type: application/json
Content-Length: 211

{
  "callbackUri": "callbackUri-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "acceptedModalities": [
    "audio"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="58f4a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f4a-147">Response</span></span>
<span data-ttu-id="58f4a-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58f4a-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="58f4a-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="58f4a-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="58f4a-150">C#</span><span class="sxs-lookup"><span data-stu-id="58f4a-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-answer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58f4a-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="58f4a-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-answer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="58f4a-152">Отвечать на звонки по VOIP с размещенными на службах носителями</span><span class="sxs-lookup"><span data-stu-id="58f4a-152">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="58f4a-153">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="58f4a-153">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
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

##### <a name="request"></a><span data-ttu-id="58f4a-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="58f4a-154">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
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

##### <a name="response"></a><span data-ttu-id="58f4a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f4a-155">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="58f4a-156">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="58f4a-156">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="58f4a-157">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="58f4a-157">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "established"
      }
    }
  ]
}
```

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="58f4a-158">Ответ на звонок VOIP с размещенными на сервере приложениями</span><span class="sxs-lookup"><span data-stu-id="58f4a-158">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="58f4a-159">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="58f4a-159">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
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

##### <a name="request"></a><span data-ttu-id="58f4a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="58f4a-160">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/answer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "ignored",
  "name": "call-answer"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "acceptedModalities": [ "audio" ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  }
}
```

##### <a name="response"></a><span data-ttu-id="58f4a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f4a-161">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="58f4a-162">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="58f4a-162">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "establishing"
      }
    }
  ]
}
```

##### <a name="notification---established"></a><span data-ttu-id="58f4a-163">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="58f4a-163">Notification - established</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
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
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-answer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
