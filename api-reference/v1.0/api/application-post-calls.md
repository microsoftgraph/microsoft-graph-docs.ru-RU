---
title: Создание звонка
description: Создайте новый вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3b2cc1c228c767e99e33ca585c3c0869eff1bd95
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177216"
---
# <a name="create-call"></a><span data-ttu-id="abb37-103">Создание звонка</span><span class="sxs-lookup"><span data-stu-id="abb37-103">Create call</span></span>

<span data-ttu-id="abb37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abb37-105">Создание [вызова](../resources/call.md) позволяет боту создать новый исходяющий одноранговой или групповой звонок или присоединиться к существующему собранию.</span><span class="sxs-lookup"><span data-stu-id="abb37-105">Create [call](../resources/call.md) enables your bot to create a new outgoing peer-to-peer or group call, or join an existing meeting.</span></span> <span data-ttu-id="abb37-106">Вам потребуется зарегистрировать [вызываемого](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) бота и перейти к списку необходимых разрешений, как упоминалось ниже.</span><span class="sxs-lookup"><span data-stu-id="abb37-106">You will need to [register the calling bot](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot) and go through the list of permissions needed as mentioned below.</span></span>

> <span data-ttu-id="abb37-107">**Примечание.** В настоящее время поддерживаются только вызовы VoIP.</span><span class="sxs-lookup"><span data-stu-id="abb37-107">**Note:** Currently, only VoIP calls are supported.</span></span> 

## <a name="permissions"></a><span data-ttu-id="abb37-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abb37-108">Permissions</span></span>

<span data-ttu-id="abb37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="abb37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot#add-microsoft-graph-permissions).</span></span>

| <span data-ttu-id="abb37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abb37-111">Permission type</span></span>                        | <span data-ttu-id="abb37-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abb37-112">Permissions (from least to most privileged)</span></span>                                             |
|:---------------------------------------|:----------------------------------------------------------------------------------------|
| <span data-ttu-id="abb37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abb37-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="abb37-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="abb37-114">Not Supported</span></span>                                                                           |
| <span data-ttu-id="abb37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abb37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abb37-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="abb37-116">Not Supported</span></span>                                                                           |
| <span data-ttu-id="abb37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abb37-117">Application</span></span>                            | <span data-ttu-id="abb37-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate. All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="abb37-118">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All</span></span> |

> <span data-ttu-id="abb37-119">**Примечание.** Для вызова с мультимедиа, на который есть приложение, требуется разрешение Calls.AccessMedia.All в дополнение к одному из разрешений, перечисленных в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="abb37-119">**Note:** For a call with app-hosted media, you need the Calls.AccessMedia.All permission in addition to one of the permissions listed in the table above.</span></span>

