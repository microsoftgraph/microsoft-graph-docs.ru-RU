---
title: 'Call: Transfer'
description: Передача активного вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 220a79b7ae9e14119bdc9f868577a6c4495185a3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262225"
---
# <a name="call-transfer"></a><span data-ttu-id="99e28-103">Call: Transfer</span><span class="sxs-lookup"><span data-stu-id="99e28-103">call: transfer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99e28-104">Передача активного вызова.</span><span class="sxs-lookup"><span data-stu-id="99e28-104">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e28-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99e28-105">Permissions</span></span>
<span data-ttu-id="99e28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99e28-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99e28-108">Permission type</span></span> | <span data-ttu-id="99e28-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99e28-109">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="99e28-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99e28-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="99e28-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="99e28-111">Not Supported</span></span>                |
| <span data-ttu-id="99e28-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99e28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e28-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="99e28-113">Not Supported</span></span>                |
| <span data-ttu-id="99e28-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99e28-114">Application</span></span>     | <span data-ttu-id="99e28-115">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="99e28-115">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="99e28-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99e28-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="99e28-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99e28-117">Request headers</span></span>
| <span data-ttu-id="99e28-118">Имя</span><span class="sxs-lookup"><span data-stu-id="99e28-118">Name</span></span>          | <span data-ttu-id="99e28-119">Описание</span><span class="sxs-lookup"><span data-stu-id="99e28-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="99e28-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99e28-120">Authorization</span></span> | <span data-ttu-id="99e28-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99e28-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99e28-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99e28-123">Request body</span></span>
<span data-ttu-id="99e28-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="99e28-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99e28-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="99e28-125">Parameter</span></span>      | <span data-ttu-id="99e28-126">Тип</span><span class="sxs-lookup"><span data-stu-id="99e28-126">Type</span></span>    |<span data-ttu-id="99e28-127">Описание</span><span class="sxs-lookup"><span data-stu-id="99e28-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99e28-128">Трансфертаржет</span><span class="sxs-lookup"><span data-stu-id="99e28-128">transferTarget</span></span>|[<span data-ttu-id="99e28-129">ИнвитатионпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="99e28-129">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="99e28-130">Участник, который является целевым объектом передачи.</span><span class="sxs-lookup"><span data-stu-id="99e28-130">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="99e28-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="99e28-131">clientContext</span></span>|<span data-ttu-id="99e28-132">String</span><span class="sxs-lookup"><span data-stu-id="99e28-132">String</span></span>|<span data-ttu-id="99e28-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="99e28-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="99e28-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e28-134">Response</span></span>
<span data-ttu-id="99e28-135">Возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="99e28-135">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="99e28-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="99e28-136">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="99e28-137">Прямой перенос вызовов без участия пользователя</span><span class="sxs-lookup"><span data-stu-id="99e28-137">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="99e28-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="99e28-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="99e28-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="99e28-139">Request</span></span>
<span data-ttu-id="99e28-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99e28-140">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="99e28-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e28-141">Response</span></span>

> <span data-ttu-id="99e28-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99e28-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="99e28-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="99e28-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="99e28-145">C#</span><span class="sxs-lookup"><span data-stu-id="99e28-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-transfer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99e28-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="99e28-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-transfer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="99e28-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="99e28-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-transfer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---transferring"></a><span data-ttu-id="99e28-148">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="99e28-148">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="99e28-149">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="99e28-149">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="99e28-150">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="99e28-150">Notification - terminated</span></span>

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

### <a name="consultative-transfer"></a><span data-ttu-id="99e28-151">Передача Консультативного</span><span class="sxs-lookup"><span data-stu-id="99e28-151">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="99e28-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="99e28-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="99e28-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e28-153">Response</span></span>

> <span data-ttu-id="99e28-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99e28-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="99e28-156">Передача уведомлений</span><span class="sxs-lookup"><span data-stu-id="99e28-156">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="99e28-157">Уведомление — передача принята</span><span class="sxs-lookup"><span data-stu-id="99e28-157">Notification - transfer accepted</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="99e28-158">Уведомление — прервано</span><span class="sxs-lookup"><span data-stu-id="99e28-158">Notification - terminated</span></span>

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
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-transfer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
