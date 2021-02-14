---
title: 'participant: invite'
description: Приглашение участников в активный вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d4702e7257a5c49a8ef1232391dc923589bd2808
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177104"
---
# <a name="participant-invite"></a><span data-ttu-id="ccc65-103">participant: invite</span><span class="sxs-lookup"><span data-stu-id="ccc65-103">participant: invite</span></span>

<span data-ttu-id="ccc65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccc65-105">Приглашение участников в активный вызов.</span><span class="sxs-lookup"><span data-stu-id="ccc65-105">Invite participants to the active call.</span></span>

<span data-ttu-id="ccc65-106">Дополнительные сведения о том, как обрабатывать операции, см. в [подстроке commsoperation.](../resources/commsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ccc65-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="ccc65-107">**Примечание.** Этот API поддерживается только для групповых вызовов.</span><span class="sxs-lookup"><span data-stu-id="ccc65-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc65-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc65-108">Permissions</span></span>
<span data-ttu-id="ccc65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccc65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccc65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccc65-111">Permission type</span></span> | <span data-ttu-id="ccc65-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccc65-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="ccc65-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccc65-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccc65-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ccc65-114">Not supported</span></span>                       |
| <span data-ttu-id="ccc65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccc65-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccc65-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ccc65-116">Not supported</span></span>                       |
| <span data-ttu-id="ccc65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccc65-117">Application</span></span>     | <span data-ttu-id="ccc65-118">Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="ccc65-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="ccc65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccc65-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/invite
```

## <a name="request-headers"></a><span data-ttu-id="ccc65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccc65-120">Request headers</span></span>
| <span data-ttu-id="ccc65-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ccc65-121">Name</span></span>          | <span data-ttu-id="ccc65-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc65-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ccc65-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccc65-123">Authorization</span></span> | <span data-ttu-id="ccc65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc65-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccc65-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccc65-126">Content-type</span></span>  | <span data-ttu-id="ccc65-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccc65-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc65-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccc65-129">Request body</span></span>
<span data-ttu-id="ccc65-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ccc65-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccc65-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ccc65-131">Parameter</span></span>      | <span data-ttu-id="ccc65-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ccc65-132">Type</span></span>    |<span data-ttu-id="ccc65-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc65-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccc65-134">participants</span><span class="sxs-lookup"><span data-stu-id="ccc65-134">participants</span></span>|<span data-ttu-id="ccc65-135">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ccc65-135">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="ccc65-136">Приглашенные участники.</span><span class="sxs-lookup"><span data-stu-id="ccc65-136">The participants to be invited.</span></span>|
|<span data-ttu-id="ccc65-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="ccc65-137">clientContext</span></span>|<span data-ttu-id="ccc65-138">String</span><span class="sxs-lookup"><span data-stu-id="ccc65-138">String</span></span>|<span data-ttu-id="ccc65-139">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="ccc65-139">Unique Client Context string.</span></span> <span data-ttu-id="ccc65-140">Максимальное ограничение — 256 chars.</span><span class="sxs-lookup"><span data-stu-id="ccc65-140">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="ccc65-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc65-141">Response</span></span>
<span data-ttu-id="ccc65-142">Если это не так, этот метод возвращает код отклика и заглавную ссылку с URI для `200 OK` [метода inviteParticipantsOperation,](../resources/inviteparticipantsoperation.md) созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="ccc65-142">If succsessful, this method returns a `200 OK` response code and a location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> 

<span data-ttu-id="ccc65-143">Тело ответа содержит созданный [inviteParticipantsOperation.](../resources/inviteparticipantsoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ccc65-143">The body of the response contains the created [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).</span></span>

><span data-ttu-id="ccc65-144">**Примечание.** Когда этот API возвращает успешный ответ, все участники получат обновление для участников.</span><span class="sxs-lookup"><span data-stu-id="ccc65-144">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="ccc65-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="ccc65-145">Examples</span></span>
<span data-ttu-id="ccc65-146">В следующих примерах покажите, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="ccc65-146">The following examples show how to call this API.</span></span>

> <span data-ttu-id="ccc65-147">**Примечание.** Объекты ответа могут быть сокращены для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="ccc65-147">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="ccc65-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccc65-148">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="ccc65-149">Пример 1. Приглашение одного участника к существующему групповому вызову</span><span class="sxs-lookup"><span data-stu-id="ccc65-149">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="ccc65-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc65-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccc65-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc65-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="ccc65-152">C#</span><span class="sxs-lookup"><span data-stu-id="ccc65-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccc65-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc65-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccc65-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc65-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccc65-155">Java</span><span class="sxs-lookup"><span data-stu-id="ccc65-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccc65-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc65-156">Response</span></span>

> <span data-ttu-id="ccc65-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccc65-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "displayName": "string"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="ccc65-159">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="ccc65-159">Notification - operation completed</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "displayName": "string"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="ccc65-160">Уведомление — список, обновленный с помощью добавленного участника</span><span class="sxs-lookup"><span data-stu-id="ccc65-160">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="ccc65-161">Пример 2. Приглашение нескольких участников к существующему групповому вызову</span><span class="sxs-lookup"><span data-stu-id="ccc65-161">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="ccc65-162">**Примечание.** Существующий групповой звонок должен иметь допустимый [chatInfo.](../resources/chatInfo.md)</span><span class="sxs-lookup"><span data-stu-id="ccc65-162">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="ccc65-163">Поддерживается приглашение до 5 участников.</span><span class="sxs-lookup"><span data-stu-id="ccc65-163">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="ccc65-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc65-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ccc65-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc65-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-multiple"
}-->

```http
POST /communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "string"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "1e126418-44a0-4a94-a6f8-0efe1ad71acb",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="ccc65-166">C#</span><span class="sxs-lookup"><span data-stu-id="ccc65-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccc65-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc65-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccc65-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc65-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccc65-169">Java</span><span class="sxs-lookup"><span data-stu-id="ccc65-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-multiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccc65-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc65-170">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
   "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e",
   "status":"Running",
   "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
   "resultInfo":null,
   "participants":[
      {
         "endpointType":null,
         "replacesCallId":null,
         "identity":{
            "user":{
              "@odata.type": "#microsoft.graph.identity",
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "@odata.type": "#microsoft.graph.identity",
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "displayName": "string"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
##### <a name="notification---operation-completed"></a><span data-ttu-id="ccc65-171">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="ccc65-171">Notification - operation completed</span></span>
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```
<!-- {
  "blockType": "example",
  "truncated": "true",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": {
        "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
        "participants": [
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "displayName": "string"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
              }
            }
          }
        ],
        "status": "completed",
        "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
        "id": null
      }
    }
  ]
}

```
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="ccc65-172">Уведомление — список, обновленный с добавленными участниками</span><span class="sxs-lookup"><span data-stu-id="ccc65-172">Notification - roster updated with participants added</span></span>
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
      "resource": "/app/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceUrl": "/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/operations/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe"
              }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
                "mediaType": "audio",
              "sourceId": "1",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "info": {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "@odata.type": "#microsoft.graph.identity",
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "displayName": "string"
             }
            },
            "endpointType": "default"
          },
          "mediaStreams": [
            {
              "@odata.type": "#microsoft.graph.mediaStream",
              "mediaType": "audio",
              "sourceId": "3",
              "direction": "sendReceive",
              "serverMuted": false
            }
          ],
          "isMuted": false,
          "isInLobby": false,
          "id": null
        }
      ]
    }
  ]
}