## <a name="http-request"></a><span data-ttu-id="abb37-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls
```

## <a name="request-headers"></a><span data-ttu-id="abb37-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abb37-121">Request headers</span></span>
| <span data-ttu-id="abb37-122">Имя</span><span class="sxs-lookup"><span data-stu-id="abb37-122">Name</span></span>          | <span data-ttu-id="abb37-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abb37-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="abb37-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abb37-124">Authorization</span></span> | <span data-ttu-id="abb37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abb37-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="abb37-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="abb37-127">Content-type</span></span>  | <span data-ttu-id="abb37-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abb37-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb37-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="abb37-130">Request body</span></span>
<span data-ttu-id="abb37-131">В теле запроса укажу представление объекта [вызова](../resources/call.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="abb37-131">In the request body, supply a JSON representation of a [call](../resources/call.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="abb37-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-132">Response</span></span>
<span data-ttu-id="abb37-133">В случае успеха этот метод возвращает код отклика и объект `201 Created` [вызова](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abb37-133">If successful, this method returns a `201 Created` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abb37-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="abb37-134">Examples</span></span>

### <a name="example-1-create-peer-to-peer-voip-call-with-service-hosted-media"></a><span data-ttu-id="abb37-135">Пример 1. Создание одноранговых вызовов VoIP с помощью мультимедиа, на который есть служба</span><span class="sxs-lookup"><span data-stu-id="abb37-135">Example 1: Create peer-to-peer VoIP call with service hosted media</span></span>

> <span data-ttu-id="abb37-136">**Примечание.** Для этого вызова требуется Calls.Iniплитки. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="abb37-136">**Note:** This call needs the Calls.Initiate.All permission.</span></span>

##### <a name="request"></a><span data-ttu-id="abb37-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-137">Request</span></span>
<span data-ttu-id="abb37-138">В следующем примере показан запрос, который совершает одноранговой звонок между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="abb37-138">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="abb37-139">В этом примере мультимедиа находится в службе.</span><span class="sxs-lookup"><span data-stu-id="abb37-139">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="abb37-140">Чтобы пример работал, значения маркера авторизации, URL-адреса, ИД приложения, имени приложения, ИД пользователя, имени пользователя и ИД клиента необходимо заменить фактическими значениями.</span><span class="sxs-lookup"><span data-stu-id="abb37-140">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="abb37-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="abb37-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
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
# <a name="javascript"></a>[<span data-ttu-id="abb37-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abb37-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-service-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="abb37-143">C#</span><span class="sxs-lookup"><span data-stu-id="abb37-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-service-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abb37-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abb37-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-service-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abb37-145">Java</span><span class="sxs-lookup"><span data-stu-id="abb37-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-service-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abb37-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-146">Response</span></span>

> <span data-ttu-id="abb37-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abb37-147">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

##### <a name="notification---establishing"></a><span data-ttu-id="abb37-148">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="abb37-148">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="abb37-149">Уведомление установлено</span><span class="sxs-lookup"><span data-stu-id="abb37-149">Notification - established</span></span>

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

### <a name="example-2-create-peer-to-peer-voip-call-with-application-hosted-media"></a><span data-ttu-id="abb37-150">Пример 2. Создание одноранговых вызовов VoIP с помощью мультимедиа, на который есть приложение</span><span class="sxs-lookup"><span data-stu-id="abb37-150">Example 2: Create peer-to-peer VoIP call with application hosted media</span></span>

> <span data-ttu-id="abb37-151">**Примечание.** В этом примере Calls.Iniплитки. Разрешения All и Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="abb37-151">**Note**: This example needs Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

##### <a name="request"></a><span data-ttu-id="abb37-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-152">Request</span></span>
<span data-ttu-id="abb37-153">В следующем примере показан запрос, который совершает одноранговой звонок между ботом и указанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="abb37-153">The following example shows the request which makes a peer-to-peer call between the bot and the specified user.</span></span> <span data-ttu-id="abb37-154">В этом примере мультимедиа локально находится в приложении.</span><span class="sxs-lookup"><span data-stu-id="abb37-154">In this example the media is hosted locally by the application.</span></span> <span data-ttu-id="abb37-155">Чтобы пример работал, значения маркера авторизации, URL-адреса, ид приложения, имени приложения, ид пользователя, имени пользователя и клиента должны быть заменены фактическими значениями.</span><span class="sxs-lookup"><span data-stu-id="abb37-155">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced with actual values to make the example work.</span></span>


# <a name="http"></a>[<span data-ttu-id="abb37-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="abb37-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="abb37-157">C#</span><span class="sxs-lookup"><span data-stu-id="abb37-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-call-app-hosted-media-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abb37-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abb37-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-call-app-hosted-media-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abb37-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abb37-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-call-app-hosted-media-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abb37-160">Java</span><span class="sxs-lookup"><span data-stu-id="abb37-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-call-app-hosted-media-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="abb37-161">**Примечание.** Для одноранговых вызовов ожидаемые уведомления только об изменениях состояния вызовов.</span><span class="sxs-lookup"><span data-stu-id="abb37-161">**Note:** For peer-to-peer calls, the expected notifications are for call state changes only.</span></span>

##### <a name="response"></a><span data-ttu-id="abb37-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-162">Response</span></span>

> <span data-ttu-id="abb37-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abb37-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-call-with-service-hosted-media"></a><span data-ttu-id="abb37-165">Пример 3. Создание группового вызова с мультимедиа, на который есть служба</span><span class="sxs-lookup"><span data-stu-id="abb37-165">Example 3: Create a group call with service hosted media</span></span>

<span data-ttu-id="abb37-166">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="abb37-166">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="abb37-167">В примере показано, как создать групповой звонок с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="abb37-167">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="abb37-168">**Примечание.** В этом примере вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="abb37-168">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="abb37-169">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="abb37-169">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="abb37-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-170">Request</span></span>

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

### <a name="example-4-create-a-group-call-with-application-hosted-media"></a><span data-ttu-id="abb37-171">Пример 4. Создание группового вызова с помощью мультимедиа, на который есть приложение</span><span class="sxs-lookup"><span data-stu-id="abb37-171">Example 4: Create a group call with application hosted media</span></span>

<span data-ttu-id="abb37-172">Это поддерживает до 5 пользователей VoIP.</span><span class="sxs-lookup"><span data-stu-id="abb37-172">This supports up to 5 VoIP users.</span></span> <span data-ttu-id="abb37-173">В примере показано, как создать групповой звонок с двумя пользователями VoIP.</span><span class="sxs-lookup"><span data-stu-id="abb37-173">The example shows how to create a group call with two VoIP users.</span></span>
> <span data-ttu-id="abb37-174">**Примечание.** В этом примере вызова требуется `Calls.InitiateGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="abb37-174">**Note:** This example call needs the `Calls.InitiateGroupCalls.All` permission.</span></span> <span data-ttu-id="abb37-175">Созданный групповой вызов не поддерживает чат или запись.</span><span class="sxs-lookup"><span data-stu-id="abb37-175">The group call created doesn't support chat or recording.</span></span>

