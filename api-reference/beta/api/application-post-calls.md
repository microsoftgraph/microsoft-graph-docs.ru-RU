---
title: Создание звонка
description: Создание нового звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b645180c3f90f0d282aa70282ac362c8365e3f02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945468"
---
# <a name="create-call"></a><span data-ttu-id="c88ab-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="c88ab-103">Create call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88ab-104">Создание нового звонка.</span><span class="sxs-lookup"><span data-stu-id="c88ab-104">Create a new call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c88ab-105">Permissions</span></span>
<span data-ttu-id="c88ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c88ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c88ab-108">Permission type</span></span>                        | <span data-ttu-id="c88ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c88ab-109">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="c88ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c88ab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c88ab-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c88ab-111">Not Supported</span></span>                                                                           |
| <span data-ttu-id="c88ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c88ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88ab-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c88ab-113">Not Supported</span></span>                                                                           |
| <span data-ttu-id="c88ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c88ab-114">Application</span></span>                            | <span data-ttu-id="c88ab-115">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls. initiate. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="c88ab-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="c88ab-116">**Примечание:** Для вызова с размещенными в приложении носителями требуется разрешение Calls. Акцессмедиа. ALL с одним из разрешений, перечисленных в предыдущей таблице.</span><span class="sxs-lookup"><span data-stu-id="c88ab-116">**Note:** For a call with app hosted media, you need the Calls.AccessMedia.All permission with one of the permissions listed in the previous table.</span></span>

## <a name="http-request"></a><span data-ttu-id="c88ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls
POST /applications/{id}/calls
```

## <a name="request-headers"></a><span data-ttu-id="c88ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c88ab-118">Request headers</span></span>
| <span data-ttu-id="c88ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c88ab-119">Name</span></span>          | <span data-ttu-id="c88ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c88ab-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c88ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c88ab-121">Authorization</span></span> | <span data-ttu-id="c88ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c88ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88ab-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c88ab-124">Request body</span></span>
<span data-ttu-id="c88ab-125">В тексте запроса добавьте представление объекта [Call](../resources/call.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c88ab-125">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

> <span data-ttu-id="c88ab-126">**Примечание:** Свойства, отмеченные как `Server generated` , игнорируются при обработке. `POST` `app/calls`</span><span class="sxs-lookup"><span data-stu-id="c88ab-126">**Note:** Properties marked as `Server generated` are ignored when processing `POST` on `app/calls`.</span></span>

## <a name="response"></a><span data-ttu-id="c88ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c88ab-127">Response</span></span>
<span data-ttu-id="c88ab-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c88ab-128">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c88ab-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c88ab-129">Examples</span></span>

### <a name="create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="c88ab-130">Создание однорангового вызова VOIP с размещенными в службе носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-130">Create peer to peer VOIP call with service hosted media</span></span>

> <span data-ttu-id="c88ab-131">**Примечание:** Для этого вызова требуется разрешение Calls. initiate. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-131">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-132">Request</span></span>
<span data-ttu-id="c88ab-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c88ab-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c88ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c88ab-134">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c88ab-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c88ab-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c88ab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c88ab-136">Response</span></span>

> <span data-ttu-id="c88ab-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c88ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="c88ab-139">Установка уведомления</span><span class="sxs-lookup"><span data-stu-id="c88ab-139">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="c88ab-140">Установленное уведомление</span><span class="sxs-lookup"><span data-stu-id="c88ab-140">Notification - established</span></span>

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

### <a name="create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="c88ab-141">Создание однорангового вызова VOIP с размещенными в приложении носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-141">Create peer to peer VOIP call with application hosted media</span></span>

> <span data-ttu-id="c88ab-142">Note: требуются вызовы. initiate. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-142">Note: Needs Calls.Initiate.All and Calls.AccessMedia.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-143">Request</span></span>
<span data-ttu-id="c88ab-144">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c88ab-144">The following example shows the request.</span></span>

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

### <a name="create-group-call-with-service-hosted-media"></a><span data-ttu-id="c88ab-145">Создание группового звонка с размещенными у службы носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-145">Create group call with service hosted media</span></span>

> <span data-ttu-id="c88ab-146">**Примечание:** В этом примере требуются разрешения Calls. Инитиатеграупкаллс. ALL и Calls. Акцессмедиа. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-146">**Note:** This example needs the Calls.InitiateGroupCalls.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-147">Request</span></span>

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

### <a name="join-private-meeting-with-service-hosted-media"></a><span data-ttu-id="c88ab-148">Присоединение к частному собранию с размещенными на службы носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-148">Join private meeting with service hosted media</span></span>

> <span data-ttu-id="c88ab-149">**Примечание:** В этом примере требуется разрешение Calls. Жоинграупкаллс. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-149">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-150">Request</span></span>

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

### <a name="join-channel-meeting-with-service-hosted-media"></a><span data-ttu-id="c88ab-151">Присоединение к собранию канала с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-151">Join channel meeting with service hosted media</span></span>

> <span data-ttu-id="c88ab-152">**Примечание:** В этом примере требуется разрешение Calls. Жоинграупкаллс. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-152">**Note:** This example needs the Calls.JoinGroupCalls.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-153">Request</span></span>

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

### <a name="join-channel-meeting-as-a-guest-with-service-hosted-media"></a><span data-ttu-id="c88ab-154">Присоединение к собранию канала в качестве гостя с размещенными в службах носителями</span><span class="sxs-lookup"><span data-stu-id="c88ab-154">Join channel meeting as a guest with service hosted media</span></span>

> <span data-ttu-id="c88ab-155">**Примечание:** В этом примере требуется разрешение Calls. Жоинграупкаллсасгуест. ALL.</span><span class="sxs-lookup"><span data-stu-id="c88ab-155">**Note:** This example needs the Calls.JoinGroupCallsAsGuest.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="c88ab-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88ab-156">Request</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