```

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="ccc65-173">Пример 3. Приглашение участников к существующему групповому вызову, заменив существующий одноранговой вызов</span><span class="sxs-lookup"><span data-stu-id="ccc65-173">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="ccc65-174">API приглашений поддерживает только одного участника при замене существующего одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="ccc65-174">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="ccc65-175">Если в тексте запроса есть несколько участников, будет прочитан только первый участник, а остальные участники будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="ccc65-175">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="ccc65-176">**Примечание.** API приглашений поддерживает только одного участника, `replacesCallId` если он предоставлен.</span><span class="sxs-lookup"><span data-stu-id="ccc65-176">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="ccc65-177">Дополнительные сведения об использовании замены существующего однорангового вызова см. в `replacesCallId` приглашенииParticipantInfo. [](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="ccc65-177">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="ccc65-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc65-178">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccc65-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc65-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite-existing"
}-->

```http
POST /communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite
Content-Type: application/json

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "string"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="ccc65-180">C#</span><span class="sxs-lookup"><span data-stu-id="ccc65-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccc65-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc65-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccc65-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc65-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccc65-183">Java</span><span class="sxs-lookup"><span data-stu-id="ccc65-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-invite-existing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccc65-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc65-184">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "278405a3-f568-4b3e-b684-009193463064",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="ccc65-185">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="ccc65-185">Notification - operation completed</span></span>