##### <a name="request"></a><span data-ttu-id="abb37-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-176">Request</span></span>

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

### <a name="example-5-join-scheduled-meeting-with-service-hosted-media"></a><span data-ttu-id="abb37-177">Пример 5. Присоединитесь к запланированному собранию с помощью мультимедиа, наемного в службе</span><span class="sxs-lookup"><span data-stu-id="abb37-177">Example 5: Join scheduled meeting with service hosted media</span></span>
<span data-ttu-id="abb37-178">Чтобы присоединиться к запланированному собранию, необходимо получить ид потока, ид сообщения, ид организатора и ид клиента, в котором запланировано собрание.</span><span class="sxs-lookup"><span data-stu-id="abb37-178">To join the scheduled meeting we will need to get the thread id, message id, organizer id and the tenant id in which the meeting is scheduled.</span></span>
<span data-ttu-id="abb37-179">Эти сведения можно получить из [API Get Online Meetings](../api/onlinemeeting-get.md) (только для собраний на основе VTC).</span><span class="sxs-lookup"><span data-stu-id="abb37-179">This information can be obtained from the [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only).</span></span>

<span data-ttu-id="abb37-180">Значения маркера авторизации, URL-адреса, ид приложения, имя приложения, ид пользователя, имя пользователя и ид клиента должны быть заменены на сведения, полученные из  [API Get Online Meetings](../api/onlinemeeting-get.md) (только на основе VTC) фактическими значениями, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="abb37-180">The values of authorization token, callback url, application id, application name, user id, user name and tenant id must be replaced along with the details obtained from  [Get Online Meetings API](../api/onlinemeeting-get.md) (VTC-based meetings only) with actual values to make the example work.</span></span>
> <span data-ttu-id="abb37-181">**Примечание.** В этом примере требуется `Calls.JoinGroupCalls.All` разрешение.</span><span class="sxs-lookup"><span data-stu-id="abb37-181">**Note:** This example needs the `Calls.JoinGroupCalls.All` permission.</span></span>

##### <a name="request"></a><span data-ttu-id="abb37-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-182">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="abb37-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-183">Response</span></span>

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

