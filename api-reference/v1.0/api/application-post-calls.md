---
title: Создание звонка
description: Создайте новый вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 34c4b2396d936a869108ca44372df8a1f7adbe5e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054646"
---
# <a name="create-call"></a><span data-ttu-id="061e2-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="061e2-103">Create call</span></span>

<span data-ttu-id="061e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="061e2-105">Создание [вызова](../resources/call.md) позволяет боту создать новый исходяющий одноранговой или групповой вызов или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="061e2-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="061e2-106">Вам потребуется [зарегистрировать вызываемого бота](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) и пройти список разрешений, необходимых, как упоминалось ниже.</span><span class="sxs-lookup"><span data-stu-id="061e2-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="061e2-107">**Примечание:** В настоящее время поддерживаются только вызовы VoIP.</span><span class="sxs-lookup"><span data-stu-id="061e2-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="061e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="061e2-108">Permissions</span></span>

<span data-ttu-id="061e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="061e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="061e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="061e2-111">Permission type</span></span>                        | <span data-ttu-id="061e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="061e2-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="061e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="061e2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="061e2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="061e2-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="061e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="061e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="061e2-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="061e2-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="061e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="061e2-117">Application</span></span>                            | <span data-ttu-id="061e2-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate. Все, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="061e2-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="061e2-119">**Примечание:** Для вызова с помощью носители, на которые есть приложения, требуется разрешение Calls.AccessMedia.All в дополнение к одному из разрешений, перечисленных в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="061e2-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed in the table above.</span></span>

