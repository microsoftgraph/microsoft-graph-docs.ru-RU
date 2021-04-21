---
title: 'вызов: передача'
description: Передача активного одноранговых вызовов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 921d3473c4564627c6787364ea7021fc9fe440d7
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921022"
---
# <a name="call-transfer"></a><span data-ttu-id="e549e-103">вызов: передача</span><span class="sxs-lookup"><span data-stu-id="e549e-103">call: transfer</span></span>

<span data-ttu-id="e549e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e549e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e549e-105">Передача активного одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="e549e-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="e549e-106">**Примечание:** Это поддерживается только в том случае, если как передателем, так и целевой целью передачи являются пользователи Microsoft Teams, принадлежащие одному клиенту.</span><span class="sxs-lookup"><span data-stu-id="e549e-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="e549e-107">Передача на номер PSTN поддерживается только для экземпляра приложения.</span><span class="sxs-lookup"><span data-stu-id="e549e-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="e549e-108">Дополнительные информацию о целевой цели переноса, переноса и переноса см. в [rFC 5589.](https://tools.ietf.org/html/rfc5589#section-2)</span><span class="sxs-lookup"><span data-stu-id="e549e-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="e549e-109">Консультативная передача означает, что перед передачей перед передачей переносчик может сообщить человеку, на которого он хочет передать вызов.</span><span class="sxs-lookup"><span data-stu-id="e549e-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="e549e-110">Это противоположно переносу вызова напрямую.</span><span class="sxs-lookup"><span data-stu-id="e549e-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="e549e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e549e-111">Permissions</span></span>
<span data-ttu-id="e549e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e549e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e549e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e549e-114">Permission type</span></span> | <span data-ttu-id="e549e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e549e-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="e549e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e549e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e549e-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e549e-117">Not Supported</span></span>                |
| <span data-ttu-id="e549e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e549e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e549e-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e549e-119">Not Supported</span></span>                |
| <span data-ttu-id="e549e-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="e549e-120">Application</span></span>     | <span data-ttu-id="e549e-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="e549e-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e549e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e549e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="e549e-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e549e-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e549e-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e549e-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e549e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e549e-125">Request headers</span></span>
| <span data-ttu-id="e549e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e549e-126">Name</span></span>          | <span data-ttu-id="e549e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e549e-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e549e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e549e-128">Authorization</span></span> | <span data-ttu-id="e549e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e549e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e549e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e549e-131">Content-type</span></span>  | <span data-ttu-id="e549e-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e549e-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e549e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e549e-134">Request body</span></span>
<span data-ttu-id="e549e-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e549e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e549e-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="e549e-136">Parameter</span></span>      | <span data-ttu-id="e549e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e549e-137">Type</span></span>    |<span data-ttu-id="e549e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e549e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e549e-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="e549e-139">transferTarget</span></span>|[<span data-ttu-id="e549e-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="e549e-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="e549e-141">Участник, который является объектом переноса.</span><span class="sxs-lookup"><span data-stu-id="e549e-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="e549e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e549e-142">Response</span></span>
<span data-ttu-id="e549e-143">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="e549e-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e549e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="e549e-144">Examples</span></span>
<span data-ttu-id="e549e-145">В этих примерах покажите поток входящих вызовов в различные типы уведомлений о переносе.</span><span class="sxs-lookup"><span data-stu-id="e549e-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="e549e-146">Пример 1. Передача вызовов</span><span class="sxs-lookup"><span data-stu-id="e549e-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="e549e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e549e-147">Request</span></span>
<span data-ttu-id="e549e-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e549e-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e549e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e549e-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e549e-150">C#</span><span class="sxs-lookup"><span data-stu-id="e549e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e549e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e549e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e549e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e549e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e549e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e549e-153">Response</span></span>

> <span data-ttu-id="e549e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e549e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="e549e-156">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="e549e-156">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="e549e-157">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="e549e-157">Notification - transfer accepted</span></span>

> <span data-ttu-id="e549e-158">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e549e-158">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="e549e-159">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="e549e-159">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="e549e-160">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="e549e-160">Notification - transfer failed</span></span>

> <span data-ttu-id="e549e-161">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="e549e-161">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="e549e-162">Пример 2. Перенос консультаций</span><span class="sxs-lookup"><span data-stu-id="e549e-162">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="e549e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e549e-163">Request</span></span>
<span data-ttu-id="e549e-164">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e549e-164">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e549e-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="e549e-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e549e-166">C#</span><span class="sxs-lookup"><span data-stu-id="e549e-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e549e-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e549e-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e549e-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e549e-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e549e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e549e-169">Response</span></span>

> <span data-ttu-id="e549e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e549e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="e549e-172">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="e549e-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="e549e-173">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="e549e-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="e549e-174">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e549e-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="e549e-175">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="e549e-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="e549e-176">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="e549e-176">Notification - transfer failed</span></span>

> <span data-ttu-id="e549e-177">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="e549e-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="e549e-178">Пример 3. Передача вызовов на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="e549e-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="e549e-179">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="e549e-179">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="e549e-180">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="e549e-180">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="e549e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="e549e-181">Request</span></span>
<span data-ttu-id="e549e-182">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e549e-182">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e549e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="e549e-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e549e-184">C#</span><span class="sxs-lookup"><span data-stu-id="e549e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e549e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e549e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e549e-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="e549e-186">Response</span></span>

> <span data-ttu-id="e549e-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e549e-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="e549e-189">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="e549e-189">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="e549e-190">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="e549e-190">Notification - transfer accepted</span></span>

> <span data-ttu-id="e549e-191">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e549e-191">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="e549e-192">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="e549e-192">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="e549e-193">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="e549e-193">Notification - transfer failed</span></span>

> <span data-ttu-id="e549e-194">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="e549e-194">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="e549e-195">Пример 4. Консультативный перевод на номер PSTN</span><span class="sxs-lookup"><span data-stu-id="e549e-195">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="e549e-196">Для этого вызова требуется экземпляр приложения с присвоенным номером PSTN.</span><span class="sxs-lookup"><span data-stu-id="e549e-196">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="e549e-197">Подробные сведения см. [в материале Назначение номера телефона боту.](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot)</span><span class="sxs-lookup"><span data-stu-id="e549e-197">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="e549e-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="e549e-198">Request</span></span>
<span data-ttu-id="e549e-199">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e549e-199">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e549e-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="e549e-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e549e-201">C#</span><span class="sxs-lookup"><span data-stu-id="e549e-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e549e-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e549e-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e549e-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="e549e-203">Response</span></span>

> <span data-ttu-id="e549e-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e549e-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="e549e-206">Уведомление — перенос</span><span class="sxs-lookup"><span data-stu-id="e549e-206">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="e549e-207">Уведомление — перенос принимается</span><span class="sxs-lookup"><span data-stu-id="e549e-207">Notification - transfer accepted</span></span>

> <span data-ttu-id="e549e-208">**Примечание:** Передача, принятая, может произойти после или до неактивного состояния мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e549e-208">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="e549e-209">Уведомление - передача завершена</span><span class="sxs-lookup"><span data-stu-id="e549e-209">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="e549e-210">Уведомление — сбой передачи</span><span class="sxs-lookup"><span data-stu-id="e549e-210">Notification - transfer failed</span></span>

> <span data-ttu-id="e549e-211">**Примечание:** При сбойе передачи вызовов состояние вызова будет `established` .</span><span class="sxs-lookup"><span data-stu-id="e549e-211">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


