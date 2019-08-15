---
title: 'Call: Transfer'
description: Передача активного вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97918efa4f55aa435214e15396283a4aa4e3cdd3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418854"
---
# <a name="call-transfer"></a><span data-ttu-id="4a12a-103">Call: Transfer</span><span class="sxs-lookup"><span data-stu-id="4a12a-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a12a-104">Передача активного вызова.</span><span class="sxs-lookup"><span data-stu-id="4a12a-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a12a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a12a-105">Permissions</span></span>
<span data-ttu-id="4a12a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a12a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a12a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a12a-108">Permission type</span></span> | <span data-ttu-id="4a12a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a12a-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="4a12a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a12a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a12a-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4a12a-111">Not Supported</span></span>                |
| <span data-ttu-id="4a12a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a12a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a12a-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4a12a-113">Not Supported</span></span>                |
| <span data-ttu-id="4a12a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a12a-114">Application</span></span>     | <span data-ttu-id="4a12a-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="4a12a-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="4a12a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a12a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="4a12a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a12a-117">Request headers</span></span>
| <span data-ttu-id="4a12a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a12a-118">Name</span></span>          | <span data-ttu-id="4a12a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4a12a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4a12a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a12a-120">Authorization</span></span> | <span data-ttu-id="4a12a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a12a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a12a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a12a-123">Request body</span></span>
<span data-ttu-id="4a12a-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4a12a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a12a-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4a12a-125">Parameter</span></span>      | <span data-ttu-id="4a12a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4a12a-126">Type</span></span>    |<span data-ttu-id="4a12a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4a12a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a12a-128">трансфертаржет</span><span class="sxs-lookup"><span data-stu-id="4a12a-128">transferTarget</span></span>|[<span data-ttu-id="4a12a-129">инвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="4a12a-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="4a12a-130">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="4a12a-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="4a12a-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="4a12a-131">clientContext</span></span>|<span data-ttu-id="4a12a-132">String</span><span class="sxs-lookup"><span data-stu-id="4a12a-132">String</span></span>|<span data-ttu-id="4a12a-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="4a12a-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="4a12a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a12a-134">Response</span></span>
<span data-ttu-id="4a12a-135">Возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="4a12a-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4a12a-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a12a-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="4a12a-137">Прямой перенос вызовов без участия пользователя</span><span class="sxs-lookup"><span data-stu-id="4a12a-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="4a12a-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4a12a-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4a12a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a12a-139">Request</span></span>
<span data-ttu-id="4a12a-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a12a-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4a12a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a12a-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a12a-142">C#</span><span class="sxs-lookup"><span data-stu-id="4a12a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a12a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a12a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a12a-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4a12a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a12a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a12a-145">Response</span></span>

> <span data-ttu-id="4a12a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a12a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="4a12a-148">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="4a12a-148">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="4a12a-149">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="4a12a-149">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="4a12a-150">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="4a12a-150">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="4a12a-151">Передача Консультативного</span><span class="sxs-lookup"><span data-stu-id="4a12a-151">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="4a12a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a12a-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="4a12a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a12a-153">Response</span></span>

> <span data-ttu-id="4a12a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a12a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="4a12a-156">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="4a12a-156">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="4a12a-157">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="4a12a-157">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="4a12a-158">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="4a12a-158">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