## <a name="http-request"></a><span data-ttu-id="061e2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls
```

## <a name="request-headers"></a><span data-ttu-id="061e2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="061e2-121">Request headers</span></span>
| <span data-ttu-id="061e2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="061e2-122">Name</span></span>          | <span data-ttu-id="061e2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="061e2-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="061e2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="061e2-124">Authorization</span></span> | <span data-ttu-id="061e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="061e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="061e2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="061e2-127">Content-type</span></span>  | <span data-ttu-id="061e2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="061e2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="061e2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="061e2-130">Request body</span></span>
<span data-ttu-id="061e2-131">В теле запроса поставляем JSON-представление объекта [вызова.](../resources/call.md)</span><span class="sxs-lookup"><span data-stu-id="061e2-131">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="061e2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-132">Response</span></span>
<span data-ttu-id="061e2-133">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [вызова](../resources/call.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="061e2-133">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="061e2-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="061e2-134">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="061e2-135">Пример 1. Создание одноранговых вызовов VoIP с помощью средств массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="061e2-135">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="061e2-136">**Примечание:** Этот вызов требует Calls.Initiate. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="061e2-136">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="061e2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-137">Request</span></span>
<span data-ttu-id="061e2-138">В следующем примере показан запрос, который делает одноранговой вызов между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="061e2-138">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="061e2-139">В этом примере носители хозяйской службы.</span><span class="sxs-lookup"><span data-stu-id="061e2-139">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="061e2-140">Значения маркера авторизации, URL-адреса, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="061e2-140">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="061e2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media-1",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="061e2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061e2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="061e2-143">C#</span><span class="sxs-lookup"><span data-stu-id="061e2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="061e2-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="061e2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="061e2-145">Java</span><span class="sxs-lookup"><span data-stu-id="061e2-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="061e2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-146">Response</span></span>

> <span data-ttu-id="061e2-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="061e2-147">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "endpointType": null,
      "replacesCallId": null,
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="061e2-148">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="061e2-148">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "id": "2e1a0b00-2db4-4022-9570-243709c565ab"
      }
    }
  ]
}
```
##### <a name="notification---established"></a><span data-ttu-id="061e2-149">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="061e2-149">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "direction": "outgoing",
        "id": "2e1a0b00-b3c5-4b0f-99b3-c133bc1e6116"
      }
    }
  ]
}
```

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="061e2-150">Пример 2. Создание одноранговых вызовов VoIP с помощью средств массовой информации приложения</span><span class="sxs-lookup"><span data-stu-id="061e2-150">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="061e2-151">**Примечание.** В этом примере Calls.Initiate. Все разрешения и разрешения Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="061e2-151">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="061e2-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-152">Request</span></span>
<span data-ttu-id="061e2-153">В следующем примере показан запрос, который делает одноранговой вызов между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="061e2-153">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="061e2-154">В этом примере средства массовой информации локализованы приложением.</span><span class="sxs-lookup"><span data-stu-id="061e2-154">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="061e2-155">Значения маркера авторизации, URL-адреса вызова, id приложения, имени приложения, пользовательского именем пользователя и id клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="061e2-155">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="061e2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
 "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="061e2-157">C#</span><span class="sxs-lookup"><span data-stu-id="061e2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061e2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061e2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="061e2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="061e2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="061e2-160">Java</span><span class="sxs-lookup"><span data-stu-id="061e2-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="061e2-161">**Примечание:** Для одноранговых вызовов ожидаемые уведомления только для изменения состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="061e2-161">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="061e2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-162">Response</span></span>

> <span data-ttu-id="061e2-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="061e2-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="061e2-164">Пример 3. Создание группового вызова с помощью средства массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="061e2-164">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="061e2-165">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="061e2-165">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="061e2-166">В примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="061e2-166">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="061e2-167">**Примечание:** В этом примере вызову требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="061e2-167">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="061e2-168">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="061e2-168">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="061e2-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-169">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with service hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "removeFromDefaultAudioGroup": false
  }
}
```

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="061e2-170">Пример 4. Создание группового вызова с помощью средства массовой информации с хостингом приложения</span><span class="sxs-lookup"><span data-stu-id="061e2-170">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="061e2-171">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="061e2-171">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="061e2-172">В примере показано, как создать групповой вызов с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="061e2-172">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="061e2-173">**Примечание:** В этом примере вызову требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="061e2-173">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="061e2-174">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="061e2-174">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="061e2-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-175">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "create-group-call-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "subject": "Create a group call with application hosted media",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "TestBot",
        "id": "dd3885da-f9ab-486b-bfae-85de3d445555"
      }
    }
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user1",
          "id": "98da8a1a-1b87-452c-a713-65d3f10b5555"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "user2",
          "id": "bf5aae9a-d11d-47a8-93b1-782504c95555"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "removeFromDefaultAudioGroup": false
  }
}
```

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="061e2-176">Пример 5. Присоединиться к запланированной встрече с средствами массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="061e2-176">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="061e2-177">Чтобы присоединиться к запланированному собранию, нам необходимо получить потоковый id, id сообщения, id организатора и id клиента, в котором планируется собрание.</span><span class="sxs-lookup"><span data-stu-id="061e2-177">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="061e2-178">Эти сведения можно получить из [API Get Online Meetings](../api/onlinemeeting-get.md) (только на основе VTC).</span><span class="sxs-lookup"><span data-stu-id="061e2-178">This information can be obtained from the [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only).</span></span>

<span data-ttu-id="061e2-179">Значения маркера авторизации, URL-адреса вызовов, id приложения, имени приложения, пользовательского именем пользователя и ид клиента должны быть заменены на сведения, полученные из API Get  [Online Meetings](../api/onlinemeeting-get.md) (только на основе VTC) с фактическими значениями для работы в примере.</span><span class="sxs-lookup"><span data-stu-id="061e2-179">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only) with actual values to make the example work.</span></span>
> <span data-ttu-id="061e2-180">**Примечание:** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="061e2-180">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="061e2-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-181">Request</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-service-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "displayName": "Bob",
        "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
      }
    },
    "allowConversationWithoutHost": true
  },
  "tenantId":"86dc81db-c112-4228-9222-63f3esaa1edb"
}
```
##### <a name="response"></a><span data-ttu-id="061e2-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-182">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": null,
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "toneInfo": null
}
```

##### <a name="notification---establishing"></a><span data-ttu-id="061e2-183">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="061e2-183">Notification - establishing</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
        "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "establishing",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}

```
##### <a name="notification---established"></a><span data-ttu-id="061e2-184">Уведомление — установлено</span><span class="sxs-lookup"><span data-stu-id="061e2-184">Notification - established</span></span>

```http
POST https://bot.contoso.com/callback
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
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "chatInfo": {
          "@odata.type": "#microsoft.graph.chatInfo",
          "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
          "messageId": "0"
        },
        "meetingInfo": {
          "@odata.type": "#microsoft.graph.organizerMeetingInfo",
          "organizer": {
            "@odata.type": "#microsoft.graph.identitySet",
            "user": {
              "@odata.type": "#microsoft.graph.identity",
              "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
              "displayName": "Bob"
            }
          },
          "allowConversationWithoutHost": true
        },
        "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92"
      }
    }
  ]
}
```
##### <a name="notification---roster"></a><span data-ttu-id="061e2-185">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="061e2-185">Notification - roster</span></span>