##### <a name="notification---establishing"></a><span data-ttu-id="abb37-184">Уведомление — создание</span><span class="sxs-lookup"><span data-stu-id="abb37-184">Notification - establishing</span></span>

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
##### <a name="notification---established"></a><span data-ttu-id="abb37-185">Уведомление установлено</span><span class="sxs-lookup"><span data-stu-id="abb37-185">Notification - established</span></span>

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
##### <a name="notification---roster"></a><span data-ttu-id="abb37-186">Уведомление — список</span><span class="sxs-lookup"><span data-stu-id="abb37-186">Notification - roster</span></span>

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

><span data-ttu-id="abb37-187">**Примечание.** Для сценариев присоединиться к собранию отдельно от уведомлений о состоянии звонка мы получаем уведомления о составе.</span><span class="sxs-lookup"><span data-stu-id="abb37-187">**Note:** For join meeting scenarios apart from call state notifications, we receive roster notifications.</span></span>

### <a name="example-6-join-scheduled-meeting-with-application-hosted-media"></a><span data-ttu-id="abb37-188">Пример 6. Присоединяйтесь к запланированному собранию с помощью мультимедиа, в которое было перенесено приложение</span><span class="sxs-lookup"><span data-stu-id="abb37-188">Example 6: Join scheduled meeting with application hosted media</span></span>
<span data-ttu-id="abb37-189">Обновите media config с [помощью AppHostedMediaConfig,](../resources/apphostedmediaconfig.md) как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="abb37-189">Update the media config with the [AppHostedMediaConfig](../resources/apphostedmediaconfig.md) as shown below.</span></span>

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

### <a name="example-7-create-peer-to-peer-pstn-call-with-service-hosted-media"></a><span data-ttu-id="abb37-190">Пример 7. Создание одноранговых вызовов PSTN с помощью мультимедиа, ведаемого службой</span><span class="sxs-lookup"><span data-stu-id="abb37-190">Example 7: Create peer-to-peer PSTN call with service hosted media</span></span>

> <span data-ttu-id="abb37-191">**Примечание.** Для этого вызова требуется Calls.Iniплитки. Все разрешения.</span><span class="sxs-lookup"><span data-stu-id="abb37-191">**Note:** This call requires the Calls.Initiate.All permission.</span></span>

