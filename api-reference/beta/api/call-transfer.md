---
title: 'Вызовите: передача'
description: Переключение активного вызова.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 5e1a26a1b3da1af8666d8fc5bcbba619c9fad97b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824901"
---
# <a name="call-transfer"></a><span data-ttu-id="a563f-103">Вызовите: передача</span><span class="sxs-lookup"><span data-stu-id="a563f-103">call: transfer</span></span>

> <span data-ttu-id="a563f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a563f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a563f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a563f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a563f-106">Переключение активного вызова.</span><span class="sxs-lookup"><span data-stu-id="a563f-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="a563f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a563f-107">Permissions</span></span>
<span data-ttu-id="a563f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a563f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a563f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a563f-110">Permission type</span></span> | <span data-ttu-id="a563f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a563f-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="a563f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a563f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a563f-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a563f-113">Not Supported</span></span>                |
| <span data-ttu-id="a563f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a563f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a563f-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a563f-115">Not Supported</span></span>                |
| <span data-ttu-id="a563f-116">Application</span><span class="sxs-lookup"><span data-stu-id="a563f-116">Application</span></span>     | <span data-ttu-id="a563f-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="a563f-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="a563f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a563f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="a563f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a563f-119">Request headers</span></span>
| <span data-ttu-id="a563f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a563f-120">Name</span></span>          | <span data-ttu-id="a563f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a563f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a563f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a563f-122">Authorization</span></span> | <span data-ttu-id="a563f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a563f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a563f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a563f-125">Request body</span></span>
<span data-ttu-id="a563f-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a563f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a563f-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="a563f-127">Parameter</span></span>      | <span data-ttu-id="a563f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a563f-128">Type</span></span>    |<span data-ttu-id="a563f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a563f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a563f-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="a563f-130">transferTarget</span></span>|[<span data-ttu-id="a563f-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="a563f-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="a563f-132">Участник, который является целевым для переключения.</span><span class="sxs-lookup"><span data-stu-id="a563f-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="a563f-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="a563f-133">clientContext</span></span>|<span data-ttu-id="a563f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a563f-134">String</span></span>|<span data-ttu-id="a563f-135">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="a563f-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="a563f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a563f-136">Response</span></span>
<span data-ttu-id="a563f-137">Возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="a563f-137">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a563f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="a563f-138">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="a563f-139">Переключение звонка напрямую, не требующее вмешательства пользователя</span><span class="sxs-lookup"><span data-stu-id="a563f-139">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="a563f-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a563f-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a563f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a563f-141">Request</span></span>
<span data-ttu-id="a563f-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a563f-142">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="a563f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a563f-143">Response</span></span>

> <span data-ttu-id="a563f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a563f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="a563f-146">Уведомления - передача</span><span class="sxs-lookup"><span data-stu-id="a563f-146">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="a563f-147">Уведомления - передачи принятия</span><span class="sxs-lookup"><span data-stu-id="a563f-147">Notification - transfer accepted</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="a563f-148">Уведомления - завершен</span><span class="sxs-lookup"><span data-stu-id="a563f-148">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="a563f-149">Консультативное переключение</span><span class="sxs-lookup"><span data-stu-id="a563f-149">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="a563f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a563f-150">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call-transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a563f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a563f-151">Response</span></span>

> <span data-ttu-id="a563f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a563f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="a563f-154">Уведомления - передача</span><span class="sxs-lookup"><span data-stu-id="a563f-154">Notification - transferring</span></span>

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
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="a563f-155">Уведомления - передачи принятия</span><span class="sxs-lookup"><span data-stu-id="a563f-155">Notification - transfer accepted</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="a563f-156">Уведомления - завершен</span><span class="sxs-lookup"><span data-stu-id="a563f-156">Notification - terminated</span></span>

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
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
