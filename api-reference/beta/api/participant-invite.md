---
title: 'участник: пригласить'
description: Приглашение участников в активный вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14c30d53dca55ce99f80cc206a6d746322887240
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455993"
---
# <a name="participant-invite"></a><span data-ttu-id="219b0-103">участник: пригласить</span><span class="sxs-lookup"><span data-stu-id="219b0-103">participant: invite</span></span>

<span data-ttu-id="219b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="219b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="219b0-105">Приглашение участников в активный вызов.</span><span class="sxs-lookup"><span data-stu-id="219b0-105">Invite participants to the active call.</span></span>

<span data-ttu-id="219b0-106">Дополнительные сведения об обработке операций можно найти в разделе [коммсоператион](../resources/commsoperation.md).</span><span class="sxs-lookup"><span data-stu-id="219b0-106">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="219b0-107">**Примечание:** Этот API поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="219b0-107">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="219b0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="219b0-108">Permissions</span></span>
<span data-ttu-id="219b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="219b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="219b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="219b0-111">Permission type</span></span> | <span data-ttu-id="219b0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="219b0-112">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="219b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="219b0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="219b0-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="219b0-114">Not supported</span></span>                       |
| <span data-ttu-id="219b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="219b0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="219b0-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="219b0-116">Not supported</span></span>                       |
| <span data-ttu-id="219b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="219b0-117">Application</span></span>     | <span data-ttu-id="219b0-118">Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="219b0-118">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="219b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="219b0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /communications/calls/{id}/participants/invite
```
> <span data-ttu-id="219b0-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="219b0-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="219b0-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="219b0-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="219b0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="219b0-122">Request headers</span></span>
| <span data-ttu-id="219b0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="219b0-123">Name</span></span>          | <span data-ttu-id="219b0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="219b0-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="219b0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="219b0-125">Authorization</span></span> | <span data-ttu-id="219b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="219b0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="219b0-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="219b0-128">Content-type</span></span>  | <span data-ttu-id="219b0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="219b0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="219b0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="219b0-131">Request body</span></span>
<span data-ttu-id="219b0-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="219b0-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="219b0-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="219b0-133">Parameter</span></span>      | <span data-ttu-id="219b0-134">Тип</span><span class="sxs-lookup"><span data-stu-id="219b0-134">Type</span></span>    |<span data-ttu-id="219b0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="219b0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="219b0-136">participants</span><span class="sxs-lookup"><span data-stu-id="219b0-136">participants</span></span>|<span data-ttu-id="219b0-137">Коллекция [invitationParticipantInfo](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="219b0-137">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="219b0-138">Приглашенных участников.</span><span class="sxs-lookup"><span data-stu-id="219b0-138">The participants to be invited.</span></span>|
|<span data-ttu-id="219b0-139">Контекст</span><span class="sxs-lookup"><span data-stu-id="219b0-139">clientContext</span></span>|<span data-ttu-id="219b0-140">String</span><span class="sxs-lookup"><span data-stu-id="219b0-140">String</span></span>|<span data-ttu-id="219b0-141">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="219b0-141">Unique Client Context string.</span></span> <span data-ttu-id="219b0-142">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="219b0-142">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="219b0-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="219b0-143">Response</span></span>
<span data-ttu-id="219b0-144">Если сукксессфул, этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="219b0-144">If succsessful, this method returns a `200 OK` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> <span data-ttu-id="219b0-145">В тексте отклика содержится созданный [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="219b0-145">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

><span data-ttu-id="219b0-146">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="219b0-146">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="219b0-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="219b0-147">Examples</span></span>
<span data-ttu-id="219b0-148">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="219b0-148">The following examples show how to call this API.</span></span>

> <span data-ttu-id="219b0-149">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="219b0-149">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="219b0-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="219b0-150">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="219b0-151">Пример 1: приглашение одного участника на существующий вызов группы</span><span class="sxs-lookup"><span data-stu-id="219b0-151">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="219b0-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="219b0-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="219b0-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="219b0-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-invite"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="219b0-154">C#</span><span class="sxs-lookup"><span data-stu-id="219b0-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="219b0-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="219b0-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="219b0-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="219b0-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="219b0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="219b0-157">Response</span></span>

> <span data-ttu-id="219b0-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="219b0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="219b0-160">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="219b0-160">Notification - operation completed</span></span>

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
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="219b0-161">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="219b0-161">Notification - roster updated with participant added</span></span>

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
                     "application":{
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"278405a3-f568-4b3e-b684-009193463064",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="219b0-162">Пример 2: Приглашение нескольких участников в существующий вызов групп</span><span class="sxs-lookup"><span data-stu-id="219b0-162">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="219b0-163">**Note**: существующий вызов группы должен иметь допустимый [чатинфо](../resources/chatInfo.md).</span><span class="sxs-lookup"><span data-stu-id="219b0-163">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="219b0-164">В приглашении поддерживается до 5 участников.</span><span class="sxs-lookup"><span data-stu-id="219b0-164">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="219b0-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="219b0-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="219b0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="219b0-166">HTTP</span></span>](#tab/http)
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
          "identityProvider": "AAD"
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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="219b0-167">C#</span><span class="sxs-lookup"><span data-stu-id="219b0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="219b0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="219b0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="219b0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="219b0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="219b0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="219b0-170">Response</span></span>

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
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      },
      {
         "endpointType":null,
         "id":null,
         "replacesCallId":null,
         "identity":{
            "user":{
               "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
               "identityProvider":"AAD",
               "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
            "application":null,
            "device":null,
            "phone":null
         }
      }
   ]
}

```
##### <a name="notification---operation-completed"></a><span data-ttu-id="219b0-171">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="219b0-171">Notification - operation completed</span></span>
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
                "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
              }
            }
          },
          {
            "@odata.type": "#microsoft.graph.invitationParticipantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="219b0-172">Уведомление — список, обновленный при добавлении участников</span><span class="sxs-lookup"><span data-stu-id="219b0-172">Notification - roster updated with participants added</span></span>
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
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "application": {
                "@odata.type": "#microsoft.graph.identity",
                "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
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
            "@odata.type": "#microsoft.graph.participantInfo",
            "identity": {
              "@odata.type": "#microsoft.graph.identitySet",
              "user":{
                "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
                "identityProvider":"AAD",
                "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="219b0-173">Пример 3: приглашение участников в существующий групповой вызов с заменой существующего однорангового вызова</span><span class="sxs-lookup"><span data-stu-id="219b0-173">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="219b0-174">API-интерфейс INVITE поддерживает только одного участника при замене существующего однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="219b0-174">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="219b0-175">Если в теле запроса указано несколько участников, будет прочитан только первый участник, а остальные участники будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="219b0-175">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="219b0-176">**Примечание:** API-интерфейс INVITE поддерживает только одного участника `replacesCallId` , когда он предоставляется.</span><span class="sxs-lookup"><span data-stu-id="219b0-176">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="219b0-177">Сведения об использовании `replacesCallId` для замены существующего однорангового звонка содержатся в разделе [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md).</span><span class="sxs-lookup"><span data-stu-id="219b0-177">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="219b0-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="219b0-178">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="219b0-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="219b0-179">HTTP</span></span>](#tab/http)
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
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```
# <a name="c"></a>[<span data-ttu-id="219b0-180">C#</span><span class="sxs-lookup"><span data-stu-id="219b0-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="219b0-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="219b0-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="219b0-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="219b0-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="219b0-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="219b0-183">Response</span></span>

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
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
          "displayName": "Participant",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="219b0-184">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="219b0-184">Notification - operation completed</span></span>

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
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="219b0-185">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="219b0-185">Notification - roster updated with participant added</span></span>

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
                  "@odata.type":"#microsoft.graph.participantInfo",
                  "identity":{
                     "@odata.type":"#microsoft.graph.identitySet",
                     "user":{ 
                        "@odata.type":"#microsoft.graph.identity",
                        "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
                        "identityProvider":"AAD",
                        "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
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

><span data-ttu-id="219b0-186">**Примечание:** С состоянием "завершено" вы можете ожидать получения уведомлений о прекращении и удалении исходного однорангового звонка.</span><span class="sxs-lookup"><span data-stu-id="219b0-186">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

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