<span data-ttu-id="abb37-192">Для этого вызова требуется экземпляр приложения с назначенным номером STN.</span><span class="sxs-lookup"><span data-stu-id="abb37-192">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="abb37-193">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="abb37-193">Step 1: Create application instance</span></span>
<span data-ttu-id="abb37-194">Используя учетные данные администратора клиента, вызовите следующие cmdlets в удаленной powerShell клиента, чтобы создать экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="abb37-194">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="abb37-195">Дополнительные сведения см. в командах [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="abb37-195">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="abb37-196">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="abb37-196">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="abb37-197">Используйте учетные данные администратора клиента для входа и перейдите на вкладку https://admin.microsoft.com/ **"Пользователи > активные пользователи".**</span><span class="sxs-lookup"><span data-stu-id="abb37-197">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="abb37-198">Выберите экземпляр приложения, назначьте план внутренних и международных звонков **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите кнопку **"Сохранить изменения".**</span><span class="sxs-lookup"><span data-stu-id="abb37-198">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="abb37-199">Если необходимые лицензии недоступны в клиенте, их можно получить на вкладке "Выставление счета **-> Приобретение служб".**</span><span class="sxs-lookup"><span data-stu-id="abb37-199">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="abb37-200">Шаг 3. Получение номера STN</span><span class="sxs-lookup"><span data-stu-id="abb37-200">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="abb37-201">Используйте учетные данные администратора клиента, чтобы войти в учетную панель и щелкнуть вкладку "Устаревший https://admin.teams.microsoft.com/ **портал"** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="abb37-201">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="abb37-202">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="abb37-202">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="abb37-203">Нажмите **+** кнопку, выберите **"Новые номера служб"** и перейдите на страницу **"Добавление новых номеров служб".**</span><span class="sxs-lookup"><span data-stu-id="abb37-203">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="abb37-204">Выберите **"Страна/регион",** **"Область",** **"Город",**"Количество **входных** данных" и нажмите **кнопку "Добавить"** для поиска.</span><span class="sxs-lookup"><span data-stu-id="abb37-204">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="abb37-205">Щелкните **"Получить номера".**</span><span class="sxs-lookup"><span data-stu-id="abb37-205">Click **acquire numbers**.</span></span> <span data-ttu-id="abb37-206">Недавно полученный номер будет показываться на **вкладке "Номера** телефонов".</span><span class="sxs-lookup"><span data-stu-id="abb37-206">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="abb37-207">Шаг 4. Назначение номера STN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="abb37-207">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="abb37-208">С помощью учетных данных администратора клиента вызовите следующие cmdlets в удаленной powerShell клиента, чтобы назначить номер STN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="abb37-208">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="abb37-209">Дополнительные сведения см. в командах [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="abb37-209">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="abb37-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-210">Request</span></span>
<span data-ttu-id="abb37-211">В следующем примере показан запрос на одноранговую связь между ботом и номером STN.</span><span class="sxs-lookup"><span data-stu-id="abb37-211">The following example shows the request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="abb37-212">В этом примере мультимедиа находится в службе.</span><span class="sxs-lookup"><span data-stu-id="abb37-212">In this example, the media is hosted by the service.</span></span> <span data-ttu-id="abb37-213">Чтобы пример работал, значения маркера авторизации, URL-адреса, ИД приложения, имени приложения, ИД пользователя, имени пользователя и ИД клиента необходимо заменить фактическими значениями.</span><span class="sxs-lookup"><span data-stu-id="abb37-213">The values of authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID must be replaced with actual values to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
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

#### <a name="response"></a><span data-ttu-id="abb37-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-214">Response</span></span>

> <span data-ttu-id="abb37-215">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abb37-215">**Note:** The response object shown here might be shortened for readability.</span></span> 

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

### <a name="example-8-create-peer-to-peer-pstn-call-with-application-hosted-media"></a><span data-ttu-id="abb37-216">Пример 8. Создание одноранговых вызовов PSTN с помощью мультимедиа, на который есть приложение</span><span class="sxs-lookup"><span data-stu-id="abb37-216">Example 8: Create peer-to-peer PSTN call with application hosted media</span></span>

> <span data-ttu-id="abb37-217">**Примечание.** В этом примере Calls.Iniплитки. Разрешения All и Calls.AccessMedia.All.</span><span class="sxs-lookup"><span data-stu-id="abb37-217">**Note**: This example requires Calls.Initiate.All and Calls.AccessMedia.All permissions.</span></span>

<span data-ttu-id="abb37-218">Для этого вызова требуется экземпляр приложения с назначенным номером STN, как описано в примере 7.</span><span class="sxs-lookup"><span data-stu-id="abb37-218">This call needs application instance with PSTN number assigned, as described in Example 7.</span></span>

#### <a name="request"></a><span data-ttu-id="abb37-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb37-219">Request</span></span>
<span data-ttu-id="abb37-220">В следующем примере показан запрос на одноранговую связь между ботом и номером STN.</span><span class="sxs-lookup"><span data-stu-id="abb37-220">The following example shows a request to make a peer-to-peer call between the bot and a PSTN number.</span></span> <span data-ttu-id="abb37-221">В этом примере мультимедиа локально находится в приложении.</span><span class="sxs-lookup"><span data-stu-id="abb37-221">In this example, the media is hosted locally by the application.</span></span> <span data-ttu-id="abb37-222">Замените значения маркера авторизации, URL-адреса вызова, ИД приложения, имени приложения, ИД пользователя, имени пользователя и ИД клиента, чтобы пример работал.</span><span class="sxs-lookup"><span data-stu-id="abb37-222">Replace the values for authorization token, callback URL, application ID, application name, user ID, user name, and tenant ID to make the example work.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-call-service-hosted-media",
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

#### <a name="response"></a><span data-ttu-id="abb37-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb37-223">Response</span></span>

> <span data-ttu-id="abb37-224">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abb37-224">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
