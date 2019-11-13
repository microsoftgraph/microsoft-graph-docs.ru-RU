---
title: 'участник: пригласить'
description: Приглашение участников в активный вызов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9c95bf23ca3e96f7ba8950e816117866456b64d2
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303032"
---
# <a name="participant-invite"></a><span data-ttu-id="79013-103">участник: пригласить</span><span class="sxs-lookup"><span data-stu-id="79013-103">participant: invite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79013-104">Приглашение участников в активный вызов.</span><span class="sxs-lookup"><span data-stu-id="79013-104">Invite participants to the active call.</span></span>

<span data-ttu-id="79013-105">Дополнительные сведения об обработке операций можно найти в разделе [коммсоператион](../resources/commsoperation.md).</span><span class="sxs-lookup"><span data-stu-id="79013-105">For more information about how to handle operations, see [commsoperation](../resources/commsoperation.md).</span></span>

><span data-ttu-id="79013-106">**Примечание:** Этот API поддерживается только для вызовов групп.</span><span class="sxs-lookup"><span data-stu-id="79013-106">**Note:** This API is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="79013-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79013-107">Permissions</span></span>
<span data-ttu-id="79013-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79013-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79013-110">Permission type</span></span> | <span data-ttu-id="79013-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79013-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="79013-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79013-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="79013-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79013-113">Not supported</span></span>                       |
| <span data-ttu-id="79013-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79013-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79013-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79013-115">Not supported</span></span>                       |
| <span data-ttu-id="79013-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79013-116">Application</span></span>     | <span data-ttu-id="79013-117">Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="79013-117">Calls.InitiateGroupCalls.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="79013-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79013-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/invite
POST /communications/calls/{id}/participants/invite
```
> <span data-ttu-id="79013-119">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="79013-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="79013-120">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="79013-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79013-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79013-121">Request headers</span></span>
| <span data-ttu-id="79013-122">Имя</span><span class="sxs-lookup"><span data-stu-id="79013-122">Name</span></span>          | <span data-ttu-id="79013-123">Описание</span><span class="sxs-lookup"><span data-stu-id="79013-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="79013-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79013-124">Authorization</span></span> | <span data-ttu-id="79013-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79013-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79013-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79013-127">Content-type</span></span>  | <span data-ttu-id="79013-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79013-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79013-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79013-130">Request body</span></span>
<span data-ttu-id="79013-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="79013-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79013-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="79013-132">Parameter</span></span>      | <span data-ttu-id="79013-133">Тип</span><span class="sxs-lookup"><span data-stu-id="79013-133">Type</span></span>    |<span data-ttu-id="79013-134">Описание</span><span class="sxs-lookup"><span data-stu-id="79013-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79013-135">participants</span><span class="sxs-lookup"><span data-stu-id="79013-135">participants</span></span>|<span data-ttu-id="79013-136">Коллекция [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="79013-136">[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection</span></span>| <span data-ttu-id="79013-137">Приглашенных участников.</span><span class="sxs-lookup"><span data-stu-id="79013-137">The participants to be invited.</span></span>|
|<span data-ttu-id="79013-138">Контекст</span><span class="sxs-lookup"><span data-stu-id="79013-138">clientContext</span></span>|<span data-ttu-id="79013-139">String</span><span class="sxs-lookup"><span data-stu-id="79013-139">String</span></span>|<span data-ttu-id="79013-140">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="79013-140">Unique Client Context string.</span></span> <span data-ttu-id="79013-141">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="79013-141">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="79013-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="79013-142">Response</span></span>
<span data-ttu-id="79013-143">Если сукксессфул, этот метод возвращает код `200 OK` отклика и заголовок Location с URI для [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="79013-143">If succsessful, this method returns a `200 OK` response code and a Location header with a URI to the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created for this request.</span></span> <span data-ttu-id="79013-144">В тексте отклика содержится созданный [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="79013-144">The body of the response contains the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) created.</span></span>

><span data-ttu-id="79013-145">**Примечание:** Когда этот API возвращает успешный ответ, все участники получат обновление списка.</span><span class="sxs-lookup"><span data-stu-id="79013-145">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>


## <a name="examples"></a><span data-ttu-id="79013-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="79013-146">Examples</span></span>
<span data-ttu-id="79013-147">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="79013-147">The following examples show how to call this API.</span></span>

> <span data-ttu-id="79013-148">**Примечание:** Объекты ответа могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="79013-148">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="79013-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79013-149">All the properties will be returned from an actual call.</span></span>

### <a name="example-1-invite-one-participant-to-an-existing-group-call"></a><span data-ttu-id="79013-150">Пример 1: приглашение одного участника на существующий вызов группы</span><span class="sxs-lookup"><span data-stu-id="79013-150">Example 1: Invite one participant to an existing group call</span></span>

##### <a name="request"></a><span data-ttu-id="79013-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="79013-151">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79013-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="79013-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79013-153">C#</span><span class="sxs-lookup"><span data-stu-id="79013-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79013-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79013-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79013-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79013-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79013-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="79013-156">Response</span></span>

> <span data-ttu-id="79013-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79013-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="79013-159">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="79013-159">Notification - operation completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="79013-160">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="79013-160">Notification - roster updated with participant added</span></span>

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

### <a name="example-2-invite-multiple-participants-to-an-existing-group-call"></a><span data-ttu-id="79013-161">Пример 2: Приглашение нескольких участников в существующий вызов групп</span><span class="sxs-lookup"><span data-stu-id="79013-161">Example 2: Invite multiple participants to an existing group call</span></span>

> <span data-ttu-id="79013-162">**Note**: существующий вызов группы должен иметь допустимый [чатинфо](../resources/chatInfo.md).</span><span class="sxs-lookup"><span data-stu-id="79013-162">**Note**: The existing group call must have a valid [chatInfo](../resources/chatInfo.md).</span></span> <span data-ttu-id="79013-163">В приглашении поддерживается до 5 участников.</span><span class="sxs-lookup"><span data-stu-id="79013-163">Inviting up to 5 participants is supported.</span></span>

##### <a name="request"></a><span data-ttu-id="79013-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="79013-164">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79013-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="79013-165">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79013-166">C#</span><span class="sxs-lookup"><span data-stu-id="79013-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-multiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79013-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79013-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-multiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79013-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79013-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-multiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79013-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="79013-169">Response</span></span>

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
##### <a name="notification---operation-completed"></a><span data-ttu-id="79013-170">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="79013-170">Notification - operation completed</span></span>
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
##### <a name="notification---roster-updated-with-participants-added"></a><span data-ttu-id="79013-171">Уведомление — список, обновленный при добавлении участников</span><span class="sxs-lookup"><span data-stu-id="79013-171">Notification - roster updated with participants added</span></span>
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

### <a name="example-3-invite-participants-to-a-an-existing-group-call-replacing-an-existing-peer-to-peer-call"></a><span data-ttu-id="79013-172">Пример 3: приглашение участников в существующий групповой вызов с заменой существующего однорангового вызова</span><span class="sxs-lookup"><span data-stu-id="79013-172">Example 3: Invite participants to a an existing group call, replacing an existing Peer-to-Peer call</span></span>


<span data-ttu-id="79013-173">API-интерфейс INVITE поддерживает только одного участника при замене существующего однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="79013-173">The invite API supports only one participant when replacing an existing peer-to-peer call.</span></span> <span data-ttu-id="79013-174">Если в теле запроса указано несколько участников, будет прочитан только первый участник, а остальные участники будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="79013-174">When multiple participants are provided in the request body, only the first participant will be read and the rest of the participants will be ignored.</span></span>


> <span data-ttu-id="79013-175">**Примечание:** API-интерфейс INVITE поддерживает только одного участника `replacesCallId` , когда он предоставляется.</span><span class="sxs-lookup"><span data-stu-id="79013-175">**Note:** The invite API supports only one participant when `replacesCallId` is provided.</span></span> 
> <span data-ttu-id="79013-176">Сведения об использовании `replacesCallId` для замены существующего однорангового звонка содержатся в разделе [инвитатионпартиЦипантинфо](../resources/invitationparticipantinfo.md).</span><span class="sxs-lookup"><span data-stu-id="79013-176">For  details about using `replacesCallId` to replace an existing peer-to-peer call, see [invitationParticipantInfo](../resources/invitationparticipantinfo.md).</span></span>

##### <a name="request"></a><span data-ttu-id="79013-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="79013-177">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79013-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="79013-178">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79013-179">C#</span><span class="sxs-lookup"><span data-stu-id="79013-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-invite-existing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79013-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79013-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-invite-existing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79013-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79013-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-invite-existing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79013-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="79013-182">Response</span></span>

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

##### <a name="notification---operation-completed"></a><span data-ttu-id="79013-183">Уведомление о завершении операции</span><span class="sxs-lookup"><span data-stu-id="79013-183">Notification - operation completed</span></span>

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

##### <a name="notification---roster-updated-with-participant-added"></a><span data-ttu-id="79013-184">Уведомление — список, обновленный при добавлении участника</span><span class="sxs-lookup"><span data-stu-id="79013-184">Notification - roster updated with participant added</span></span>

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

><span data-ttu-id="79013-185">**Примечание:** С состоянием "завершено" вы можете ожидать получения уведомлений о прекращении и удалении исходного однорангового звонка.</span><span class="sxs-lookup"><span data-stu-id="79013-185">**Note:** With a "completed" status, you can expect to receive notifications on how your original peer-to-peer call has been terminated and deleted.</span></span>

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
