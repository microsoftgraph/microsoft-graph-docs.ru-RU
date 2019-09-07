---
title: 'вызов: ответ'
description: Ответ на входящий вызов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8cbdd87e037bb22972394423203f0f9218edf7b2
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792431"
---
# <a name="call-answer"></a><span data-ttu-id="3ec10-103">вызов: ответ</span><span class="sxs-lookup"><span data-stu-id="3ec10-103">call: answer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec10-104">Ответ на входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="3ec10-104">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec10-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec10-105">Permissions</span></span>
<span data-ttu-id="3ec10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ec10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ec10-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ec10-108">Permission type</span></span> | <span data-ttu-id="3ec10-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ec10-109">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="3ec10-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ec10-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ec10-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ec10-111">Not Supported</span></span>                        |
| <span data-ttu-id="3ec10-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ec10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec10-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ec10-113">Not Supported</span></span>                        |
| <span data-ttu-id="3ec10-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ec10-114">Application</span></span>     | <span data-ttu-id="3ec10-115">Нет</span><span class="sxs-lookup"><span data-stu-id="3ec10-115">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="3ec10-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ec10-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="3ec10-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ec10-117">Request headers</span></span>
| <span data-ttu-id="3ec10-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3ec10-118">Name</span></span>          | <span data-ttu-id="3ec10-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec10-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3ec10-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ec10-120">Authorization</span></span> | <span data-ttu-id="3ec10-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ec10-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec10-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ec10-123">Request body</span></span>
<span data-ttu-id="3ec10-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3ec10-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ec10-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="3ec10-125">Parameter</span></span>        | <span data-ttu-id="3ec10-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3ec10-126">Type</span></span>                                     |<span data-ttu-id="3ec10-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec10-127">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="3ec10-128">callbackUri</span><span class="sxs-lookup"><span data-stu-id="3ec10-128">callbackUri</span></span>       |<span data-ttu-id="3ec10-129">String</span><span class="sxs-lookup"><span data-stu-id="3ec10-129">String</span></span>                                    |<span data-ttu-id="3ec10-130">Идентификатор обратного вызова или подписки, для которой будут предоставляться обратные вызовы.</span><span class="sxs-lookup"><span data-stu-id="3ec10-130">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="3ec10-131">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="3ec10-131">(Required)</span></span>                                                               |
|<span data-ttu-id="3ec10-132">акцептедмодалитиес</span><span class="sxs-lookup"><span data-stu-id="3ec10-132">acceptedModalities</span></span>|<span data-ttu-id="3ec10-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3ec10-133">String collection</span></span>                         |<span data-ttu-id="3ec10-134">Список принимаемых модальности.</span><span class="sxs-lookup"><span data-stu-id="3ec10-134">The list of accept modalities.</span></span> <span data-ttu-id="3ec10-135">Возможные `unknown`значения:, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`,. `data`</span><span class="sxs-lookup"><span data-stu-id="3ec10-135">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="3ec10-136">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="3ec10-136">(Required)</span></span> |
|<span data-ttu-id="3ec10-137">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="3ec10-137">mediaConfig</span></span>       |[<span data-ttu-id="3ec10-138">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="3ec10-138">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="3ec10-139">Настройка мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3ec10-139">The media configuration.</span></span> <span data-ttu-id="3ec10-140">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="3ec10-140">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="3ec10-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec10-141">Response</span></span>
<span data-ttu-id="3ec10-142">Этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec10-142">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3ec10-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ec10-143">Examples</span></span>
<span data-ttu-id="3ec10-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3ec10-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3ec10-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec10-145">Request</span></span>
<span data-ttu-id="3ec10-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ec10-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3ec10-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec10-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ec10-148">C#</span><span class="sxs-lookup"><span data-stu-id="3ec10-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-answer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ec10-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec10-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-answer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ec10-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3ec10-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-answer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ec10-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec10-151">Response</span></span>
<span data-ttu-id="3ec10-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ec10-152">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="3ec10-153">Отвечать на звонки по VOIP с размещенными на службах носителями</span><span class="sxs-lookup"><span data-stu-id="3ec10-153">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="3ec10-154">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="3ec10-154">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="3ec10-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec10-155">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="3ec10-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec10-156">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="3ec10-157">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="3ec10-157">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="3ec10-158">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="3ec10-158">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="3ec10-159">Ответ на звонок VOIP с размещенными на сервере приложениями</span><span class="sxs-lookup"><span data-stu-id="3ec10-159">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="3ec10-160">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="3ec10-160">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="3ec10-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ec10-161">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="3ec10-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ec10-162">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="3ec10-163">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="3ec10-163">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="3ec10-164">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="3ec10-164">Notification - established</span></span>

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
  ]
}
-->
