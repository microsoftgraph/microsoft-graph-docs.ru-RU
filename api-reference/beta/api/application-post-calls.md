---
title: Создание вызова
description: Создайте новый звонок.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 1a2c6e85579e82787abf0bb7bb8b541c81aaf12e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818741"
---
# <a name="create-call"></a><span data-ttu-id="468a2-103">Создание вызова</span><span class="sxs-lookup"><span data-stu-id="468a2-103">Create call</span></span>

> <span data-ttu-id="468a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="468a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="468a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="468a2-106">Создайте новый звонок.</span><span class="sxs-lookup"><span data-stu-id="468a2-106">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="468a2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="468a2-107">Permissions</span></span>
<span data-ttu-id="468a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="468a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="468a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="468a2-110">Permission type</span></span>                        | <span data-ttu-id="468a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="468a2-111">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="468a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="468a2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="468a2-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="468a2-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="468a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="468a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="468a2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="468a2-115">Not Supported</span></span>                                                                           |
| <span data-ttu-id="468a2-116">Application</span><span class="sxs-lookup"><span data-stu-id="468a2-116">Application</span></span>                            | <span data-ttu-id="468a2-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="468a2-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="468a2-118">**Примечание:** Для вызова с приложение, размещенное мультимедиа необходимо иметь разрешение Calls.AccessMedia.All с одним из разрешения, перечисленные в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="468a2-118">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="468a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="468a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="468a2-120">Request headers</span></span>
| <span data-ttu-id="468a2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="468a2-121">Name</span></span>          | <span data-ttu-id="468a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="468a2-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="468a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="468a2-123">Authorization</span></span> | <span data-ttu-id="468a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="468a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="468a2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="468a2-126">Request body</span></span>
<span data-ttu-id="468a2-127">В тексте запроса укажите представление JSON объекта [вызова](../resources/call.md) .</span><span class="sxs-lookup"><span data-stu-id="468a2-127">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="468a2-128">**Примечание:** Свойства помечены как `Server generated` игнорируются при обработке `POST` на `app/calls`.</span><span class="sxs-lookup"><span data-stu-id="468a2-128">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="468a2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="468a2-129">Response</span></span>
<span data-ttu-id="468a2-130">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [call](../resources/call.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="468a2-130">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="468a2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="468a2-131">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="468a2-132">Создание одноранговые звонок по протоколу VOIP с помощью службы, размещенной мультимедиа</span><span class="sxs-lookup"><span data-stu-id="468a2-132">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="468a2-133">**Примечание:** Этот вызов необходимо иметь права Calls.Initiate.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-133">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-134">Request</span></span>
<span data-ttu-id="468a2-135">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="468a2-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json

{
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="response"></a><span data-ttu-id="468a2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="468a2-136">Response</span></span>

> <span data-ttu-id="468a2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="468a2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json


{
  "id": "57DAB8B1894C409AB240BD8BEAE78896",
  "callbackUri": "https://bot.contoso.com/api/calls",
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
  },
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="468a2-139">Уведомления - Установка</span><span class="sxs-lookup"><span data-stu-id="468a2-139">Notification - establishing</span></span>

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
        "state": "establishing",
        "direction": "outgoing"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="468a2-140">Уведомления - соединения</span><span class="sxs-lookup"><span data-stu-id="468a2-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="468a2-141">Создание одноранговые звонок по протоколу VOIP с приложение, размещенное мультимедиа</span><span class="sxs-lookup"><span data-stu-id="468a2-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="468a2-142">Примечание: Требуется разрешение Calls.Initiate.All и Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-143">Request</span></span>
<span data-ttu-id="468a2-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="468a2-144">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "https://bot.contoso.com/api/calls",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "requestedModalities": [ "audio" ],
  "source": {
    "identity": {
      "application": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "IT Bot"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "subject": "Test Call",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      }
    }
  ],
  "tenantId": "tenantId-value"
}
```

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="468a2-145">Создание группы вызова с помощью службы, размещенной мультимедиа</span><span class="sxs-lookup"><span data-stu-id="468a2-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="468a2-146">**Примечание:** В этом примере должно разрешения Calls.InitiateGroupCalls.All и Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-147">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "targets": [
    {
      "identity": {
        "user": {
          "id": "29362BD4-CD58-4ED0-A206-0E4A33DBB0B6",
          "displayName": "Heidi Steen"
        }
      }
    },
    {
      "identity": {
        "phone": {
          "displayName": "+12345678890",
          "id": "+12345678890"
        }
      }
    }
  ],
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  }
}
```

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="468a2-148">Закрытый присоединиться к собранию с помощью службы, размещенной мультимедиа</span><span class="sxs-lookup"><span data-stu-id="468a2-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="468a2-149">**Примечание:** В этом примере требуется разрешение Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-150">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="468a2-151">Присоединение к собранию канала с помощью службы, размещенной мультимедиа</span><span class="sxs-lookup"><span data-stu-id="468a2-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="468a2-152">**Примечание:** В этом примере требуется разрешение Calls.JoinGroupCalls.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-153">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "application": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="468a2-154">Присоединение к собранию канала в качестве гостя с мультимедиа службы, размещенной</span><span class="sxs-lookup"><span data-stu-id="468a2-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="468a2-155">**Примечание:** В этом примере требуется разрешение Calls.JoinGroupCallsAsGuest.All.</span><span class="sxs-lookup"><span data-stu-id="468a2-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="468a2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="468a2-156">Request</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "subject": "Test Call",
  "callbackUri": "https://bot.contoso.com/api/calls",
  "source": {
    "identity": {
      "user": {
        "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698",
        "displayName": "App_Guest_DisplayName",
        "identityProvider": "None"
      }
    }
  },
  "requestedModalities": [ "audio", "video" ],
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
  },
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "1507228578052",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
        "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
      }
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