```http
POST https://bot.contoso.com/callback
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92/participants",
      "callbackUri": "https://bot.contoso.com/callback",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "John",
                "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
              }
            },
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "video",
              "sourceId": "2",
              "direction": "receiveOnly",
              "serverMuted": false
            },
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "videoBasedScreenSharing",
              "sourceId": "8",
              "direction": "receiveOnly",
              "serverMuted": false
            }
          ],
          "isMuted": true,
          "isInLobby": false,
          "id": "0d7664b6-6432-43ed-8d27-d9e7adec188c"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            }
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "10",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": "05491616-385f-44a8-9974-18cc5f9933c1"
        }
      ]
    }
  ]
}
```

><span data-ttu-id="061e2-186">**Примечание:** Для сценариев присоединиться к собраниям, кроме уведомлений состояния вызовов, мы получаем уведомления реестра.</span><span class="sxs-lookup"><span data-stu-id="061e2-186">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-application-hosted-media"></a><span data-ttu-id="061e2-187">Пример 6. Регистрация запланированной встречи с носители приложения</span><span class="sxs-lookup"><span data-stu-id="061e2-187">Example 6: Join scheduled meeting with application hosted media</span></span>
<span data-ttu-id="061e2-188">Обнови медиафайл [с помощью AppHostedMediaConfig,](../resources/apphostedmediaconfig.md) как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="061e2-188">Update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below.</span></span>

<!-- {
  "blockType": "example",
  "name": "join-scheduled-meeting-app-hosted-media",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "displayName": "Bob"
      }
    },
    "allowConversationWithoutHost": true
  }
}
```

### <a name="example-7-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="061e2-189">Пример 7. Создание одноранговых вызовов PSTN с помощью средства массовой информации службы</span><span class="sxs-lookup"><span data-stu-id="061e2-189">Example 7: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="061e2-190">**Примечание:** Этот вызов требует Calls.Initiate. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="061e2-190">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="061e2-191">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="061e2-191">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="061e2-192">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="061e2-192">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="061e2-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-193">Request</span></span>
<span data-ttu-id="061e2-194">В следующем примере показан запрос на одноранговой вызов между ботом и номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="061e2-194">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="061e2-195">В этом примере носители хозяйской службы.</span><span class="sxs-lookup"><span data-stu-id="061e2-195">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="061e2-196">Значения маркера авторизации, URL-адреса, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента должны быть заменены фактическими значениями, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="061e2-196">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="061e2-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media-2",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="061e2-198">C#</span><span class="sxs-lookup"><span data-stu-id="061e2-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061e2-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061e2-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="061e2-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-200">Response</span></span>

> <span data-ttu-id="061e2-201">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="061e2-201">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

### <a name="example-8-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="061e2-202">Пример 8. Создание одноранговых вызовов PSTN с помощью средств массовой информации, на которые было организовано приложение.</span><span class="sxs-lookup"><span data-stu-id="061e2-202">Example 8: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="061e2-203">**Примечание.** В этом примере Calls.Initiate. Все разрешения и разрешения Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="061e2-203">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="061e2-204">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="061e2-204">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="061e2-205">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="061e2-205">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="061e2-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="061e2-206">Request</span></span>
<span data-ttu-id="061e2-207">В следующем примере показан запрос на одноранговой вызов между ботом и номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="061e2-207">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="061e2-208">В этом примере средства массовой информации локализованы приложением.</span><span class="sxs-lookup"><span data-stu-id="061e2-208">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="061e2-209">Замените значения маркера авторизации, URL-адреса вызова, ID приложения, имени приложения, пользовательского ИД, имени пользователя и ИД клиента, чтобы сделать пример работой.</span><span class="sxs-lookup"><span data-stu-id="061e2-209">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="061e2-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media-3",
  "@odata.type": "microsoft.graph.call"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "callbackUri": "https://bot.contoso.com/callback",
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="061e2-211">C#</span><span class="sxs-lookup"><span data-stu-id="061e2-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061e2-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061e2-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="061e2-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="061e2-213">Response</span></span>

> <span data-ttu-id="061e2-214">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="061e2-214">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "establishing",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callChainId": "d8217646-3110-40b1-bae6-e9ac6c3a9f74",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "applicationInstance": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    "countryCode": null,
    "endpointType": null,
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      },
      "endpointType": null,
      "region": null,
      "replacesCallId": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<Media Session Configuration>",
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "mediaState": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "meetingCapability": null,
  "toneInfo": null
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
