---
title: 'Вызовите: ответ'
description: Ответ на входящий звонок.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 98d3f54e87e36de6c8f492644be1b47486b48d39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879536"
---
# <a name="call-answer"></a><span data-ttu-id="eb7b8-103">Вызовите: ответ</span><span class="sxs-lookup"><span data-stu-id="eb7b8-103">call: answer</span></span>

> <span data-ttu-id="eb7b8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb7b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb7b8-106">Ответ на входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-106">Answer an incoming call.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb7b8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb7b8-107">Permissions</span></span>
<span data-ttu-id="eb7b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb7b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb7b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb7b8-110">Permission type</span></span> | <span data-ttu-id="eb7b8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-111">Permissions (from least to most privileged)</span></span>                 |
| :-------------- | :-----------------------------------------------------------|
| <span data-ttu-id="eb7b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb7b8-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eb7b8-113">Not Supported</span></span>                        |
| <span data-ttu-id="eb7b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb7b8-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eb7b8-115">Not Supported</span></span>                        |
| <span data-ttu-id="eb7b8-116">Application</span><span class="sxs-lookup"><span data-stu-id="eb7b8-116">Application</span></span>     | <span data-ttu-id="eb7b8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="eb7b8-117">None</span></span>                                                        |

## <a name="http-request"></a><span data-ttu-id="eb7b8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb7b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/answer
POST /applications/{id}/calls/{id}/answer
```

## <a name="request-headers"></a><span data-ttu-id="eb7b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb7b8-119">Request headers</span></span>
| <span data-ttu-id="eb7b8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eb7b8-120">Name</span></span>          | <span data-ttu-id="eb7b8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eb7b8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="eb7b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb7b8-122">Authorization</span></span> | <span data-ttu-id="eb7b8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb7b8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb7b8-125">Request body</span></span>
<span data-ttu-id="eb7b8-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb7b8-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="eb7b8-127">Parameter</span></span>        | <span data-ttu-id="eb7b8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eb7b8-128">Type</span></span>                                     |<span data-ttu-id="eb7b8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="eb7b8-129">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="eb7b8-130">callbackUri</span><span class="sxs-lookup"><span data-stu-id="eb7b8-130">callbackUri</span></span>       |<span data-ttu-id="eb7b8-131">Строка</span><span class="sxs-lookup"><span data-stu-id="eb7b8-131">String</span></span>                                    |<span data-ttu-id="eb7b8-132">Идентификатор обратного вызова или подписки, на котором будет доставлено обратных вызовов.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-132">The callback or subscription ID on which callbacks will be delivered.</span></span> <span data-ttu-id="eb7b8-133">(Обязательно)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-133">(Required)</span></span>                                                               |
|<span data-ttu-id="eb7b8-134">acceptedModalities</span><span class="sxs-lookup"><span data-stu-id="eb7b8-134">acceptedModalities</span></span>|<span data-ttu-id="eb7b8-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eb7b8-135">String collection</span></span>                         |<span data-ttu-id="eb7b8-136">Список принимать модальности.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-136">The list of accept modalities.</span></span> <span data-ttu-id="eb7b8-137">Приведены возможные значения: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-137">Possible value are: `unknown`, `audio`, `video`, `screenSharing`, `videoBasedScreenSharing`, `data`.</span></span> <span data-ttu-id="eb7b8-138">(Обязательно)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-138">(Required)</span></span> |
|<span data-ttu-id="eb7b8-139">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="eb7b8-139">mediaConfig</span></span>       |[<span data-ttu-id="eb7b8-140">mediaConfig</span><span class="sxs-lookup"><span data-stu-id="eb7b8-140">mediaConfig</span></span>](../resources/mediaconfig.md)|<span data-ttu-id="eb7b8-141">Конфигурация мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-141">The media configuration.</span></span> <span data-ttu-id="eb7b8-142">(Обязательно)</span><span class="sxs-lookup"><span data-stu-id="eb7b8-142">(Required)</span></span>                                                                                                            |

## <a name="response"></a><span data-ttu-id="eb7b8-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb7b8-143">Response</span></span>
<span data-ttu-id="eb7b8-144">Этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-144">This method returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eb7b8-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb7b8-145">Examples</span></span>
<span data-ttu-id="eb7b8-146">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-146">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="eb7b8-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb7b8-147">Request</span></span>
<span data-ttu-id="eb7b8-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-148">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="eb7b8-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb7b8-149">Response</span></span>
<span data-ttu-id="eb7b8-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb7b8-150">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="answer-voip-call-with-service-hosted-media"></a><span data-ttu-id="eb7b8-151">VOIP ответить на звонок с помощью службы, размещенной мультимедиа</span><span class="sxs-lookup"><span data-stu-id="eb7b8-151">Answer VOIP call with service hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="eb7b8-152">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="eb7b8-152">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="eb7b8-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb7b8-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="eb7b8-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb7b8-154">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="eb7b8-155">Уведомления - Установка</span><span class="sxs-lookup"><span data-stu-id="eb7b8-155">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="eb7b8-156">Уведомления - соединения</span><span class="sxs-lookup"><span data-stu-id="eb7b8-156">Notification - established</span></span>

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

### <a name="answer-voip-call-with-application-hosted-media"></a><span data-ttu-id="eb7b8-157">Отвечать на звонок по протоколу VOIP с приложение, размещенное мультимедиа</span><span class="sxs-lookup"><span data-stu-id="eb7b8-157">Answer VOIP call with application hosted media</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="eb7b8-158">Уведомления - входящие</span><span class="sxs-lookup"><span data-stu-id="eb7b8-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="eb7b8-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb7b8-159">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="eb7b8-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb7b8-160">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---establishing"></a><span data-ttu-id="eb7b8-161">Уведомления - Установка</span><span class="sxs-lookup"><span data-stu-id="eb7b8-161">Notification - establishing</span></span>

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

##### <a name="notification---established"></a><span data-ttu-id="eb7b8-162">Уведомления - соединения</span><span class="sxs-lookup"><span data-stu-id="eb7b8-162">Notification - established</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: answer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
