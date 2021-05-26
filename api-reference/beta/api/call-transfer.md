---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dbc7c4b07470ea0de1e4afe492a9accfc9173d1e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664015"
---
# <a name="call-transfer"></a><span data-ttu-id="c173d-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="c173d-103">call: transfer</span></span>

<span data-ttu-id="c173d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c173d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c173d-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="c173d-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="c173d-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и Microsoft Teams пользователями, принадлежащими одному и одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="c173d-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="c173d-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="c173d-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="c173d-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="c173d-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="c173d-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="c173d-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="c173d-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="c173d-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="c173d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c173d-111">Permissions</span></span>
<span data-ttu-id="c173d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c173d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c173d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c173d-114">Permission type</span></span> | <span data-ttu-id="c173d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c173d-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="c173d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c173d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c173d-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c173d-117">Not Supported</span></span>                |
| <span data-ttu-id="c173d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c173d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c173d-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c173d-119">Not Supported</span></span>                |
| <span data-ttu-id="c173d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="c173d-120">Application</span></span>     | <span data-ttu-id="c173d-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="c173d-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c173d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c173d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="c173d-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c173d-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="c173d-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="c173d-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c173d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c173d-125">Request headers</span></span>
| <span data-ttu-id="c173d-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c173d-126">Name</span></span>          | <span data-ttu-id="c173d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c173d-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c173d-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c173d-128">Authorization</span></span> | <span data-ttu-id="c173d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c173d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c173d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c173d-131">Content-type</span></span>  | <span data-ttu-id="c173d-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c173d-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c173d-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c173d-134">Request body</span></span>
<span data-ttu-id="c173d-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c173d-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c173d-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="c173d-136">Parameter</span></span>      | <span data-ttu-id="c173d-137">Тип</span><span class="sxs-lookup"><span data-stu-id="c173d-137">Type</span></span>    |<span data-ttu-id="c173d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c173d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c173d-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="c173d-139">transferTarget</span></span>|[<span data-ttu-id="c173d-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c173d-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="c173d-141">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="c173d-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="c173d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173d-142">Response</span></span>
<span data-ttu-id="c173d-143">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="c173d-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c173d-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="c173d-144">Examples</span></span>
<span data-ttu-id="c173d-145">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="c173d-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="c173d-146">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="c173d-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="c173d-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c173d-147">Request</span></span>
<span data-ttu-id="c173d-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c173d-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c173d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c173d-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
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
    "region": "region-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c173d-150">C#</span><span class="sxs-lookup"><span data-stu-id="c173d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c173d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c173d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c173d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c173d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c173d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173d-153">Response</span></span>

> <span data-ttu-id="c173d-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c173d-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="c173d-155">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="c173d-155">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="c173d-156">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="c173d-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="c173d-157">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c173d-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="c173d-158">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="c173d-158">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="c173d-159">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="c173d-159">Notification - transfer failed</span></span>

> <span data-ttu-id="c173d-160">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="c173d-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        }
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="c173d-161">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="c173d-161">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="c173d-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c173d-162">Request</span></span>
<span data-ttu-id="c173d-163">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c173d-163">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c173d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c173d-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c173d-165">C#</span><span class="sxs-lookup"><span data-stu-id="c173d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c173d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c173d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c173d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c173d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c173d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173d-168">Response</span></span>

> <span data-ttu-id="c173d-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c173d-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="c173d-170">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="c173d-170">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="c173d-171">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="c173d-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="c173d-172">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c173d-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="c173d-173">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="c173d-173">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="c173d-174">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="c173d-174">Notification - transfer failed</span></span>

> <span data-ttu-id="c173d-175">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="c173d-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
      }
    }
  ]
}
```

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="c173d-176">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="c173d-176">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="c173d-177">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="c173d-177">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="c173d-178">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="c173d-178">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="c173d-179">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="c173d-179">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="c173d-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="c173d-180">Request</span></span>
<span data-ttu-id="c173d-181">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c173d-181">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c173d-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="c173d-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c173d-183">C#</span><span class="sxs-lookup"><span data-stu-id="c173d-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c173d-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c173d-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c173d-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173d-185">Response</span></span>

> <span data-ttu-id="c173d-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c173d-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="c173d-187">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="c173d-187">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="c173d-188">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="c173d-188">Notification - transfer accepted</span></span>

> <span data-ttu-id="c173d-189">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c173d-189">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="c173d-190">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="c173d-190">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```
### <a name="notification---transfer-failed"></a><span data-ttu-id="c173d-191">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="c173d-191">Notification - transfer failed</span></span>

> <span data-ttu-id="c173d-192">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="c173d-192">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        }
      }
    }
  ]
}
```

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="c173d-193">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="c173d-193">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="c173d-194">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="c173d-194">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="c173d-195">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="c173d-195">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="c173d-196">**Примечание.** Телефон ID — это номер телефона в формате E.164.</span><span class="sxs-lookup"><span data-stu-id="c173d-196">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="c173d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="c173d-197">Request</span></span>
<span data-ttu-id="c173d-198">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c173d-198">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c173d-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="c173d-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c173d-200">C#</span><span class="sxs-lookup"><span data-stu-id="c173d-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c173d-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c173d-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c173d-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="c173d-202">Response</span></span>

> <span data-ttu-id="c173d-203">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c173d-203">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="c173d-204">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="c173d-204">Notification - transferring</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="c173d-205">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="c173d-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="c173d-206">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c173d-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

#### <a name="notification---transfer-completed"></a><span data-ttu-id="c173d-207">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="c173d-207">Notification - transfer completed</span></span>

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
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

#### <a name="notification---transfer-failed"></a><span data-ttu-id="c173d-208">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="c173d-208">Notification - transfer failed</span></span>

> <span data-ttu-id="c173d-209">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="c173d-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        }
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