``` http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->

```json
{ 
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/278405a3-f568-4b3e-b684-009193463064",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "displayName": "string"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"278405a3-f568-4b3e-b684-009193463064"
         }
      }
   ]
}
```

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="ccc65-186">Уведомление — список, обновленный с помощью добавленного участника</span><span class="sxs-lookup"><span data-stu-id="ccc65-186">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceUrl":"/communications/calls/a7ebfb2d-871e-419c-87af-27290b22e8db/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "displayName": "string"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}
```

><span data-ttu-id="ccc65-187">**Примечание.** С состоянием "завершено" можно ожидать получения уведомлений о том, как ваш исходный одноранговой звонок был завершен и удален.</span><span class="sxs-lookup"><span data-stu-id="ccc65-187">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

### <a name="example-4-invite-one-pstn-participant-to-an-existing-group-call"></a><span data-ttu-id="ccc65-188">Пример 4. Приглашение одного участника PSTN к существующему групповому вызову</span><span class="sxs-lookup"><span data-stu-id="ccc65-188">Example 4: Invite one PSTN participant to an existing group call</span></span>

<span data-ttu-id="ccc65-189">Для этого вызова требуется экземпляр приложения с назначенным номером STN.</span><span class="sxs-lookup"><span data-stu-id="ccc65-189">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="ccc65-190">Шаг 1. Создание экземпляра приложения</span><span class="sxs-lookup"><span data-stu-id="ccc65-190">Step 1: Create application instance</span></span>
<span data-ttu-id="ccc65-191">Используя учетные данные администратора клиента, вызовите следующие cmdlets в удаленной powerShell клиента, чтобы создать экземпляр приложения.</span><span class="sxs-lookup"><span data-stu-id="ccc65-191">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="ccc65-192">Дополнительные сведения см. в командах [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ccc65-192">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="ccc65-193">Шаг 2. Назначение лицензий Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ccc65-193">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="ccc65-194">Используйте учетные данные администратора клиента для входа и перейдите на вкладку https://admin.microsoft.com/ **"Пользователи > активные пользователи".**</span><span class="sxs-lookup"><span data-stu-id="ccc65-194">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="ccc65-195">Выберите экземпляр приложения, назначьте план внутренних и международных звонков **Microsoft 365** и телефонную систему **Microsoft 365 —** лицензии виртуальных пользователей и нажмите кнопку **"Сохранить изменения".**</span><span class="sxs-lookup"><span data-stu-id="ccc65-195">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="ccc65-196">Если необходимые лицензии недоступны в клиенте, их можно получить на вкладке "Выставление счета **-> Приобретение служб".**</span><span class="sxs-lookup"><span data-stu-id="ccc65-196">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="ccc65-197">Шаг 3. Получение номера STN</span><span class="sxs-lookup"><span data-stu-id="ccc65-197">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="ccc65-198">Используйте учетные данные администратора клиента, чтобы войти в учетную панель и щелкнуть вкладку "Устаревший https://admin.teams.microsoft.com/ **портал"** на левой панели.</span><span class="sxs-lookup"><span data-stu-id="ccc65-198">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="ccc65-199">На новой странице перейдите на вкладку **голосовых > номеров** телефонов.</span><span class="sxs-lookup"><span data-stu-id="ccc65-199">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="ccc65-200">Нажмите **+** кнопку, выберите **"Новые номера служб"** и перейдите на страницу **"Добавление новых номеров служб".**</span><span class="sxs-lookup"><span data-stu-id="ccc65-200">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="ccc65-201">Выберите **"Страна/регион",** **"Область",** **"Город",**"Количество **входных** данных" и нажмите **кнопку "Добавить"** для поиска.</span><span class="sxs-lookup"><span data-stu-id="ccc65-201">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="ccc65-202">Щелкните **"Получить номера".**</span><span class="sxs-lookup"><span data-stu-id="ccc65-202">Click **acquire numbers**.</span></span> <span data-ttu-id="ccc65-203">Недавно полученный номер будет показываться на **вкладке "Номера** телефонов".</span><span class="sxs-lookup"><span data-stu-id="ccc65-203">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="ccc65-204">Шаг 4. Назначение номера STN экземпляру приложения</span><span class="sxs-lookup"><span data-stu-id="ccc65-204">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="ccc65-205">С помощью учетных данных администратора клиента вызовите следующие cmdlets в удаленной powerShell клиента, чтобы назначить номер STN экземпляру приложения.</span><span class="sxs-lookup"><span data-stu-id="ccc65-205">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="ccc65-206">Дополнительные сведения см. в командах [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) и [Sync-CsOnlineApplicationInstance.](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ccc65-206">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="ccc65-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccc65-207">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST /communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
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
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```

#### <a name="response"></a><span data-ttu-id="ccc65-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccc65-208">Response</span></span>

> <span data-ttu-id="ccc65-p114">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccc65-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": null,
      "identity": {
        "user": null,
        "guest": null,
        "encrypted": null,
        "onPremises": null,
        "applicationInstance": null,
        "application": null,
        "device": null,
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
      }
    }
  ]
}
```

#### <a name="notification---operation-completed"></a><span data-ttu-id="ccc65-211">Уведомление — операция завершена</span><span class="sxs-lookup"><span data-stu-id="ccc65-211">Notification - operation completed</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[ 
      { 
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"deleted",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/operations/eec3812a-fdc3-4fb4-825c-a06c9f35414e",
         "resourceData":{ 
            "@odata.type":"#microsoft.graph.inviteParticipantsOperation",
            "participants":[ 
               { 
                  "@odata.type":"#microsoft.graph.invitationParticipantInfo",
                  "identity":{ 
                     "@odata.type":"#microsoft.graph.identitySet",
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
                     }
                  }
               }
            ],
            "status":"completed",
            "clientContext":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         }
      }
   ]
}
```

#### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="ccc65-212">Уведомление — список, обновленный с помощью добавленного участника</span><span class="sxs-lookup"><span data-stu-id="ccc65-212">Notification - roster updated with participant added</span></span>

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
   "@odata.type":"#microsoft.graph.commsNotifications",
   "value":[
      {
         "@odata.type":"#microsoft.graph.commsNotification",
         "changeType":"updated",
         "resource":"/app/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceUrl":"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants",
         "resourceData":[
            {
               "@odata.type":"#microsoft.graph.participant",
               "info":{
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "phone": {
                        "@odata.type": "#microsoft.graph.identity",
                        "id": "+12345678901"
                     }
                  },
                  "endpointType":"default"
               },
               "mediaStreams":[
                  {
                     "@odata.type":"#microsoft.graph.mediaStream",
                     "mediaType":"audio",
                     "sourceId":"1",
                     "direction":"sendReceive",
                     "serverMuted":false
                  }
               ],
               "isMuted":false,
               "isInLobby":false,
               "id":null
            }
         ]
      }
   ]
}

```

><span data-ttu-id="ccc65-213">**Примечание.** С состоянием можно ожидать получения уведомлений о том, как ваш исходный одноранговой звонок `completed` был завершен и удален.</span><span class="sxs-lookup"><span data-stu-id="ccc65-213">**Note:** With a `completed` status, you can expect to receive notifications about how your original peer-to-peer call has been terminated and deleted.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

